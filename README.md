# 🏥 Awesome AI for Healthcare

> A community-curated list of free and open-source AI tools, datasets, APIs, and research for healthcare — with a focus on the US market, Medicaid, community health, and underserved populations.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Stars](https://img.shields.io/github/stars/Norrisont/awesome-ai-healthcare?style=social)](https://github.com/Norrisont/awesome-ai-healthcare/stargazers)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

---

## What is this?

AI is changing healthcare — but the best tools and resources are scattered across hundreds of websites, locked behind academic paywalls, or buried in GitHub with no plain-English explanation.

**This list fixes that.** Everything here is:

- ✅ Free, open-source, or has a meaningful free tier
- ✅ Working and actively maintained (verified April 2026)
- ✅ Written in plain English — no jargon
- ✅ Focused on real deployment, not just demos
- ✅ US-market relevant (HIPAA, FHIR, Medicaid, CMS standards)

---

## Who is this for?

| You are... | You will find... |
|---|---|
| A developer | APIs, SDKs, and open-source tools ready to build with |
| A researcher | Verified datasets and open-access papers |
| A startup founder | Building blocks so you don't reinvent the wheel |
| A community health org | Free platforms already used in the field |
| A policymaker | US government data, frameworks, and evidence |
| A medical student | Project ideas and learning resources |

---

## Contents

- [🔬 Diagnostic AI](#-diagnostic-ai)
- [📋 EHR & Health Data Standards](#-ehr--health-data-standards)
- [👩‍⚕️ Community & Primary Care Tools](#-community--primary-care-tools)
- [🚌 Medical Transportation (NEMT)](#-medical-transportation-nemt)
- [🧠 Mental Health AI](#-mental-health-ai)
- [🦠 Disease Surveillance & Public Health](#-disease-surveillance--public-health)
- [🔒 HIPAA, Privacy & Responsible AI](#-hipaa-privacy--responsible-ai)
- [📊 US Healthcare Datasets](#-us-healthcare-datasets)
- [📖 Research & US Policy Reports](#-research--us-policy-reports)
- [🤝 US Communities & Organizations](#-us-communities--organizations)
- [💡 Project Ideas](#-project-ideas)
- [🙌 How to Contribute](#-how-to-contribute)

---

## 🔬 Diagnostic AI

> AI tools that help clinicians identify diseases from images, symptoms, or patient data.

### Medical Imaging

- **[TorchXRayVision](https://github.com/mlmed/torchxrayvision)** — Open-source Python library of chest X-ray AI models. Pre-trained on 100,000+ labeled X-rays from public US datasets (NIH, CheXpert, MIMIC). Free under MIT license.
  > *Ready-made starting point for any chest X-ray AI project. No training from scratch required.*

- **[MONAI (Medical Open Network for AI)](https://monai.io/)** — NVIDIA's free, open-source framework for medical imaging AI. Supports CT, MRI, pathology, and X-ray. Apache 2.0 license. Widely used in US academic hospitals.
  > *The most production-ready open-source medical imaging framework available.*

- **[OHIF Viewer](https://ohif.org/)** — Free, open-source web-based DICOM viewer. Runs in any browser. Used by major US health systems for viewing radiology images.

- **[Orthanc DICOM Server](https://www.orthanc-server.com/)** — Free, lightweight open-source DICOM server. Store, retrieve, and view medical images without expensive PACS software.

- **[PyHealth](https://github.com/sunlabuiuc/PyHealth)** — Free Python library for building ML models on clinical healthcare data. Works with MIMIC-III, MIMIC-IV, OMOP-CDM, and eICU. Predicts readmissions, drug interactions, and disease progression.

### Symptom Checking & Clinical Decision Support

- **[Infermedica API](https://infermedica.com/)** — AI symptom checker and triage engine. Free developer tier. Works in English + 20 other languages. Used to build patient-facing triage apps.
  > *Patient describes symptoms → AI asks follow-up questions → recommends care level (ER, urgent care, or home).*

- **[Isabel DDx](https://www.isabelhealthcare.com/)** — AI differential diagnosis tool used by US clinicians. Research access available. Suggests possible conditions from symptom input.

- **[CDS Hooks](https://cds-hooks.org/)** — Open standard for embedding AI clinical decision support directly into any EHR (Epic, Cerner, etc.). Free specification.
  > *This is how you get an AI alert to pop up inside a doctor's EHR workflow without replacing the EHR.*

- **[OpenAPS (Open Artificial Pancreas System)](https://openaps.org/)** — Open-source DIY insulin dosing AI for Type 1 Diabetes patients. Free. Community-maintained.

---

## 📋 EHR & Health Data Standards

> Systems and tools for storing, sharing, and connecting patient records — the US way.

*The US healthcare system uses HIPAA for privacy and FHIR for data exchange. Any health app you build needs to understand both.*

### US-Focused EHR Platforms

- **[OpenEMR](https://www.open-emr.org/)** — The most widely used open-source EHR in the US. Free. HIPAA-compliant. ONC-certified. Supports e-prescribing, billing, scheduling, and patient portal. Used by thousands of US clinics.
  > *If you're building anything for a US clinic or community health center, start with OpenEMR.*

- **[Medplum](https://www.medplum.com/)** — Open-source (Apache 2.0) FHIR-native developer platform for building custom EHRs and health apps. HIPAA and SOC2 compliant out of the box. Used by US health tech startups.
  > *Think of it as Supabase but for healthcare. FHIR data storage + auth + APIs in one.*

- **[OpenMRS](https://openmrs.org/)** — Open-source EHR used in 80+ countries. Has US deployments. REST and FHIR APIs available.

### FHIR & Interoperability

*FHIR (say "fire") is the US government's required standard for health data exchange. CMS mandated FHIR APIs for all Medicaid/Medicare payers in 2021.*

- **[HAPI FHIR](https://hapifhir.io/)** — The most widely used open-source FHIR server implementation. Free. Java-based. Powers thousands of health systems and startups.

- **[Metriport](https://www.metriport.com/)** — Open-source (Apache 2.0) API for accessing patient medical records from US health information networks (CommonWell, Carequality). Supports FHIR R4, C-CDA, and PDF.
  > *Connect your app to real US patient records from thousands of hospitals and clinics.*

- **[SMART on FHIR](https://smarthealthit.org/)** — Open standard for building apps that plug into any US hospital EHR. Like OAuth but for healthcare. Free specification and SDKs.

- **[Blue Button 2.0 (CMS)](https://bluebutton.cms.gov/)** — Free API from the US Centers for Medicare & Medicaid Services. Access Medicare claims data for your patients with their consent. FHIR R4.
  > *Over 67 million Medicare beneficiaries. Their data, available to them and their apps.*

- **[Mirth Connect](https://github.com/nextgenhealthcare/connect)** — Free, open-source healthcare integration engine. Connects legacy HL7 v2 systems to modern FHIR APIs. Used by US hospitals.

### Clinical NLP

- **[cTAKES](https://ctakes.apache.org/)** — Free, open-source NLP tool from Apache. Reads clinical notes and extracts diagnoses, medications, and symptoms. Used in US academic medical centers.

- **[MedSpaCy](https://github.com/medspacy/medspacy)** — Free Python library for clinical NLP. Built on spaCy. Extracts clinical concepts from doctor notes and discharge summaries.

- **[BioBERT (HuggingFace)](https://huggingface.co/dmis-lab/biobert-v1.1)** — AI language model pre-trained on biomedical literature. Free on HuggingFace. Good for medical Q&A, NER, and relation extraction.

- **[ClinicalBERT (HuggingFace)](https://huggingface.co/medicalai/ClinicalBERT)** — BERT model fine-tuned on MIMIC clinical notes. Free. Understands clinical language better than general-purpose models.

---

## 👩‍⚕️ Community & Primary Care Tools

> Tools for federally qualified health centers (FQHCs), community health workers, and primary care in underserved US communities.

*FQHCs serve 30+ million low-income Americans. They need affordable, HIPAA-compliant tools that work in resource-limited settings.*

- **[OpenEMR](https://www.open-emr.org/)** — (See EHR section.) Free, ONC-certified EHR used by FQHCs across the US.
- **[CommCare](https://www.dimagi.com/commcare/)** — Mobile platform used by 200,000+ community health workers worldwide. Includes AI decision support. Free tier for small programs.
  > *CHW asks patient questions on their phone → app guides them to the right next step.*
- **[ODK (Open Data Kit)](https://getodk.org/)** — Free, open-source data collection for field health workers. Works offline. Used by US public health departments.
- **[KoboToolbox](https://www.kobotoolbox.org/)** — Free data collection platform used by US nonprofits and community health orgs for needs assessments.
- **[RapidPro](https://rapidpro.io/)** — Free, open-source platform for automated health messaging via SMS and WhatsApp.
- **[DHIS2](https://dhis2.org/)** — Free, open-source health data platform used by US public health departments and global health programs.

---

## 🚌 Medical Transportation (NEMT)

> Tools for building Non-Emergency Medical Transportation systems that serve Medicaid patients in the US.

*NEMT is a required Medicaid benefit. 3.6 million Americans miss medical appointments each year due to transportation. It's a $5B+ US market.*

### Routing & Dispatch (Open Source)

- **[OpenRouteService](https://openrouteservice.org/)** — Free routing API. Supports wheelchair-accessible routes, multi-stop optimization. Free API key available.
  > *Use this as the routing backbone for a CareRide-style NEMT dispatch system.*

- **[Vroom](https://github.com/VROOM-Project/vroom)** — Free, open-source vehicle route optimization. Solves which driver picks up which patient in what order. MIT license.

- **[OSRM (Open Source Routing Machine)](http://project-osrm.org/)** — Very fast, free routing engine. Processes millions of routes per day. Self-hostable.

- **[GraphHopper](https://www.graphhopper.com/)** — Open-source routing engine with free tier API. Supports vehicle routing and isochrones.

- **[OpenTripPlanner](https://www.opentripplanner.org/)** — Open-source multimodal trip planner combining public transit + walking + driving.

### US NEMT Data & Standards

- **[CMS NEMT Open Data](https://data.cms.gov/)** — Free Medicaid transportation claims and provider data.
- **[GTFS](https://gtfs.org/)** — Standard format for US public transit data. Most major cities publish free feeds.
- **[Medicaid NEMT Policy Guide (CMS)](https://www.medicaid.gov/medicaid/benefits/transportation/index.html)** — Official CMS documentation on NEMT as a Medicaid benefit.

### Communication Tools

- **[Twilio](https://www.twilio.com/)** — SMS, voice, and WhatsApp API. Free tier: 1,000 SMS/month. HIPAA-eligible.
- **[Vonage](https://www.vonage.com/communications-apis/)** — Alternative to Twilio. HIPAA BAA available.

---

## 🧠 Mental Health AI

> AI tools for mental health screening, support, and crisis detection in US clinical settings.

*1 in 5 Americans experience mental illness. Only 46% get treatment.*

- **[Woebot Health (Research)](https://woebothealth.com/)** — AI chatbot delivering Cognitive Behavioral Therapy (CBT). RCT-validated. Being used in US healthcare systems.
- **[Wysa](https://www.wysa.com/)** — AI mental health chatbot. Free for individuals. FDA Breakthrough Device designation.
- **[Crisis Text Line (Open Data)](https://www.crisistextline.org/data-philosophy/)** — Anonymized research data from 250M+ crisis messages. Free for researchers.
- **[PHQ-9 & GAD-7 (SAMHSA)](https://www.integration.samhsa.gov/clinical-practice/screening-tools)** — Free validated depression and anxiety screening tools used across the US.
- **[NIMH Mental Health Research Data](https://nda.nih.gov/)** — Free mental health research datasets for qualified researchers.

---

## 🦠 Disease Surveillance & Public Health

- **[CDC Open Data Portal](https://data.cdc.gov/)** — Free US CDC datasets: flu, COVID, chronic disease, vaccinations, mortality.
  > *The authoritative source for US public health data.*
- **[HealthMap](https://www.healthmap.org/)** — Free real-time disease outbreak tracker. Built by Harvard/Boston Children's Hospital.
- **[Epi Info (CDC)](https://www.cdc.gov/epiinfo/)** — Free epidemiology software from the CDC. Public domain.
- **[EpiNow2 (R Package)](https://github.com/epiforecasts/EpiNow2)** — Free R package for real-time epidemic tracking. Used by US state health departments.
- **[County Health Rankings (RWJF)](https://www.countyhealthrankings.org/)** — Free annual rankings for every US county. Identify where to target community health interventions.

---

## 🔒 HIPAA, Privacy & Responsible AI

*HIPAA is not optional. Any app handling Protected Health Information (PHI) must comply.*

- **[AWS HIPAA Eligible Services](https://aws.amazon.com/compliance/hipaa-eligible-services-reference/)** — Free reference list of AWS services covered under their BAA.
- **[Google Cloud HIPAA Compliance](https://cloud.google.com/security/compliance/hipaa)** — Google Cloud's HIPAA compliance guide. BAA available.
- **[AI Fairness 360 (IBM)](https://aif360.mybluemix.net/)** — Free toolkit to detect and fix bias in AI models.
  > *Most health AI is trained on non-representative data. This checks if your model treats everyone fairly.*
- **[NIST AI Risk Management Framework](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10)** — Free PDF. Referenced in FDA guidance, ONC rules, and NIW petitions.
- **[PySyft](https://github.com/OpenMined/PySyft)** — Free library for federated learning. Train AI on patient data without centralizing PHI.
- **[TensorFlow Federated](https://www.tensorflow.org/federated)** — Train shared models across hospitals without sharing patient data.
- **[OpenDP](https://opendp.org/)** — Free differential privacy library. Share health statistics without exposing individual patients.

---

## 📊 US Healthcare Datasets

### Medical Imaging

| Dataset | What it is | Size | Link |
|---|---|---|---|
| NIH Chest X-ray | X-rays with 14 disease labels | 112,000 images | [NIH Box](https://nihcc.app.box.com/v/ChestXray-NIHCC) |
| MIMIC-CXR | X-rays + radiology reports (Boston) | 227,000 images | [PhysioNet](https://physionet.org/content/mimic-cxr/2.0.0/) |
| CheXpert | Stanford Hospital X-rays | 224,000 images | [Stanford](https://stanfordmlgroup.github.io/competitions/chexpert/) |
| ISIC Archive | Skin lesion images | 70,000+ images | [isic-archive.com](https://www.isic-archive.com/) |
| EyePACS | Diabetic retinopathy images | 88,000 images | [Kaggle](https://www.kaggle.com/c/diabetic-retinopathy-detection) |

### Clinical Records (US)

| Dataset | What it is | Size | Link |
|---|---|---|---|
| MIMIC-IV | De-identified ICU records (Boston) | 300,000+ patients | [PhysioNet](https://physionet.org/content/mimiciv/2.2/) |
| eICU | Multi-center ICU data from 208 US hospitals | 200,000+ stays | [PhysioNet](https://physionet.org/content/eicu-crd/2.0/) |
| TCGA | US cancer genomics (NCI) | 11,000 patients | [cancer.gov](https://www.cancer.gov/ccg/research/genome-sequencing/tcga) |
| All of Us (NIH) | Diverse US population health data | 500,000+ participants | [allofus.nih.gov](https://allofus.nih.gov/) |

### US Public Health Data

| Dataset | What it is | Link |
|---|---|---|
| CDC WONDER | US mortality and disease surveillance | [wonder.cdc.gov](https://wonder.cdc.gov/) |
| CMS Open Payments | Medicare/Medicaid claims and provider data | [data.cms.gov](https://data.cms.gov/) |
| County Health Rankings | Health outcomes for all 3,000+ US counties | [countyhealthrankings.org](https://www.countyhealthrankings.org/) |
| AHRQ MEPS | US household healthcare spending | [ahrq.gov](https://www.ahrq.gov/meps/index.html) |

---

## 📖 Research & US Policy Reports

- **[Deep Learning for Medical Image Analysis (2017)](https://arxiv.org/abs/1702.05747)** — 9,000+ citations. Foundational paper on AI in radiology.
- **[Racial Bias in Dermatology AI (2021)](https://www.nature.com/articles/s41591-020-01192-7)** — Proves skin AI fails on dark skin tones when trained on non-diverse data.
- **[AI-First Medicaid (2025)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12663265/)** — Policy roadmap for AI within US Medicaid programs.
- **[NIST AI Risk Management Framework (2023)](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10)** — The US standard for trustworthy AI.
- **[ONC Federal Health IT Strategic Plan 2024–2030](https://www.healthit.gov/topic/onc-strategic-plan)** — Where US health IT policy is heading.
- **[FDA AI/ML SaMD Action Plan](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-aiml-enabled-medical-devices)** — Required reading if your AI tool assists in diagnosis or treatment.

---

## 🤝 US Communities & Organizations

- **[HIMSS](https://www.himss.org/)** — Largest US health IT professional organization.
- **[HL7 International](https://www.hl7.org/)** — Maintains FHIR. Free access to specifications.
- **[ONC](https://www.healthit.gov/)** — US government office for health IT policy. Free datasets and standards.
- **[AHRQ](https://www.ahrq.gov/)** — US federal agency funding health services research.
- **[Partnership on AI](https://partnershiponai.org/)** — Coalition working on responsible AI in healthcare.
- **[AI Now Institute](https://ainowinstitute.org/)** — Research on AI's social implications including health equity.
- **[National Academy of Medicine](https://nam.edu/programs/value-science-driven-health-care/artificial-intelligence-in-health-and-health-care/)** — Free reports on AI in healthcare.

---

## 💡 Project Ideas

### Beginner Friendly

- [ ] **Medicaid NEMT route optimizer** — Vroom + OpenRouteService to assign dialysis patients to drivers optimally.
- [ ] **FHIR patient data viewer** — Blue Button 2.0 web app letting Medicare patients see their claims in plain English.
- [ ] **Community health needs dashboard** — County Health Rankings + US Census data visualized by county.
- [ ] **PHQ-9 / GAD-7 intake form** — HIPAA-compliant mental health screening feeding into OpenEMR via FHIR.

### Intermediate

- [ ] **Clinical note summarizer** — MedSpaCy or ClinicalBERT extracting key info from discharge notes.
- [ ] **Medication adherence SMS bot** — Twilio + RapidPro automated reminders for Medicaid patients.
- [ ] **NEMT broker comparison tool** — Compare broker performance using CMS NEMT claims data.
- [ ] **Health equity gap finder** — MIMIC-IV + demographics + AI Fairness 360 to quantify care disparities.

### Advanced

- [ ] **Federated EHR learning network** — PySyft training a shared readmission model across OpenEMR instances.
- [ ] **Prior authorization AI assistant** — NLP drafting prior auth letters from clinical notes with evidence cited.
- [ ] **AI-powered FQHC scheduling optimizer** — Predict no-shows and optimize appointments for community health centers.

---

## 🙌 How to Contribute

1. **Fork this repo** — click "Fork" top right on GitHub
2. **Edit README.md** — find the right section and add:

```markdown
- **[Tool Name](https://verified-link.com)** — One sentence on what it does.
  > *Why it matters: One sentence on real-world US healthcare impact.*
```

3. **Open a Pull Request** — one-line description of what you added

**Rules:** ✅ Verified link ✅ Free or open-source ✅ US healthcare relevant ✅ Plain English ✅ Actively maintained ❌ No paid-only tools ❌ No self-promotion without `[Disclosure: I built this]`

---

## 📜 License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Public domain. Use it, share it, build on it.

---

*Maintained by [Morris Kithinji](https://github.com/Norrisont) and contributors · Last verified: April 2026*
