# The Problem Space: AI Inference at Scale

## Why this matters
Artificial Intelligence workloads — from language models to vision transformers — are driven almost entirely by **multiply–accumulate (MAC) arrays** and the transport of data to and from them.
The toughest challenge for all accelerators, including GPUs, comes down to **memory latency, throughput, and energy**.

Inference is also deployed far more widely than training, and it’s where the greatest impact will be felt for the foreseeable future.

## Bottlenecks Today
- **Memory-bound performance**
Accelerators spend more time and energy moving weights than doing math. SRAM and DRAM accesses consume orders of magnitude more energy than local compute.

- **Power as the limiting factor**
State-of-the-art accelerators already draw tens to hundreds of watts per chip. Scaling inference for trillion-parameter models would push power consumption into physically unsustainable territory.

- **Latency from contention**
When weights, inputs, and outputs all share the same ports, cycles are lost. This creates unpredictable stalls that compound at scale.

## Industry Pressure
- **Edge Devices:** Users want near-instant inference (e.g., a 70B-parameter model on a phone) without draining batteries.
- **Data Centers:** Operators face rising electricity costs and grid limits. Serving high-context inference remotely at scale is already stretching infrastructure.
- **AGI/ASI Ambitions:** The power demand of truly general AI systems cannot be met by incremental improvements alone — breakthroughs are required.


## Looking Ahead
This repository focuses on building **benchmarks and integration frameworks**.

The technology behind BiFlow MAC Arrays (BMAC) is designed to **shift the bottleneck back to compute instead of memory**.
- **Zero weight pressure** is the #1 goal of BMAC.
- With weights held steady, the role of SRAM and DRAM becomes simply the **transport of inputs and outputs** — a directional flow that is far easier to schedule for dot products.

This simplification opens the door to:
- More predictable latency
- Reduced energy per operation
- A clear path to scaling inference workloads sustainably

The details of the architecture are reserved for partners and licensees. Here, we provide only the **public narrative and scaffolding**:
- Example configs and workflows for future benchmarks
- Documentation of bottlenecks that affect everyone
- Integration notes to illustrate how next-gen compute blocks might slot into familiar flows

