# Sakurakouji-Luna

Main project repository for a long-term backend-first learning project: building a future voice-enabled character agent system.

## Project Position

This repository is the future home of the original system.

It is intentionally kept light for now because the current priority is still:

1. learning how to read real repositories
2. understanding the current reference projects
3. stabilizing architecture direction before large-scale implementation

This repo is not yet a full product and should not become a dumping ground for copied external code.

## Long-Term Goal

The long-term target is not just text-to-speech and not just a chatbot.

The target system is:

- a user-facing character agent
- able to accept text first, and later possibly speech
- able to reply in character
- able to speak the reply in the character's voice
- able to gradually improve memory, consistency, and interaction quality over time

In short, the project goal is:

- a voice-enabled character agent system

## Stable Architecture Direction

The future system should be designed as three major layers:

### 1. Dialogue / LLM

Responsibilities:

- understand user input
- generate response text
- keep replies reasonably in character
- support multi-turn interaction later

### 2. Persona / Memory

Responsibilities:

- character profile
- tone and style constraints
- lore and examples
- short-term context
- long-term memory and relationship design

### 3. Voice / TTS

Responsibilities:

- convert the final response text into speech
- preserve voice identity and style
- support later improvement in voice quality and expression

Core design rule:

- what to say and how it sounds are separate problems

The LLM layer decides the content.
The TTS layer decides the voice output.

## Current Workspace Role

This repository exists to hold:

- original system design
- future backend services
- future API boundaries
- future dialogue, memory, and orchestration code
- project-specific documentation that belongs to the final system

This repository should not be used for:

- storing credentials
- replacing external reference repositories
- merging large third-party codebases directly into the main project
- unstructured experiments without clear purpose

## Workspace Context

The current workspace is organized as:

- `Reference/`
  - external learning and reference repositories
- `Project/`
  - original project repositories
- `Note/`
  - roadmap, handoff, study notes, and stable principles
- `Backup/`
  - archived material

Current important neighbors:

- `Reference/GPT-SoVITS/`
  - speech and TTS engine reference
- `Reference/LLM-TTM-Interface/`
  - product-shaped reference implementation

This separation is intentional and should remain stable.

## Reference Repo Interpretation

### `Reference/GPT-SoVITS`

This repo is treated as:

- a learning reference
- a speech pipeline reference
- a TTS engine reference
- a possible future independent speech service

It is not the future full system repository.

### `Reference/LLM-TTM-Interface`

This repo is treated as:

- a learning reference
- an example of how a character LLM, TTS backend, and frontend can be connected
- a product-shaped prototype to study architecture and module boundaries

It is not automatically the base of the final system.

## Stable Project Principles

The following principles are already decided:

1. This is a long-term learning backbone project, not a short-term shipping sprint.
2. First learn to read, run, and understand real projects; then build the original system gradually.
3. Prefer composition over hard merging.
4. External repos should usually remain references, dependencies, or services.
5. The future main system must live in its own repo.
6. Early work should prioritize small runnable milestones over ambitious all-in builds.
7. Do not freeze too many implementation details before the foundations are stable.
8. Credentials must not be stored in this workspace.

## Current Stage

The project is currently in the foundation and repo-reading stage.

That means the main work right now is:

1. understand the structure of the reference repos
2. identify important entry points
3. trace one real inference or request flow
4. explain the flow clearly in plain language
5. only then start building small original modules here

## Working Strategy

The project should progress in small stages:

1. understand one concrete flow
2. run one concrete component
3. explain it simply
4. modify it safely
5. rebuild a minimal version in this repo

This is the default rule when unsure:

- prefer a small step
- prefer a concrete file
- prefer real input/output
- prefer one clear deliverable

## Near-Term Roadmap

Current near-term priority:

1. continue studying `Reference/GPT-SoVITS`
2. map the inference flow and major entry points
3. understand how `Reference/LLM-TTM-Interface` stitches components together
4. build a minimal backend-first prototype in this repo
5. later add dialogue, persona, memory, and TTS integration gradually

## Definition Of Progress

A step is good enough when:

- the main idea can be explained simply
- one real file or flow can be pointed out
- one small practical action can be completed

Perfect mastery is not required before moving forward.

## Repository Status

At the current stage, this repository is mainly:

- a clean project anchor
- a boundary marker between reference code and original code
- a place for future implementation once the direction is stable enough

Large implementation should begin only after the current reference-reading goals are clear enough.
