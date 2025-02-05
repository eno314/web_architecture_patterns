# Simple Layered Architecture

## UseCase

- not so large application
- read only
- first step

## Organizing Code

```text
├── domain (domain is often separate to use another app.)
│   ├── entity
│   ├── service
│   └── value
├── presentation
│   └── [divide by entrypoints]
├── application
│   └── [divide by features]
├── repository
│   └── [divide by features]
└── infrastructure
    └── [divide by data sources]
```

## Dependency

```text
presentation   ↘ ︎
↓
application    ↘ ︎
↓                domain
repository     ↗︎
↓
infrastructure ↗︎
````
