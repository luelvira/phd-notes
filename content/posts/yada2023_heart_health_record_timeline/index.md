+++
title = "yada2023 - Heart: Health record timeline"
author = ["Lucas Elvira Martín"]
date = 2025-01-10T12:37:00+01:00
draft = false
+++

## Yada2023 - Heart: Health record timeline {#yada2023-heart-health-record-timeline}

The authors' work proposes a system to aid in the representation of EHR.

The authors analyzed existing tools and observed that most rely solely on
structured text. To address this issue, they use a state-of-the-art machine
learning techniques to process clinical histories and represent them as
timeline. The techniques they use include Name Entity Recognition (NER) and
Relation extraction (RE).

The project's use case focused on creating an interactive visualization
of patients' medical history. The system objective is:

1.  Quick Understanding of long-term hospitalized patients.
2.  Education for (co-)medical staff.
3.  Improve communication between patients and doctors.

They use JaMIE, an algorithm they developed based on BERT, to perform NER and
RE simultaneously.

The problems they found and the possible solutions are:

1.  Inconsistencies in medical documentation:
    1.  A significant challenge lies in the discrepancies between how medical
        institutions and hospitals draft their reports. To address this issue, they
        propose incorporating clinical entities linking or normalization
        techniques. These approaches aim to standardize terminology and improve
        interoperability.
2.  Ambiguity in clinical concepts:
    1.  Clinical concepts may be referenced multiple times using identical or
        varying expressions, and the same term might refer to entirely different
        concepts. To resolve this problem, the system requires co-reference resolution.

Finally, they have defined five entity categories

1.  Diseases -&gt; This category includes metadata with the grade of confidence.
    The disease could be confirmed, suspected, discarded, etc...
2.  Anatomical -&gt; This refers to parts of the body.
3.  Features -&gt; Provides additional details about the disease and the affected
    body parts
4.  Changes -&gt; Possible changes over time affecting the patient, such as diseases
    or anatomical alternations.
5.  Time -&gt; Describe when an event occur, using tags like:
    1.  timeOn: \\(E\\) happens at \\(T\\)
    2.  timeBefore: \\(E\\) happens before \\(T\\)
    3.  timeAfter: \\(E\\) happens after \\(T\\)
    4.  timeBegin: \\(E\\) starts at \\(T\\)
    5.  timeEnd: \\(E\\) finishes at \\(T\\)

---

Ref: Yada2023a
