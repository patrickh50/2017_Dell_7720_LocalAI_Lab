# 2017 Dell 7720 Local AI Lab

A practical lab for exploring how well local AI models run on a 2017 Dell 7720 workstation, and for sharing what the experiments teach about AI engineering.

The goal is to make local AI approachable on modest, older hardware—not to assume a new, expensive system is required to learn. This repository is a place to share setup notes, reproducible experiments, measured results, and lessons learned.

## Lab hardware

The current workstation is reported as:

- Dell 7720 (2017)
- 32 GB RAM
- NVIDIA Quadro 4000 with 8 GB of memory

Record the exact operating system, driver, runtime, and hardware details used for each experiment. They can affect results and may differ between installations.

## Getting started

There is no one-size-fits-all installation command: supported runtimes and model requirements change, and this repository does not yet prescribe a particular operating system or inference tool. Use these steps to document a setup that works on your machine:

1. Record your operating system version and hardware.
2. Install and verify the appropriate GPU driver and local inference runtime for your operating system. Follow the runtime's official installation instructions.
3. Choose a model that fits available system and GPU memory. Start with a smaller model, and note any quantization or CPU/GPU offloading settings.
4. Run a small prompt locally and confirm the inference runtime is using the intended hardware.
5. Record the model, software versions, settings, test prompt category, output quality, and performance using the template below.

Keep downloaded model weights out of Git; document the model name and source instead. Avoid including private prompts or personal data in shared experiments.

## Experiment and results log

Add a row for each meaningful run. Do not report unmeasured estimates as benchmark results.

| Date | Model and source | Runtime / version | Settings | Task | Result quality | Performance | Lessons |
| --- | --- | --- | --- | --- | --- | --- | --- |
| | | | | | | | |

For useful comparisons, keep the task and settings consistent, and record how performance was measured (for example, time to first token, tokens per second, or total time). Include enough context for another person to repeat the run without publishing private machine identifiers or data.

## What this lab is for

- Learn how model size, quantization, context length, and hardware affect local inference.
- Compare quality and performance on a real, constrained workstation.
- Practice reproducible AI engineering: record versions, settings, measurements, and limitations.
- Share useful setup notes and honest results so others can learn from the experiments.

## Public-repository safety

This project does not need API keys, passwords, private keys, access tokens, or other credentials. Keep all secrets and personal or machine-identifying information out of commits, experiment logs, screenshots, and prompts. Use placeholders in examples; if a tool requires credentials, configure them locally through that tool's documented secret-management mechanism and do not add them here.

The `.gitignore` rules help keep common secret files and generated files out of new commits, but they are not a security check and do not remove files already tracked or erase repository history. Review staged changes before publishing.

## Contributing

Share setup notes and results that are specific, reproducible, and clear about limitations. Do not commit model weights, private data, credentials, or local configuration.
