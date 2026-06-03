# Project Instructions: anahata-os-pom

This file contains project-specific system instructions for the **anahata-os-pom** project.

**Note**: This is a **Sub-module** of **anahata-pom**. These instructions are intended to extend the shared context provided by the parent project's `anahata.md`.

## 6. Shared CI/CD & DevOps Philosophy 👑📡

Following our core standard of **Stability through Simplicity**, this project inherits its entire DevOps layer directly from the grandfather project **`anahata-pom`**:

*   **Centralized Reusable Workflows:** This repository's artifacts pipeline has been completely cleaned and modernized. It contains no duplicate setup-java, GPG keys, or maven compilation steps. It imports the master `shared-maven-build.yml` workflow dynamically from the grandfather repository in a single, self-documenting 5-line configuration.
*   **Insecure HTTP Artifactory Trust:** The runner’s environment automatically redefines the Maven blocker globally via the inherited shared template to trust `http://repo.anahata.uno` securely, keeping our child POM files pristine, completely standard, and focused purely on Java architecture.

*Força Barça!*
