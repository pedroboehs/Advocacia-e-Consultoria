# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## GitHub Sync

Este projeto está configurado com sincronização automática com GitHub. A cada commit realizado localmente, as mudanças são automaticamente enviadas para o repositório remoto via um git hook (`.git/hooks/post-commit`).

**Configuração inicial:**
```bash
# Após criar o repositório em https://github.com/novo/advocacia-consultoria
git remote add origin https://github.com/seu-usuario/advocacia-consultoria.git
git branch -M main
git push -u origin main
```

**Como funciona:**
- Cada vez que você faz um `git commit`, o hook automaticamente executa `git push`
- Isso garante que todas as mudanças sejam sincronizadas com o GitHub em tempo real
- Se houver erro de sincronização, uma mensagem de aviso será exibida

## Project Overview

This is a new project for "Advocacia e Consultoria" (Legal Advocacy and Consulting). As the project develops, this document should be updated with:

- Project purpose and goals
- Tech stack and technology choices
- Architecture decisions
- Development workflow and conventions

## Getting Started

### Setup
- Document installation steps and prerequisites here as the project is initialized
- Include any environment setup required

### Common Commands
Add the key commands for this project as they're established:
- Build/compile commands
- Test execution
- Linting and formatting
- Development server startup
- Deployment commands

## Architecture & Structure

As the project grows, document:
- High-level system architecture
- Directory structure and organization
- Key modules and their responsibilities
- Data models and relationships
- Authentication and authorization patterns

## Development Workflow

Document project-specific conventions as they're established:
- Git workflow (branching strategy, commit conventions)
- Code style and formatting standards
- Testing requirements and patterns
- PR review process
- Deployment procedures

## Important Notes for Future Claude Instances

- Add project-specific knowledge here that would help future Claude Code sessions
- Document any non-obvious setup steps or gotchas
- Link to external documentation or resources
