---
title: "From Assisted to Validated: Building My Engineer-in-the-Loop Delivery Stack"
excerpt: "I moved from chat assistance to Copilot, then Codex CLI automation, and finally a Bedrock + Anthropic wrapper where I primarily validate each cycle."
summary: "A first-person operating model for AI-assisted engineering: staged tool progression, sandboxed execution, and a validated delivery loop with human sign-off."
modeTag: "Validated"
readingTimeMinutes: 3
author: "Marcus"
keywords: "individual engineer, codex cli, aws bedrock, anthropic, validated loop"
---

## Context

My adoption path was incremental. I started by using chat for coding assistance. Then I moved into IDE Copilot workflows. After that, I shifted to Codex CLI with sandbox automation so changes could be executed in a more controlled loop.

That progression changed my role from doing every step manually to validating high-velocity execution cycles.

## What Changed

The major step was building a wrapper framework that calls AWS Bedrock Anthropic models to work in conjunction with Codex CLI.

The working model now looks like this:

- define a plan for the cycle
- AI proposes changes based on that plan
- AI implements the changes
- AI writes tests for those changes
- AI runs the test cycle and reports status
- I review and validate outputs before moving to the next cycle

At this stage, my primary function is quality control and direction-setting, not manual implementation of every unit of work.

## Evidence and Signals

The practical signal is development acceleration with tighter feedback loops.

More importantly, repeatability improved:

- each cycle has a clear plan-to-output trace
- execution is resumable after interruption
- validation evidence is produced in-line with implementation
- update summaries make each handoff explicit

This created more operational visibility than purely interactive coding sessions.

## Outcome and Next Step

The result is a validated loop where AI handles proposal, implementation, and test generation, while I remain the final validator each cycle.

This is the shift that matters for individual engineers: autonomy increases, but accountability remains human-closed through systematic validation.

Next, I will harden policy checks and expand reusable cycle templates so the loop scales without losing control quality.
