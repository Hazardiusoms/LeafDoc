# LeafDoc: Crop Disease Detection from Leaf Images

> Working title. Replace with your project name.

LeafDoc is an information system that identifies diseases of agricultural crops from photographs of leaves. A user uploads a leaf photo and receives the most likely diagnosis, a confidence level, and basic recommendations for treatment and prevention.

## Problem Statement

Plant diseases are a significant cause of crop losses. Early and accurate identification is critical for choosing the right treatment, but many farmers have no quick access to an agronomist, and visual diagnosis by non-experts is often slow, subjective, or wrong. Late or incorrect diagnosis leads to yield loss and unnecessary or improper use of pesticides.

Existing mobile solutions cover this problem only partially. They may lack support for Russian/Kazakh languages, region-specific crops and recommendations, transparency about accuracy, or an open API. In addition, many research models are trained on laboratory images and perform worse on real field photos. This project addresses that gap.

## Target Users

- **Farmers and small agricultural producers**: primary users who need a fast preliminary diagnosis.
- **Agronomists and agricultural consultants**: users who want a decision-support tool and a second opinion.
- **Agricultural organisations / cooperatives**: potential users of the API for integration.

## Aim and Expected Outcomes

**Aim:** to develop and evaluate a system that recognises diseases from leaf images on a held-out set of field-like images and presents the result in an understandable form.

**Expected outcomes:**

1. A trained and evaluated image classification model, compared against a baseline.
2. A backend API for diagnosis requests and diagnosis history.
3. A user interface (web application) for uploading photos and viewing results.
4. A knowledge base with descriptions and recommendations for each supported disease.
5. Documentation: requirements, architecture, evaluation report, and user instructions.

## Team and Supervisor

Student — Nursalim Onalbayev SE-2425. Responsible for whole diplom project which includes: ML engineering and AI model teaching, creating backend part and integrating API, designing and installating the web application, therefore frontend

Supervisor — Nurzhamal Kashkimbayeva. 

## Scope

**In scope**

- Photo-based diagnosis of crops and disease classes plus "healthy" for each crop.
- Single-leaf photo as input (JPG/PNG).
- Output: top-3 predictions with confidence, recommendations, "cannot determine" for low-confidence or non-leaf images.
- History of diagnoses for a user.
- Evaluation on field-like images and comparison with a baseline.

**Out of scope**

- Pest (insect) detection, weed detection.
- Drone or satellite imagery, field-level monitoring.
- Yield prediction.
- Fully offline native mobile application.
- Replacement of expert agronomic consultation: results are advisory.

## Current Status

**Stage:** planning working structure, and developing the runnable scheme structure of diploma project.

No runnable application is available yet. Runnable code will appear in `src/` in later stages.

## Selected Technologies

| Area | Technology |
|---|---|
| Machine learning | Python, PyTorch, EfficientNet / MobileNet (fine-tuning), ONNX |
| Backend | FastAPI |
| Database and storage | PostgreSQL, S3-compatible / local image storage |
| Client | React web application |
| Infrastructure | Docker, Docker Compose, GitHub Actions |
| Project management | YouTrack, Git |
| Design and diagrams | Figma, Mermaid |

## Links

- **YouTrack project:** 
- **Prototype (Figma):** 

## Repository Structure

```
docs/        Project documentation
diagrams/    Editable diagram sources and exported images
src/         Source code by component (ml/, backend/, frontend/)
tests/       Automated tests and test materials
config/      Configuration examples (placeholders only, no secrets)
```

## Setup, Execution, and Testing

In development
