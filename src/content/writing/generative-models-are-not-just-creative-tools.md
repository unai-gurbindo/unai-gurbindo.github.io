---
title: "Generative Models Are Not Just Creative Tools"
description: "A short note on how generative models can support robustness evaluation, not only content creation."
category: "Generative Models"
type: "Essay"
pubDate: "2026-05-11"
draft: false
---

## Generative models beyond creativity

Generative models are often presented as tools for producing images, text, audio or code. That framing is useful, but incomplete. In research, generative models can also become instruments for asking what a system has learned, where it fails and how stable its behaviour is under changed conditions.

One example is synthetic visual transformation. If a perception model performs well on clean images, we can use generative models to produce controlled variations: fog, rain, low light, snow or unusual textures. The point is not only to create plausible images, but to examine how model behaviour changes when the visual domain is modified.

## Synthetic data as a stress test

Synthetic data should not be treated as automatically equivalent to real data. A generated image may look realistic to humans while still failing to capture the statistical structure that matters for model generalisation.

This creates a useful tension. Generative models can help us stress-test AI systems, but they also force us to ask what kind of realism is relevant:

- visual realism;
- semantic realism;
- distributional realism;
- task-relevant realism.

For robustness evaluation, the last two are often the most important.

## Why this matters

If we use generative models carefully, they can help expose hidden assumptions in evaluation. They can show that a model is not only sensitive to labels, but also to background conditions, lighting, texture, acquisition process and domain structure.

In that sense, generative models are not just creative tools. They can become tools for studying shift.