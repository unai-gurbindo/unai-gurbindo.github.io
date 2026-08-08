---
title: "Why Predictive Uncertainty Is Not Enough"
description: "A non-technical introduction to why uncertainty over labels does not fully capture uncertainty under distribution shift."
category: "Uncertainty Quantification"
type: "Explainer"
pubDate: "2026-05-11"
draft: false
---

## The usual question

Many uncertainty methods ask a version of the following question: given this input, how uncertain is the model about the label?

That is an important question. If a classifier sees an image and assigns similar probabilities to several classes, predictive uncertainty can tell us that the model is unsure about the output.

But under distribution shift, this is not the only question that matters.

## A second question

We also need to ask whether the input itself belongs to the domain where the model's prediction is meaningful.

This is the motivation behind domain uncertainty. A model can be uncertain because an in-domain example is genuinely ambiguous. But it can also be uncertain because the input is outside the support or assumptions of the training domain.

These two cases can look similar if we only inspect predictive uncertainty.

## The problem under shift

Out-of-distribution inputs and difficult in-domain inputs may both produce high uncertainty. This means that a high predictive entropy score does not automatically tell us whether the model is seeing a hard but valid example or an input that should be treated as outside the deployment domain.

That distinction matters for robust evaluation, selective prediction and responsible deployment.

## A broader view of uncertainty

A trustworthy AI system should not only estimate uncertainty over labels. It should also help us reason about the relation between the input, the training data and the deployment domain.

Predictive uncertainty remains useful. But it is not the whole uncertainty story.