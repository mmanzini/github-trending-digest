# TileKernels

**Repo:** [deepseek-ai/TileKernels](https://github.com/deepseek-ai/TileKernels)
**Language:** Python | **First seen:** 2026-04-25 | **Stars (7-day peak):** ~1,235

A GPU kernel library from the DeepSeek team, written in TileLang. Targets high-performance compute primitives for LLM training and inference workloads.

## What It Is
- TileLang is DeepSeek's domain-specific language for writing GPU tile programs
- TileKernels is the standard library / reference implementations for TileLang kernels
- Covers primitives relevant to transformer training and inference (attention, matmul, etc.)
- Not a model, not an agent framework — pure GPU infrastructure

## Why It Appeared in Trending
DeepSeek regularly surfaces in GitHub trending due to its reputation for efficient LLM infrastructure. TileKernels is of interest to ML engineers who need fine-grained GPU control below the level of PyTorch or CUDA abstractions.

## Key Takeaways
- TileLang + TileKernels represents DeepSeek's bet on a proprietary DSL for GPU kernels — analogous to Triton but in-house
- Low relevance to the AI agent / Claude Code thesis of this vault — captured here as a recurring DeepSeek infrastructure signal
- Peaked at ~1,235 stars in 7 days; notable but not breakout-level for a GPU infrastructure repo
