# AMOS

**Overview** | [Starter](https://github.com/open-amos/starter) | [Core](https://github.com/open-amos/core) | [Source Example](https://github.com/open-amos/source-example) | [Dashboard](https://github.com/open-amos/dashboard-example)

---

# Project Overview

![image](https://img.shields.io/badge/version-0.1.0-blue?style=for-the-badge) ![image](https://img.shields.io/badge/status-proof--of--concept-yellow?style=for-the-badge) 

> AMOS is currently in an early proof-of-concept stage (v0.1.0).  
> Core architecture, models, and patterns are functional but still evolving.  
> Expect incomplete coverage and active iteration across components.

## What is AMOS?

AMOS (the **Asset Management Operating System**) is a modern, open-source data stack purpose-built for private markets. It provides both emerging and established funds with the core infrastructure to turn fragmented operational data into a consistent, intelligent foundation for analysis and automation:

- Automated pipelines to extract and centralize data from multiple source systems (CRM, portfolio management, fund admin, accounting systems, etc.)
- Canonical data model for funds, portfolios, deals, accounts, and entities   
- Curated data marts and metrics for reporting and live dashboards 
- Modular, cloud-agnostic architecture for flexible deployment   
- MCP server integration — exposes AMOS data and semantics to AI assistants and notebooks using the [Model Context Protocol](https://modelcontextprotocol.io)   
- REST API — programmatic access to canonical data and metrics for external systems

AMOS is **open-source**, **cloud-agnostic**, and **vendor-independent**, giving funds full control of their architecture while enabling shared data standards across the industry. 

## Who It’s For

- **Emerging funds** looking for a lightweight but robust data foundation to support efficient operations, reliable reporting, and AI-readiness from day one  
- **Established funds** seeking to modernize legacy systems and simplify complex data architectures without vendor lock-in  

## Project Components

- **[Starter](https://github.com/open-amos/starter)** — Thin coordinator that wires AMOS Core and Source Example together
- **[Core](https://github.com/open-amos/core)** — Canonical dimensional model and curated marts 
- **[Source Example](https://github.com/open-amos/source-example)** — Sample connectors and mapping patterns  
- **[Dashboard](https://github.com/open-amos/dashboard-example)** — Example analytics and KPI dashboards built on AMOS Core  
- **REST API** — programmatic access to canonical data and metrics for external systems (coming soon)
- **MCP Server** — exposes AMOS data and semantics to AI assistants and notebooks (coming soon)
- **AMOS Utility Apps** - Prebuilt apps for common use cases, eg data extraction, reconciliation, report generation, and more (coming soon) 

## Current Scope

AMOS currently supports core private markets use cases and data sources:

- Canonical model and base metrics for **Private Equity** and **Private Credit** workflows  
- Integration patterns for key systems: **deal pipeline**, **portfolio management**, **fund administration**, and **accounting**

The existing components provide a functional foundation for consolidating and analyzing fund, portfolio, and deal data in a unified way.

## Roadmap

AMOS is evolving toward broader coverage across asset classes and workflows. Upcoming milestones include:

- Additional models and metrics for **ESG**, **impact measurement**, and for other asset types  
- Extended data connectors and transformation patterns  
- A public **REST API** for external programmatic access  
- **MCP server integration** for AI assistants and notebooks  
- Prebuilt **dashboards** and **utility apps** for reporting, reconciliation, and data management

## Customization and Extensibility

AMOS is built to be extended. You can:

- Add new source connectors and models for your specific systems  
- Define custom marts and metrics tailored to your fund’s reporting needs  
- Package extensions as standalone AMOS-compatible modules

To maintain upgrade compatibility, avoid editing the AMOS Core directly. Instead, use the **AMOS Source Example** and **AMOS Core** marts as templates to develop your own packages while keeping AMOS Core as the foundation of your data stack.

## Community & Support

- Documentation: [https://docs.amos.tech](https://docs.amos.tech)
- Issues: Use GitHub Issues within each subproject  
- Contributions: PRs welcome for connectors, mappings, transformations, tests, and documentation

## Licensing

AMOS is currently in public preview.
Each subproject README describes its temporary licensing terms.
Final open-source or source-available licenses will be published before the 1.0 release.
