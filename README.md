# CURQ 18 Documentation (`curq18-doc`)

Functional documentation and process guides for CURQ 18.

---

## Modules

* [Sales (`Sales/`)](Sales/00-overview.md): Quotations, sales orders, pricelists, shipping, and invoicing.
* [Contacts (`Contacts/`)](Contacts/00-overview.md): Companies, individuals, addresses, tags, banking, and localization.
* [Chat (`Chat/`)](Chat/00-overview.md): Channels, direct messages, voice and video calls, and record chatter.
* [CRM (`CRM/`)](CRM/00-overview.md): Leads, pipeline stages, opportunity tracking, sales teams, and lost reasons.
* [Dashboard (`Dashboard/`)](Dashboard/00-overview.md): Key performance indicators (KPIs), standard dashboards, personal user dashboards, and [General Settings](Dashboard/general-settings.md).
* [Website (`Website/`)](Website/00-overview.md): Drag-and-drop website builder, multi-website management, pages, SEO, and portal.

---

## Documentation Structure & Conventions

Each module documentation folder follows a standardized structure:

* `00-overview.md`: Module landing page and quick action cards.
* `manual/`: Core workflows and everyday operational user journeys *(such as creating quotations, sending offers, confirming orders, and invoicing)*. Files inside use numbered prefixes, such as `01-task-name.md`.
* `procedures/`: Feature configuration, system settings, master data setup, and parameter options. Files inside use numbered prefixes, such as `01-config-name.md`.
* `articles/`: Business use case scenarios, operational examples, and end-to-end commercial walkthroughs.
* `FAQs/`: Frequently asked business and system questions with short one- or two-line answers. Files inside use numbered prefixes, such as `01-topic-faq.md`.

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
└── FAQs/                     # Quick Q&A with short 1-2 line answers
    ├── 01-pricing-faq.md
    └── 02-invoicing-faq.md
```

### List Formatting Standards: Numbered vs. Bullet Lists

Follow strict functional rules when authoring lists across all documentation files:

#### Numbered Lists (`1.`, `2.`, `3.`)
Use numbers for **sequential, chronological procedures** where execution order matters:
1. **User workflows & how-tos**: Step-by-step instructions that must be performed in exact sequence *(such as navigation paths, button clicks, and submission actions)*.
2. **Setup procedures**: Multi-step configuration guides where earlier steps are prerequisites for later steps.

*Note: Never insert intermediate headings (`####`) in the middle of a numbered list, as this breaks standard Markdown list parsing (`<ol>`). If a step contains form fields, modal options, or screenshots, nest them as indented sub-bullets under that specific step number to preserve continuous numbering.*

#### Bullet Lists (`*`)
Use asterisks (`*`) exclusively for **non-sequential, unordered items** where sequence does not matter:
* **Form fields & parameters**: Explaining input fields, toggles, checkboxes, and settings in a form view.
* **Mutually exclusive choices**: Documenting selectable options or radio buttons *(such as Individual vs. Company, or Regular Invoice vs. Down Payment)*.
* **Outcomes & results**: Summarizing post-action system status, record updates, or chatter history logs.
* **Feature overviews**: High-level module capabilities, bulleted summaries, and directory indexes.

#### Quick Reference

| List Type | Markdown Syntax | Use Case | Order Dependent? |
| :--- | :---: | :--- | :---: |
| **Numbered List** | `1.`, `2.`, `3.` | Step-by-step procedures, clicks, and setup workflows | **Yes** |
| **Bullet List** | `*` | Field definitions, option choices, feature summaries, and outcomes | **No** |

