# Simple Layered Architecture

## UseCase

- not so large application
- read only
- first step

## Organizing Code

```text
├── domain
│   ├── entity
│   ├── service
│   └── value
├── presentation
│   └── [divide by entrypoints]
├── application
│   └── [divide by features]
└── infrastructure
    └── [divide by data sources]
```

## Dependency

```text
presentation   ↘ ︎
↓
application    → domain
↓
infrastructure ↗︎
````
