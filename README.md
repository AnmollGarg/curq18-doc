# CURQ 18 Documentation (`curq18-doc`)

Functional documentation and process guides for CURQ 18.

---

## Modules

* [Sales (`Sales/`)](Sales/00-overview.md): Quotations, sales orders, pricelists, shipping, and invoicing.

---

## Documentation Structure & Conventions

Each module documentation folder follows a standardized structure:

* `00-overview.md`: Module landing page and quick action cards.
* `manual/`: Step by step guides for everyday user actions in the interface. Files inside use numbered prefixes, such as `01-task-name.md`.
* `02-procedures.md`: Standard operating procedures, business policies, role responsibilities, and approval workflows.
* `03-articles/`: Feature configuration, master data setup, and technical topic deep dives.
* `04-faq.md`: Frequently asked questions and troubleshooting tips.

### Naming Conventions
* **Format**: Lowercase and hyphens (`kebab-case`).
* **Ordering**: Numbered prefix (`00-`, `01-`, etc.) to preserve navigation order.

### Example Directory Layout

```
<module-name>/
├── 00-overview.md            # Landing page and quick actions
├── manual/                   # Step by step guides for everyday user tasks
│   ├── 01-create-record.md
│   └── 02-process-action.md
├── 02-procedures.md          # Standard operating procedures and business policies
├── 03-articles/              # Feature setup, settings, and topic deep dives
│   ├── configuration-guide.md
│   └── custom-rules.md
└── 04-faq.md                 # Frequently asked questions and troubleshooting
```
