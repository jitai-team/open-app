# Open-App

Framework chassis for JitAI - Aggregates core capabilities through multiple inheritance for rapid application development.

## Overview

Open-App is the foundational framework layer of the JitAI ecosystem. It serves as an "aggregation application" that doesn't contain specific business logic but defines **multiple inheritance relationships** for a comprehensive set of framework applications.

By inheriting from Open-App, developers gain instant access to all framework capabilities without needing to manage individual dependencies.

## Architecture Role

Open-App acts as the chassis that connects JitNode engine with framework applications:

```
┌─────────────────────────────────────┐
│           JitNode Engine            │
│  (Application Loader & Runtime)     │
└──────────────┬──────────────────────┘
               │
       ┌───────▼───────┐
       │   Open-App    │  ← Framework Chassis
       │   (Chassis)   │     (Multiple Inheritance)
       └───────┬───────┘
               │
    ┌──────────┼──────────┐
    │          │          │
┌───▼───┐  ┌──▼───┐  ┌──▼───┐
│jitai- │  │jitai-│  │jitai-│  ... (All Framework Apps)
│ web   │  │ ai   │  │ auth │
└───────┘  └──────┘  └──────┘
```

## Key Features

- 🎯 **Single Inheritance Point** - Inherit once, access all framework capabilities
- 🔗 **Capability Aggregation** - Unified access to web, AI, auth, ORM, and more
- 🚀 **Rapid Development** - Build applications without managing individual framework dependencies
- 🧩 **Modular Design** - Clean separation between framework layer and business logic
- 📦 **Zero Business Logic** - Pure framework aggregation, no business code

## Inherited Framework Applications

When you inherit from Open-App, you automatically gain access to:

- **[jitai-web](https://github.com/jitai-team/jitai-web)** - Frontend interaction layer with UI components
- **[jitai-ai](https://github.com/jitai-team/jitai-ai)** - AI capabilities and LLM integration
- **[jitai-auth](https://github.com/jitai-team/jitai-auth)** - Authentication and authorization
- **[jitai-orm](https://github.com/jitai-team/jitai-orm)** - Data modeling and database adapters
- **[jitai-service](https://github.com/jitai-team/jitai-service)** - Service orchestration
- **[jitai-storage](https://github.com/jitai-team/jitai-storage)** - File storage services
- **[jitai-task](https://github.com/jitai-team/jitai-task)** - Task scheduling
- **[jitai-workflow](https://github.com/jitai-team/jitai-workflow)** - Workflow engine
- **[jitai-pay](https://github.com/jitai-team/jitai-pay)** - Payment integration
- **[jitai-message](https://github.com/jitai-team/jitai-message)** - Message notifications
- **[jitai-i18n](https://github.com/jitai-team/jitai-i18n)** - Internationalization
- **[jitai-commons](https://github.com/jitai-team/jitai-commons)** - Common utilities

## Getting Started

For development setup and contribution guidelines, please refer to the [JitAI Quickstart](https://github.com/jitai-team/quickstart) repository.

### Prerequisites

- Python >= 3.12
- Node.js >= 20 (for frontend resources)
- JitNode runtime engine

### Installation

Open-App is typically installed as part of the complete JitAI development environment. See the [quickstart guide](https://github.com/jitai-team/quickstart) for detailed setup instructions.

## Development Philosophy

Open-App follows the principle of **"Inherit Once, Access Everything"**:

1. **No Business Logic** - Open-App contains zero business code
2. **Pure Aggregation** - Only defines inheritance relationships
3. **Framework Gateway** - Single entry point to all framework capabilities
4. **Clean Separation** - Clear boundary between framework and application layers

## Community

- 📝 [Submit Issues](https://github.com/jitai-team/open-app/issues)
- 💬 [Discussions](https://github.com/jitai-team/open-app/discussions)

## Contributing

We welcome contributions! Please see our [Contribution Guide](https://github.com/jitai-team/quickstart#contribution-guide) for details on how to get started.


