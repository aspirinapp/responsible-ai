# Responsible AI at aspirin.app

How the AI in [aspirin.app](https://aspirin.app) is designed: what it does, what it does not do and the rules we follow.

> **Stage: in development.** aspirin.app is a project in development, at the concept and research stage. Everything below describes how the app is being designed. Features, data sources and timelines are plans and may change. Nothing here is medical advice.

**Our principle: AI reads, verified data decides, and people stay in charge.**

AI is very good at reading packaging and explaining text. But it should never be the source of medical facts. That is why we keep these jobs separate.

## How a check works

| Step | Who does it | What happens |
| --- | --- | --- |
| 1. Recognise | AI | The AI reads the box. The code on the pack gives the exact medicine, batch and expiry date. |
| 2. Match | Verified data | The brand name is matched to its active ingredient using official medicine registers. |
| 3. Check | Verified data | Fixed rules run against a licensed interactions database. Nothing is guessed. |
| 4. Explain | AI | The result is put into plain words in your language, based on text approved by a pharmacist. |
| 5. Decide | People | The app informs. You and your pharmacist or doctor make the decisions. |

## What the AI does

- **Recognises the pack.** An AI model reads the box: name, strength, form and expiry date. If it isn't sure, it asks you to check.
- **Drafts plain language.** AI drafts plain-language leaflet summaries and translations. A pharmacist approves them before anyone sees them.

## What the AI does not do

These are the six safeguards built into the design:

1. **No medical facts from memory.** The AI never makes up doses, ingredients or interactions. It only rewords verified sources.
2. **Nothing medical written on the fly.** Summaries are written once per medicine, checked and then fixed. Users only see approved text.
3. **Never "safe to take".** The app explains what is known and points you to a professional. It doesn't approve or prescribe anything.
4. **Asks when unsure.** If the app isn't sure what it scanned, it asks you to compare with the box before saving.
5. **Traceable.** Every warning shows where its data comes from and which version was used.
6. **Emergency first.** Signs of an overdose or a serious reaction? The app always shows the emergency number 112 first.

## Who decides

People do. Every warning ends with a next step: talk to a pharmacist or doctor. Double doses and interactions are worked out by fixed rules on licensed medical data, and every version is logged. Feedback from users flags mistakes for review. The app never makes treatment decisions.

## Data and consent

- Clear consent for health data, and separate consent for each relative who can see it
- Stored and processed in the EU, encrypted in transit and at rest
- Photos of boxes are deleted once they have been read
- No selling of data and no advertising profiles
- You can download or delete all your data at any time
- No pharma advertising: we don't sell medicines, promote brands or sell data

## Planned data sources

| Source | Used for |
| --- | --- |
| European Medicines Agency (EMA) | Product information for medicines authorised across the EU |
| National medicine registers | Official product data and leaflets, such as BfArM (Germany), AEMPS CIMA (Spain) and ANSM (France) |
| WHO ATC classification | The international code for each active ingredient, used to spot duplicates across brands |
| GS1 DataMatrix and EMVS | The standard code on EU prescription packs: product, batch, expiry and serial number |
| Licensed interaction database | A clinically maintained database such as ABDATA or DrugBank, currently under evaluation |

These are planned data sources for launch. Licence agreements are being finalised.

## Rules we are building for

Under the EU Medical Device Regulation (MDR), software that checks interactions for a specific person is generally a medical device of at least Class IIa. We launch step by step.

| Stage | Features | Status | Standards |
| --- | --- | --- | --- |
| 1. Smart cabinet | Medicine list, expiry dates, reminders, family mode, list for the pharmacist, official leaflet with translation | Information tool, not a medical device (legal review under way) | GDPR, ISO/IEC 27001 (planned) |
| 2. Interactions | Interaction warnings through a certified partner module with CE marking | Certified partner component | MDR, IEC 62304 |
| 3. Our own device | Our own medicine safety engine, tailored to each person | CE marking, Class IIa, reviewed by a notified body | ISO 13485, ISO 14971, EU AI Act |

- **GDPR:** health data only with explicit consent (Art. 9).
- **EU AI Act:** obligations for AI in medical devices apply from August 2028. Human oversight, transparency and logging are built in now.
- **European Health Data Space:** medicine lists controlled by the patient, ready for secure exchange.

## Contact

Questions or suggestions about this document: open an issue here or email [info@aspirin.app](mailto:info@aspirin.app).

## Licence

This document is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You may share and adapt it with attribution to aspirin.app.

The aspirin.app name and logos are not covered by this licence. See [brand-assets](https://github.com/aspirinapp/brand-assets).
