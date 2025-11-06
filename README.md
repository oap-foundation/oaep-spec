# Open Agent Exchange Protocol (OAEP) Specification

<p align="center">
  <img src="https://img.shields.io/badge/Version-0.1%20(Draft)-blue.svg" alt="Specification v0.1 (Draft)">
  <img src="https://img.shields.io/badge/Status-Public%20Draft%20for%20Discussion-orange.svg" alt="Status: Public Draft for Discussion">
  <img src="https://img.shields.io/badge/Layer-0%20(Trust%20Foundation)-lightgrey.svg" alt="Layer 0 (Trust Foundation)">
</p>

This repository contains the official technical specification for the **Open Agent Exchange Protocol (OAEP)**.

OAEP is the foundational trust layer (Layer 0) of the [Open Agent Protocol Framework](https://github.com/oap-foundation/oap-framework). It defines a universal and decentralized standard for how agents establish secure, authenticated, and trustworthy communication channels. Every interaction within the OAP ecosystem **must** begin with a successful OAEP handshake.

## The Problem Solved by OAEP

The modern internet lacks a native, decentralized identity layer. This "identity vacuum" is the root cause of widespread security issues like phishing, identity theft, and spam. Current solutions are centralized and proprietary, leading to a trade-off between security and sovereignty.

OAEP is designed to solve this fundamental problem by creating a universal "digital passport system" for the AI-to-AI economy, based on the principles of **self-sovereign identity (SSI)** and **cryptographic truth**.

## Core Concepts

OAEP standardizes the essential primitives of digital trust:

1.  **Sovereign Identity:** Defines how every agent (user, AI, organization) can create and manage their own [W3C Decentralized Identifiers (DIDs)](https://www.w3.org/TR/did-core/) and prove ownership of them.
2.  **Verifiable Credentials:** Standardizes the use of [W3C Verifiable Credentials (VCs)](https://www.w3.org/TR/vc-data-model/) as the primary data structure for agents to make provable claims about themselves (e.g., `AgentProfile`).
3.  **Secure Handshake:** Specifies a mandatory, cryptographic challenge-response handshake to establish a mutually authenticated communication channel between two agents.
4.  **Trust Management:** Defines a robust and scalable mechanism for credential revocation, ensuring that trust in the ecosystem remains dynamic and secure.

## Specification Document

The full technical specification is a work in progress and is being developed in this repository.

> **➡️ [Read the full OAEP v0.1 Specification (Draft)](/specification/v0.1.md)**
> *(Note: The spec itself should be a separate, more detailed markdown file within this repo, for example in a `/specification` folder.)*

This document details:
*   The core data objects (like `AgentProfile`).
*   The step-by-step sequence of the connection handshake.
*   The required DID methods and Verifiable Credential structures.
*   The standard for key management and revocation (`StatusList2021`).

## Status: Public Draft for Discussion

This specification is at a very early stage (**v0.1 Draft**). It is published as a "Strawman Proposal" to serve as a concrete basis for technical discussion with the developer and SSI community. We explicitly invite feedback, critique, and proposals for improvement.

## How to Contribute

This is where the core technical work happens. Your expertise is highly valued here.

*   **To propose a change or addition,** please [open a new issue](https://github.com/oap-foundation/oaep-spec/issues/new) to start a discussion. We use an RFC-style process where proposals are discussed before being formally adopted into the specification.
*   **To report a security vulnerability,** please follow the instructions in our `SECURITY.md` file.
*   **To suggest an editorial change or fix a typo,** feel free to submit a pull request directly.

Please review our main [Contribution Guidelines](https://github.com/oap-foundation/oap-framework/blob/main/CONTRIBUTING.md) before you start.

## Relationship to Other Protocols

OAEP is the foundational layer upon which all other OAP application protocols (Layer 1) are built. A successful OAEP connection is a prerequisite for using protocols like:

*   [**OACP (Open Agent Commerce Protocol)**](https://github.com/oap-foundation/oacp-spec): For fair and secure commercial transactions.
*   And many others for health, robotics, collaboration, etc.

## License

The Open Agent Exchange Protocol Specification is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). This "ShareAlike" license legally prevents the standard from being captured and closed by a proprietary fork.
