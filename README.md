# oh-emr
OH EMR is an open-source, Myanmar-localized electronic medical record and hospital information system built on the Bahmni/OpenMRS ecosystem, with integrated billing and ERP capabilities through Odoo.

# OH EMR

### Open Health Electronic Medical Record

**Open-source. Clinical. Local.**

OH EMR is an open-source electronic medical record platform designed for healthcare organizations in Myanmar.

It is built on the **Bahmni/OpenMRS ecosystem**, with Myanmar-specific clinical workflows, localization, terminology, reporting, integrations, and implementation tools.

The goal is to provide a practical, sustainable, interoperable and locally adaptable EMR that can be used by healthcare facilities without dependence on proprietary software vendors.

---

## 🚀 Project Status

**Status:** Foundation / Pre-Alpha

**Current release:** `0.1.0-alpha` — not yet released

OH EMR is currently in the architecture, development-environment and clinical workflow design phase.

This project is **not yet recommended for production patient care**.

---

## 🎯 Vision

> Make high-quality, sustainable, open-source digital health technology accessible to healthcare organizations across Myanmar.

---

## 🩺 Mission

OH EMR aims to develop, localize and maintain an open-source electronic medical record platform that reflects the clinical workflows, healthcare environment, language and operational needs of Myanmar.

---

## 🏗️ Foundation

OH EMR builds on established open-source healthcare technologies rather than attempting to recreate an entire hospital information system from scratch.

### Core ecosystem

* **Bahmni** — hospital management and EMR platform
* **OpenMRS** — clinical record and EMR foundation
* **OpenELIS** — laboratory information system where included in the selected Bahmni distribution
* **Odoo** — billing, accounting and ERP capabilities through the Bahmni integration
* **Docker** — development and deployment foundation

Bahmni currently provides Docker-based Standard and Lite distributions and maintains separate repositories for its core, frontend, configuration, reporting and other components.

---

## 🇲🇲 Myanmar Localization

OH EMR is designed specifically to address healthcare requirements in Myanmar.

Planned localization includes:

* English and Myanmar Unicode interfaces
* Myanmar patient registration requirements
* Myanmar administrative locations
* Local clinical workflows
* Myanmar-oriented clinical forms
* Local terminology and translations
* Hospital reporting requirements
* Local implementation and training documentation

---

## 🏥 Core Clinical Modules

### Patient Management

* Patient registration
* Patient identification
* Patient search
* Duplicate patient detection
* Patient demographics
* Patient history

### Outpatient Department

* OPD registration
* Queue management
* Triage
* Vital signs
* Doctor consultation
* Diagnosis
* Investigation orders
* Prescription
* Follow-up

### Inpatient Department

* Admission
* Ward and bed management
* Initial assessment
* Daily progress notes
* Nursing documentation
* Medication administration
* Investigation tracking
* Procedures
* Discharge summary

### Pharmacy

* Medication ordering
* Prescription management
* Dispensing
* Medication inventory
* Stock management

### Laboratory

* Laboratory orders
* Sample collection
* Result entry
* Result review
* Laboratory reporting

### Imaging

* Imaging orders
* Imaging reports
* PACS integration where appropriate

---

## 💳 Billing & ERP

OH EMR will use the **Bahmni-Odoo integration architecture** for hospital billing and ERP functions rather than creating a separate accounting engine.

Planned capabilities include:

* Consultation charges
* Laboratory charges
* Imaging charges
* Procedure charges
* Medication charges
* Admission charges
* Bed charges
* Package billing
* Discounts
* Invoices
* Payments
* Refunds
* Receipts
* Financial reporting
* Inventory and procurement where appropriate

The current Bahmni Docker ecosystem includes Odoo-based billing/inventory integration, with Odoo 16 as the current default direction for the Standard Docker setup.

---

## 📊 Data Quality

Data quality is a core feature of OH EMR.

The system will progressively support:

* Structured clinical documentation
* Standardized diagnoses
* Structured vital signs
* Standardized investigations
* Structured medication orders
* Duplicate-patient detection
* Required-field validation
* Audit trails
* Documentation completeness monitoring
* Data-quality dashboards

Our principle is:

> **Capture data once, structure it correctly, and make it useful for care, operations, reporting and research.**

---

## 🔗 Interoperability

OH EMR is intended to support standards-based interoperability.

Future interoperability capabilities may include:

* REST APIs
* HL7 FHIR
* OpenMRS APIs
* Laboratory integration
* Imaging/PACS integration
* Health information exchange
* Public-health reporting
* External health-program integration

Interoperability will be introduced progressively according to actual implementation requirements.

---

## 🧠 Future AI & Analytics

AI is **not the starting point** of OH EMR.

The first priority is:

> **Good clinical workflow → high-quality data → interoperability → analytics → AI**

Future possibilities include:

* Clinical documentation assistance
* Data-quality monitoring
* Clinical decision support
* Population-health analytics
* Operational forecasting
* Research analytics

AI features will only be introduced where there is a clear clinical or operational benefit and appropriate safety and governance.

---

## 🔐 Security & Privacy

OH EMR is intended for sensitive healthcare information and therefore follows a security-by-design approach.

