+++
title = "wang2022 EHR STAR"
author = ["Lucas Elvira Martín"]
date = 2025-01-09T13:21:00+01:00
draft = false
+++

## Wang2022 EHR STAR {#wang2022-ehr-star}

This paper addresses a systematic review of techniques used for visual
representation of EHR, enhanced through the use of Machine Learning.

Using the timeline representation is a point that appears in multiple reviews.

The review highlight the works of:

-   Dabek et al. Who propose a framework that transforms each event in the
    patient historical record into a node. They also employ a sunbursts chart to
    visualize diagnostics and a horizontal graph to display tests results.
-   Glueck et al. propose a visualization that represents disease sub-types and their
    evolution based on phenotype groups.
-   The work of Kwon et al. has two phases. The first one is a tool to view and
    analyze the test results based on RNN for predictive tasks. As this technology
    acts as black-box, they provide another tool that aims to help user in
    interpreting the predictive results of the first one.
-   Jin et al. work on a system that converts the clinical record from a cohort of
    patients into a sequence of events allowing the prediction of risk levels.

Another important part is the conversion between the EHR into an event sequence.
They highlight two techniques:

1.  Manual review, where users makes the changes manually
2.  Automatic review: First try to simplify the event sequence, and then an
    interface allows users to modify and improve the results provided by the tool.
