# Sakurakouji-Luna

Backend-first learning project for building a future voice-enabled character agent system.

## Status

This repository is the **future main project repo**.

Current stage:
- foundation and project-reading stage
- not full implementation yet
- the immediate focus is still learning from the reference repos

Current reference repos:
- `Reference/GPT-SoVITS/`
- `Reference/LLM-TTM-Interface/`

This repo is intentionally kept light until the architecture and learning direction are stable enough.

## Long-Term Goal

Build a system where:
- a user gives text, and later possibly speech
- the system replies as a character
- the reply stays reasonably in character
- the reply is spoken in the character's voice
- over time the system supports better context, memory, and consistency

## Architecture Direction

The future system is expected to have three major layers:

1. `Dialogue / LLM`
   - user input understanding
   - reply generation
   - role-consistent response text

2. `Persona / Memory`
   - character profile
   - lore and style constraints
   - session and memory management

3. `Voice / TTS`
   - text-to-speech generation
   - likely connected through an external speech engine such as `GPT-SoVITS`

Core principle:
- “what to say” and “how it sounds” are separate problems

## Current Working Strategy

The project will progress in stages:

1. Learn how to read and understand real repos
2. Understand `GPT-SoVITS` as a speech engine and learning repo
3. Understand `LLM-TTM-Interface` as a product-shaped reference repo
4. Build a small backend-first prototype
5. Add dialogue, persona, memory, and TTS integration gradually

This means:
- do not rush into the final full system
- do not hard-merge large external repos into this repo
- prefer small milestones and clean boundaries

## Repo Role

This repo is for:
- original system design
- future backend code
- future API and service boundaries
- future documentation that belongs to the actual project

This repo is not for:
- storing credentials
- replacing the reference repos
- dumping all experiments without structure

## Nearby Workspace Structure

Workspace-level structure currently follows this separation:

- `Reference/`
  - external learning and reference repos
- `Project/`
  - original project repos
- `Note/`
  - project notes, handoff, roadmap, learning docs
- `Backup/`
  - archived material

## Immediate Next Step

Before building this repo out, the next step is:
- continue studying `Reference/GPT-SoVITS/`
- map the inference flow
- understand the major entry points
- gain enough confidence reading real code

Only after that should larger implementation begin here.
