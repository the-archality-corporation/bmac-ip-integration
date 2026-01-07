# Bi-phase MAC Arrays (Matrix Multiply) — IP Integration Guide

This repository is currently a work in progress for Bi-phase MAC Arrays (BMAC), a new class of compute silicon blocks and chiplets targeting **efficient AI inference at every scale**.  
This repo contains **no proprietary RTL or device-level IP**. It exists to provide safe public documentation, example workflows for integration partners.

## Why BMAC?
AI inference is increasingly **memory- and power-bound**. Scaling models from billions to trillions of parameters stresses today’s accelerators.  
BMAC rethinks how multiply–accumulate (MAC) operations are orchestrated, aiming to restore **compute, not memory, as the bottleneck**.

## What’s Inside
- **docs/problem-space.md** — overview of today’s bottlenecks in AI inference  
- **docs/roadmap.md** — future plans for benchmarks and integration guides  
- **examples/integration.md** — placeholder notes for how BMAC could slot into a standard SoC or accelerator  

## Roadmap
Planned safe contributions here include:
- **Integration Notes:** high-level design flow documents for SoC or FPGA teams
- **PDK Expansions:** how to request access to validated flows with PDKs (we do not provide the PDKs)
- **Partner Hooks:** where to find documentation on IP licensing, evaluation, and support

## Today
Right now this repo contains **only placeholders**. The real IP lives elsewhere under non-public licensing and NDAs.

## Contributing
No contribution is allowed, this is a public reference reposoitory.

---
(c) 2025 Liam Coffey, The Archality Corporation. All rights reserved.

This repository contains public documentation, integration guidelines, and
example workflows related to Bi-phase MAC Arrays (Matrix Multiply).

Permission is granted to view and reference the materials in this repository
for informational and educational purposes only.

You may not copy, modify, distribute, sublicense, or use any part of this
repository, in whole or in part, for any commercial purpose without prior
written permission from The Archality Corporation.

No license of any kind is granted to the underlying intellectual property,
designs, or implementations described in this repository. The integration
guidelines are provided "as is," without warranty of any kind.

Some aspects of the technology discussed herein are patent pending.
