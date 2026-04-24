# Contributing Guide

Thanks for your interest in contributing.

## Development Setup

1. Fork and clone the repository.
2. Create a virtual environment:
   - `python3 -m venv .venv`
   - `source .venv/bin/activate`
3. Install dependencies:
   - `pip install -r requirements.txt`

## Recommended Workflow

1. Create a feature branch from `main`.
2. Make focused, small commits with clear messages.
3. Validate notebook cells and outputs before opening a PR.
4. Update `README.md` when behavior, structure, or usage changes.

## Pull Requests

Please include:

- What changed
- Why it changed
- How to test it
- Screenshots/plots when relevant

## Code Style

- Keep code and notebook cells readable and modular.
- Prefer explicit variable names over abbreviations.
- Avoid committing large generated artifacts unless necessary.
