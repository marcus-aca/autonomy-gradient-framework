---
title: "From Assisted to Validated: AI Is Now Part of How I Actually Ship"
excerpt: "AI stopped being an idea for me. It now changes how I build, test, and deliver software every day."
summary: "A personal field note on moving from chat assistance to a validated engineering loop with Codex CLI and Bedrock, where outcomes are faster, more repeatable, and clearly real."
modeTag: "Validated"
readingTimeMinutes: 3
author: "Marcus"
keywords: "individual engineer, codex cli, aws bedrock, anthropic, validated loop"
---

## Context

A month ago, AI in my workflow was mostly exploratory. I used chat for help, then moved into Copilot in the IDE, then into Codex CLI with sandbox automation.

The real shift came when I added my own wrapper framework on top of AWS Bedrock Anthropic models working with Codex CLI. That changed AI from "helpful assistant" into a repeatable delivery system I can direct and validate.

## What Changed

My loop now looks like this:

- I define the plan for the cycle
- AI proposes implementation changes
- AI applies code changes
- AI writes tests for those changes
- AI runs the tests and reports results
- I validate output and decide the next cycle

In practice, I am no longer typing every change myself. I am setting direction, enforcing quality, and validating each cycle.

## Evidence and Signals

The impact is concrete.

Work that normally would have taken 4 to 6 weeks has been compressed into roughly 3 to 4 days, including infrastructure as code and a unit test suite.

I also learned a useful tradeoff: the framework-driven loop can be slower than pure interactive IDE work on a single task, but it is far more repeatable and resumable. It creates better logs, clearer traceability, and much better visibility into what changed and why.

## Outcome and Next Step

For me, AI is no longer a concept or a future-state discussion. It is already changing how I work, and the outcome is measurable in speed, consistency, and delivery quality.

The key is discipline: structured cycles, explicit validation, and clear control boundaries. With that in place, AI integration is not theoretical. It is operational.

Next, I plan to harden policy checks and tighten evaluation criteria so the loop scales without losing reliability.
