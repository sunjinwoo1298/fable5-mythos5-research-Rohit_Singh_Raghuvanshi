# API Integration Guide (Reference Architecture)

A future-proof architecture guide for Tekravio engineers covering Fable 5 and Mythos 5 in a restricted-access environment.

## Executive Summary

As of June 2026, Fable 5 and Mythos 5 are restricted. This guide focuses on architecture, fallback patterns, adaptive thinking concepts, and migration planning rather than exact API implementations.

## Current Availability Status

- Fable 5: Restricted
- Mythos 5: Restricted
- APIs and model identifiers may change before broader availability returns.

## Core Architecture

```text
User -> Classifier Layer -> Fable 5 -> Fallback Layer -> Opus 4.8
```

## Refusal Architecture

A refusal should be treated as a valid outcome rather than a transport error.

## Fallback Strategy

Recommended pattern:

```text
Request -> Evaluation -> Fallback -> Alternative Response
```

## Adaptive Thinking

Focus prompts on objectives, constraints, and outcomes rather than explicitly requesting reasoning steps.

## Tekravio Studio

Use future Mythos-class systems for:
- Architecture reviews
- Discovery analysis
- Migration planning

## Tekravio Academy

Use future Mythos-class systems for:
- AI mentor platforms
- Assignment evaluation
- Personalized learning plans

## Tekravio Labs

Use future Mythos-class systems for:
- Repository intelligence
- Modernization planning
- Autonomous engineering workflows

## Migration Strategy

Use a model gateway abstraction:

```text
Application -> Model Gateway -> Sonnet / Opus / Future Fable
```

## Quick Reference

- Model Class: Mythos-Class
- Status: Restricted
- Key Innovations: Classifiers, Fallbacks, Adaptive Thinking
- Current Recommendation: Build on Opus 4.8 and Sonnet while preparing infrastructure for future adoption.
