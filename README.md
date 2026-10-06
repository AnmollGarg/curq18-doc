# CURQ 18 Documentation (`curq18-doc`)

Functional documentation and process guides for CURQ 18.

---

## Modules

* [Sales (`Sales/`)](Sales/00-overview.md): Quotations, sales orders, pricelists, shipping, and invoicing.
* [Contacts (`Contacts/`)](Contacts/00-overview.md): Companies, individuals, addresses, tags, banking, and localization.
* [Chat (`Chat/`)](Chat/00-overview.md): Channels, direct messages, voice and video calls, and record chatter.
* [CRM (`CRM/`)](CRM/00-overview.md): Leads, pipeline stages, opportunity tracking, sales teams, and lost reasons.
* [Dashboard (`Dashboard/`)](Dashboard/00-overview.md): Key performance indicators (KPIs), standard dashboards, and personal user dashboards.
* [General Settings (`General-Settings/`)](General-Settings/00-overview.md): Users, companies, access rights, email servers, localization, and developer tools.

---

## Documentation Structure & Conventions

Each module documentation folder follows a standardized structure:

* `00-overview.md`: Module landing page and quick action cards.
* `manual/`: Core workflows and everyday operational user journeys *(such as creating quotations, sending offers, confirming orders, and invoicing)*. Files inside use numbered prefixes, such as `01-task-name.md`.
* `procedures/`: Feature configuration, system settings, master data setup, and parameter options. Files inside use numbered prefixes, such as `01-config-name.md`.
* `articles/`: Business use case scenarios, operational examples, and end-to-end commercial walkthroughs.
* `faq/`: Frequently asked business and system questions with short one- or two-line answers. Files inside use numbered prefixes, such as `01-topic-faq.md`.

### Naming Conventions
* **Format**: Lowercase and hyphens (`kebab-case`).
* **Ordering**: Numbered prefix (`00-`, `01-`, etc.) to preserve navigation order.

### Example Directory Layout

```
<module-name>/
├── 00-overview.md            # Landing page and quick actions
├── manual/                   # Core workflows and user journeys
│   ├── 01-create-quotation.md
│   └── 02-confirm-order.md
├── procedures/               # Feature configuration and master data setup
│   ├── 01-product-setup.md
│   └── 02-pricelists-setup.md
├── articles/                 # Business use case scenarios and commercial examples
│   ├── b2b-wholesale-pricing.md
│   └── export-delivery-flow.md
└── faq/                      # Quick Q&A with short 1-2 line answers
    ├── 01-pricing-faq.md
    └── 02-invoicing-faq.md
```