Planned controls include:

* Role-based access control
* Authentication
* Authorization
* Audit logging
* Secure password management
* HTTPS/TLS
* Backup and recovery
* Environment separation
* Access monitoring
* Vulnerability management

### Important

**Never commit real patient-identifiable information to this repository.**

Development and testing must use synthetic, anonymized or appropriately authorized data.

---

## 📦 Repository Structure

```text
oh-emr/
│
├── docs/             # Project and technical documentation
├── config/           # Myanmar-specific configuration
├── deployment/       # Docker and deployment configuration
├── integrations/     # External system integrations
├── testing/          # Automated and clinical testing
└── .github/          # GitHub workflows and templates
```

OH EMR will initially keep Myanmar-specific configuration and integration work separate from upstream Bahmni source code wherever practical.

---

## 🛣️ Roadmap

### Alpha 0.1

**OPD + basic billing**

* Patient registration
* Triage
* Vital signs
* Doctor consultation
* Diagnosis
* Prescription
* Basic investigations
* Pharmacy
* Billing
* Payment
* Follow-up

### Alpha 0.2

**Diagnostics + pharmacy expansion**

* Laboratory
* Imaging
* Results
* Pharmacy dispensing
* Medication inventory

### Beta 0.3

**IPD**

* Admission
* Bed management
* Nursing
* Daily progress notes
* Medication administration
* Discharge

### Beta 0.4

**Analytics**

* Hospital dashboards
* Clinical reports
* Financial reports
* Data-quality dashboards

### Pilot 0.5

**Real-world clinical implementation**

* Clinical UAT
* Hospital pilot
* Workflow evaluation
* Performance testing
* Security review
* User feedback

### v1.0

**Production-ready OH EMR**

---

## 👥 Who Can Contribute?

OH EMR welcomes contributions from:

* Doctors
* Nurses
* Pharmacists
* Laboratory professionals
* Health informaticians
* Software developers
* DevOps engineers
* UI/UX designers
* Data scientists
* Researchers
* Hospital administrators
* Students
* Digital-health organizations

Healthcare software should be built **with healthcare professionals, not only for them.**

---

## 🤝 Contribution Philosophy

We encourage:

* Open discussion
* Transparent development
* Clinical review
* Code review
* Documentation
* Testing
* Reusable solutions
* Upstream contributions where appropriate

Clinical and patient-safety-related changes require appropriate clinical review before release.

---

## 🧪 Development Status

OH EMR currently follows:

```text
Architecture
     ↓
Development Environment
     ↓
Clinical Workflow Design
     ↓
Configuration
     ↓
Development
     ↓
Testing
     ↓
Clinical UAT
     ↓
Pilot
     ↓
Production Release
```

---

## 📜 Licensing

OH EMR uses and builds upon multiple open-source projects.

Bahmni states that its own components and modifications are available under AGPL-3.0, while underlying projects have their own licenses. OH EMR will therefore maintain a third-party dependency and license inventory and will determine the appropriate licensing for each OH EMR component before public release.

See:

* `LICENSE`
* `NOTICE`
* `docs/licensing/`
* Third-party dependency inventory

---

## 🛡️ Security

For security vulnerabilities, please follow the responsible disclosure process described in:

`SECURITY.md`

Do **not** publicly disclose exploitable vulnerabilities before the project maintainers have had an opportunity to investigate and address them.

---

## 📚 Documentation

Project documentation will be developed alongside the software.

Planned documentation includes:

* Project Charter
* Architecture
* Installation Guide
* Developer Guide
* Clinical Workflow Guide
* Configuration Guide
* Deployment Guide
* User Manual
* Testing Guide
* Implementation Guide

---

## 🌏 Project Philosophy

OH EMR follows a simple principle:

> **Technology should adapt to clinical care — clinical care should not be forced to adapt to technology.**

Our priorities are:

**Clinical usefulness → Data quality → Interoperability → Sustainability → Scale**

---

## 📬 Project Status

OH EMR is currently seeking:

* Core developers
* Clinical contributors
* Health informatics contributors
* Implementation partners
* Pilot healthcare facilities
* Documentation contributors
* Testing volunteers

---

## ⚠️ Disclaimer

OH EMR is an open-source software project.

During development and testing, it must not be assumed to be suitable for clinical use without appropriate validation, configuration, security assessment, clinical governance and regulatory review.

Healthcare organizations are responsible for ensuring that their deployment meets applicable legal, regulatory, privacy, security and clinical requirements.

---

## ❤️ Built for Open Healthcare

**OH EMR**

**Open Health Electronic Medical Record**

*Open. Clinical. Local.*

Repo Structure
oh-emr/
│
├── README.md
├── LICENSE
├── NOTICE
├── SECURITY.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
│
├── docs/
│   ├── project-charter.md
│   ├── architecture.md
│   ├── roadmap.md
│   ├── clinical-workflows/
│   └── implementation/
│
├── config/
│   ├── registration/
│   ├── concepts/
│   ├── forms/
│   ├── locations/
│   └── translations/
│
├── deployment/
│   ├── docker/
│   └── scripts/
│
└── testing/
