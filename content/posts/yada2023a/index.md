+++
title = "Yada2023a"
author = ["Yada", "Shuntaro and Aramaki", "Eiji"]
date = 2024-12-20T09:37:00+01:00
draft = false
+++

## HeaRT: Health Record Timeliner to Visualise Patients’ Medical History from Health Record Text {#heart-health-record-timeliner-to-visualise-patients-medical-history-from-health-record-text}

The authors propose a tool to visualize the health record of a patient in a
timeline. The system they proposed in this work, is capable of, using
state-of-the-art Language Model, recognize clinical entities and their relations
from the raw text in EHR (Electronic health record) and radiology reports. In
spate of the complexity, the free style text record offers more information
about the patient than the schematic input. Now, with the progress in NLP, there
are techniques like NER o RE (Recognition entities) that help extracting
information from the free style text.

They first focus on the use-case of visualizing the medical history of patient
and offers doctors and patients to interact with the visualization as with
google, where you can search for any information, and the system offers a short
summary of the point.


### USE CASE {#use-case}

-   Understanding long-term hospitalized patient speedily
-   Co-medical staff education
-   Patient doctor communication.


### Problems that they founded {#problems-that-they-founded}

A problem they had was the lack of relationship or matches between how medical
and hospital redact their informs. So, adding a clinical entity linking or
normalisation techniques could help to solve this issue. Also, a clinical
concept can be mentioned multiple times both in identical or different
expression, and the same term could be a reference for something different. In
this case, they need to add a coreference resolution to the NLP model.

The authors propose a tool for visualizing a patient's health record in a
timeline format. The system presented in this work leverages a state-of-the-art
Language Model to recognize clinical entities and their relationships from raw
text in Electronic Health Records (EHRs) and radiology reports. Despite the
inherent complexity, free-form text records often provide more comprehensive
information about a patient compared to structured inputs. Recent advancements
in Natural Language Processing (NLP), such as Named Entity Recognition (NER) and
Relation Extraction (RE), facilitate the extraction of valuable information from
free-form text.


### Key Use Case {#key-use-case}

The primary focus is on creating an interactive visualization of a patient’s
medical history. The system offers a functionality similar to Google search,
enabling doctors and patients to look up specific information and receive
concise summaries. The use cases include:

-   Quick understanding of long-term hospitalized patients.
-   Education for co-medical staff.
-   Improved communication between patients and doctors.


### Identified Problems and Proposed Solutions {#identified-problems-and-proposed-solutions}

1.  Inconsistencies in Medical Documentation

A significant challenge lies in the discrepancies between how different medical
institutions and hospitals draft their reports. To address this, incorporating
clinical entity linking or normalization techniques can standardize the
terminology and improve interoperability.

1.  Ambiguity in Clinical Concepts

Clinical concepts may be referenced multiple times using identical or varying
expressions. Additionally, the same term might refer to entirely different
concepts in different contexts. To resolve this, the system requires coreference
resolution capabilities within the NLP model to identify and consolidate related
references accurately.

Permanent note: yada2023 - Heart: Health record timeline
