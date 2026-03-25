# Quick Structure Example: Build vs Buy Data Pipeline

## User prompt

> "I'm thinking about whether we should build or buy our data pipeline."

## Response (Quick Structure mode)

Before structuring: one clarifying question -- are you comparing building in-house vs. buying a managed platform (e.g., Fivetran, Airbyte), or is "buy" an acquisition of a data company? I'll assume managed platform.

### Issue Tree: Build vs Buy

```
Should we build or buy our data pipeline?
├── Cost
│   ├── Build: engineering time (FTEs x months), infra, ongoing maintenance
│   └── Buy: license/SaaS fee, integration cost, vendor lock-in switching cost
├── Capability Fit
│   ├── Build: full customization, supports edge-case connectors
│   └── Buy: covers 80% of connectors out-of-box, limited on custom transforms
├── Speed to Value
│   ├── Build: 3-6 months to production-ready (typical)
│   └── Buy: 2-4 weeks to first pipelines running
├── Control & Risk
│   ├── Build: own the code, but own the bugs and on-call too
│   └── Buy: vendor dependency, but SLA-backed uptime
└── Team
    ├── Build: requires 1-2 senior data engineers (do you have them?)
    └── Buy: requires 0.5 FTE for config + monitoring
```

### Synthesis

The decision hinges on two things: (1) how custom your data sources are, and (2) whether you have the engineering capacity to build and maintain it. If most of your sources are standard SaaS tools and databases, buying gets you to production 5-10x faster and frees engineering for differentiated work. If you have proprietary data formats or need tight control over transformation logic, building gives you flexibility that no vendor will match -- but budget 3-6 months and at least one senior data engineer dedicated to it.

The most common mistake is building because it "feels" cheaper. Run the numbers: a senior data engineer costs $180-220K/yr fully loaded, and they'll spend ~40% of ongoing time on maintenance. Compare that to a $1-2K/mo SaaS tool. Build only when the capability gap justifies it, not when the sticker price looks lower.
