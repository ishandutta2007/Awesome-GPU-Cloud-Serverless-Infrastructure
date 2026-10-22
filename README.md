<div align="center">

<p align="center">
  <img src="assets/banner.svg" alt="Awesome GPU Cloud &amp; Serverless Infrastructure Banner" width="100%" />
</p>

# 🚀 Awesome GPU Cloud & Serverless Infrastructure

> ⚡ A curated ecosystem of elite GPU cloud providers, serverless GPU inference platforms, bare-metal AI superclusters, and self-hosted open-source runtimes.

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-GPU-Cloud-Serverless-Infrastructure/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-GPU-Cloud-Serverless-Infrastructure?style=social" alt="GitHub stars" /></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-GPU-Cloud-Serverless-Infrastructure/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome" /></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

</div>

---

This curated directory tracks prominent **SaaS platforms** and **open-source systems** spanning the modern **GPU Cloud, AI Infrastructure, and Serverless GPU** computing ecosystem. These solutions provide instantaneous, on-demand access to high-performance NVIDIA GPUs (H100, H200, B200, GH200, A100, RTX 4090)—as raw bare-metal virtual machines, managed Kubernetes clusters, or scale-to-zero serverless runtimes—enabling machine learning engineers and developers to train, fine-tune, and serve models without datacenter management overhead. 🛠️✨

---

## 📑 Table of Contents

- [📊 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS & Hosted GPU Platforms](#️-saas--hosted-gpu-platforms)
- [📦 Open-Source GitHub Projects](#-open-source-github-projects)
- [🏗️ Architectural Patterns & Recommendations](#️-architectural-patterns--recommendations)
- [⭐ Star History](#-star-history)
- [🤝 Support](#-support)
- [💡 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer](#️-disclaimer)

---

## 📊 Sector Overview & Market Dynamics

The global **GPU-as-a-Service (GPUaaS)** and cloud GPU instance market is estimated at **$7.4B–$16B+ in 2026** and projected to exceed **$26.6B by 2030** (~26.5% CAGR), while the broader serverless AI computing sector is scaling beyond **$30B**. 🌐📈

The sector is currently **moderately fragmented with strong oligopolistic tendencies** among specialized neoclouds (CoreWeave, Crusoe, Nebius, Lambda) competing directly against hyperscalers (AWS, Azure, GCP); while bare-metal capacity faces raw commoditization pressures, serverless orchestration, low-latency cold-start networks, and dedicated high-speed InfiniBand/NVLink fabrics are creating high-barrier "winner-take-most" advantages in enterprise foundational model training and high-throughput real-time inference. 🏎️💨

---

## ☁️ SaaS & Hosted GPU Platforms

*Platforms are sorted in descending order by estimated company valuation / scale.* 🏢💰

| Platform | Company Valuation / Scale | Starting Tier Pricing | Free Tier / Trial Limit | Key Focus & Use Cases |
| :--- | :--- | :--- | :--- | :--- |
| **[Crusoe Cloud](https://www.crusoe.ai/cloud/pricing)** | 🌿 **$31.0 Billion** valuation ($2.0B ARR run-rate) | Starts from **$0.04/vCPU-hr** (CPU) and **$1.99/GPU-hr** (L40S / A100 spot); H100 SXM from **$3.95/hr** | **No standard public free tier/trial**; promotional pilot credits issued via enterprise application and federal/institutional research consortium grants | Clean-energy powered GPU infrastructure, InfiniBand multi-node training clusters, and managed inference fine-tuning without GPU lock-in. |
| **[FluidStack](https://www.fluidstack.io/)** | 💧 **$18.0 Billion** valuation (~$660M revenue run-rate) | Starts from **$0.50/hr** (RTX 4090), **$0.70/hr** (RTX A6000), **$0.95/hr** (A100 40GB), and **$2.50/hr** (H100 SXM on-demand; **$1.80/hr** reserved) | **No free tier or public trial**; enterprise-first direct card/invoice onboarding with custom proof-of-concept testing agreements | Ultra-low-cost, high-density GPU compute with free egress and 99.9% SLA across a global distributed datacenter network. |
| **[CoreWeave](https://www.coreweave.com/)** | ⚡ **~$12.0 Billion – $19.0 Billion+** valuation / public scale (~$7.6B TTM revenue) | Starts from **$6.50/hr** (1x GH200 single chip); Hopper/Blackwell nodes start at **$49.24/hr** (8x H100 node) and **$50,224/month** (8x B200) | **14-day trial window** with custom inference credits via the **CoreWeave ARENA Pass** for qualified teams (no permanent free tier; developer grant requests reviewed individually) | Massive-scale NVIDIA HGX H100/H200/B200 superclusters, InfiniBand interconnects, and Kubernetes-native infrastructure for tier-1 AI labs. |
| **[Together AI](https://www.together.ai/)** | 🤝 **$8.3 Billion** valuation (~$1.15B ARR run-rate) | Dedicated endpoints start from **$5.49/hr** (H100) and **$8.99/hr** (B200); GPU clusters from **$3.99/hr** on-demand (**$3.09/hr** reserved); Serverless inference from **$0.0001/1K tokens** | **No free tier**; requires an initial minimum prepaid credit deposit ($5.00–$15.00) to activate API usage; up to $50,000 via startup accelerator grants | Serverless token-based inference, dedicated high-throughput endpoints, and full-stack model fine-tuning environments. |
| **[Lambda](https://lambda.ai/)** | 🧠 **$5.9 Billion – $12.0 Billion** valuation target (~$1.5B revenue target) | Starts from **$2.79/hr** (8x A100 80GB per-GPU rate), **$3.99/hr** (8x H100 SXM), and **$4.29/hr** (1x H100 SXM on-demand) | **No public free tier or automated sign-up trial**; offers academic/open-source **Lambda Research Grants** with up to **$5,000 in cloud credits** | Bare-metal instances and 1-Click Clusters with NVIDIA Quantum-2 InfiniBand for consistent, unthrottled deep learning training runs. |
| **[Scaleway](https://www.scaleway.com/)** | 🇪🇺 **$4.0 Billion+** parent scale (Iliad Group subsidiary; €15M–€40M+ regional cloud segment revenue) | Starts from **€0.35/hr** (L4 GPU instances) up to **€2.90–€3.50/hr** (H100 PCIe/SXM nodes via Kubernetes pools) | **€100 free credit trial** for new business accounts; includes a permanent free tier for first 1,000,000 tokens on Generative AI API endpoints | European cloud ecosystem with sovereign EU data residency (GDPR-compliant), managed Kubernetes GPU pools, and serverless AI functions. |
| **[Voltage Park](https://voltagepark.com/)** | ⚡ **$2.5 Billion** valuation (merged with Lightning AI; $500M+ ARR) | Starts from **$1.99/hr** (NVIDIA H100 SXM on-demand without long-term commitment) | **No free tier on bare-metal H100s**; unified Lightning AI platform provides **22 free GPU compute credits/month** (free forever tier for developer sandbox exploration) | Accessible bare-metal H100 clusters integrated with Lightning AI developer environments for distributed model training. |
| **[Prime Intellect](https://app.primeintellect.ai/)** | 🌐 **$1.0 Billion** valuation (~$100M ARR) | Real-time aggregate spot rates from **$0.68/hr** (A100 spot), **$1.23/hr** (A100 on-demand), **$1.99/hr** (GH200), **$2.35/hr** (H100), and **$2.68/hr** (B200 spot) | **No automated public free tier**; provides **$500 to $100,000 in compute credits** through Fast Compute Grants and ~$2,000 partner startup vouchers | Decentralized multi-provider GPU marketplace enabling price aggregation, global compute bursting, and distributed training. |
| **[RunPod](https://www.runpod.io/)** | 🟣 **$1.0 Billion** valuation (~$240M ARR run-rate) | Starts from **$0.20/hr** (community GPU pods / RTX 3070), **$0.44/hr** (RTX 4090), and **$0.0002/sec** (~$0.72/hr) for serverless GPU workers | **$5 to $10 promotional starter credit** occasionally available via referral/partner signups; up to **$1,000 in free credits** via RunPod Startup Program | Developer-friendly serverless GPU inference, micro-VM execution, scale-to-zero workloads, and containerized development pods. |

---

## 📦 Open-Source GitHub Projects

*Curated open-source projects for self-hosted serverless GPU runtimes, high-throughput model serving engines, and orchestration frameworks, sorted by GitHub stargazers count (descending).* 🌟🛠️

| Project | Stars | Focus & Description |
| :--- | :--- | :--- |
| **[ollama/ollama](https://github.com/ollama/ollama)** | [![GitHub stars](https://img.shields.io/github/stars/ollama/ollama?style=social&color=white)](https://github.com/ollama/ollama/stargazers) | 🦙 Get up and running with large language models locally or on private GPU nodes with single-command setup and full OpenAI API compatibility. |
| **[ggerganov/llama.cpp](https://github.com/ggerganov/llama.cpp)** | [![GitHub stars](https://img.shields.io/github/stars/ggerganov/llama.cpp?style=social&color=white)](https://github.com/ggerganov/llama.cpp/stargazers) | ⚡ Ultra-efficient LLM inference in C/C++ with state-of-the-art quantization, mixed CPU/GPU offloading, and custom CUDA/Metal backends. |
| **[vllm-project/vllm](https://github.com/vllm-project/vllm)** | [![GitHub stars](https://img.shields.io/github/stars/vllm-project/vllm?style=social&color=white)](https://github.com/vllm-project/vllm/stargazers) | 🚀 High-throughput, low-latency LLM serving engine featuring PagedAttention, speculative decoding, continuous batching, and chunked prefill. |
| **[ray-project/ray](https://github.com/ray-project/ray)** | [![GitHub stars](https://img.shields.io/github/stars/ray-project/ray?style=social&color=white)](https://github.com/ray-project/ray/stargazers) | ☀️ Unified open-source compute framework for scaling AI and Python workloads—including distributed training, data preprocessing, and Ray Serve. |
| **[sgl-project/sglang](https://github.com/sgl-project/sglang)** | [![GitHub stars](https://img.shields.io/github/stars/sgl-project/sglang?style=social&color=white)](https://github.com/sgl-project/sglang/stargazers) | 🏎️ High-performance serving framework for large language models and vision-language models with RadixAttention for fast prefix caching and multi-turn KV reuse. |
| **[NVIDIA/TensorRT](https://github.com/NVIDIA/TensorRT)** | [![GitHub stars](https://img.shields.io/github/stars/NVIDIA/TensorRT?style=social&color=white)](https://github.com/NVIDIA/TensorRT/stargazers) | 🟢 High-performance deep learning inference optimizer and runtime compiler delivering microsecond latencies on NVIDIA GPUs. |
| **[triton-inference-server/server](https://github.com/triton-inference-server/server)** | [![GitHub stars](https://img.shields.io/github/stars/triton-inference-server/server?style=social&color=white)](https://github.com/triton-inference-server/server/stargazers) | 🔱 NVIDIA enterprise inference server providing standardized multi-framework model deployment (PyTorch, ONNX, TensorRT, vLLM) with dynamic batching. |
| **[skypilot-org/skypilot](https://github.com/skypilot-org/skypilot)** | [![GitHub stars](https://img.shields.io/github/stars/skypilot-org/skypilot?style=social&color=white)](https://github.com/skypilot-org/skypilot/stargazers) | ✈️ Multi-cloud framework for seamlessly orchestrating AI/ML training and inference across 8+ GPU clouds (Lambda, RunPod, AWS, GCP, Azure) with automatic cost minimization. |
| **[bentoml/BentoML](https://github.com/bentoml/BentoML)** | [![GitHub stars](https://img.shields.io/github/stars/bentoml/BentoML?style=social&color=white)](https://github.com/bentoml/BentoML/stargazers) | 🍱 Python framework for building reliable, production-ready AI services, custom compound AI systems, and containerized scale-to-zero GPU deployments. |
| **[kserve/kserve](https://github.com/kserve/kserve)** | [![GitHub stars](https://img.shields.io/github/stars/kserve/kserve?style=social&color=white)](https://github.com/kserve/kserve/stargazers) | ⛵ Standardized, Kubernetes-native serverless model serving with autoscaling, scale-to-zero, GPU resource scheduling, and canary rollouts. |
| **[beam-cloud/beta9](https://github.com/beam-cloud/beta9)** | [![GitHub stars](https://img.shields.io/github/stars/beam-cloud/beta9?style=social&color=white)](https://github.com/beam-cloud/beta9/stargazers) | 💡 Open-source Modal alternative for self-hosted serverless GPU compute—write Python/TypeScript decorators for inference, sandboxes, and checkpoint restore. |
| **[runpod/runpod-python](https://github.com/runpod/runpod-python)** | [![GitHub stars](https://img.shields.io/github/stars/runpod/runpod-python?style=social&color=white)](https://github.com/runpod/runpod-python/stargazers) | 🐍 Official open-source Python SDK and serverless worker runtime for deploying and automating serverless GPU endpoints on RunPod. |

---

## 🏗️ Architectural Patterns & Recommendations

- 🔄 **Serverless Scale-to-Zero Inference**: Use **[beam-cloud/beta9](https://github.com/beam-cloud/beta9)** or **[bentoml/BentoML](https://github.com/bentoml/BentoML)** for self-hosting serverless containers on your own Kubernetes cluster, or deploy to managed serverless workers on **[RunPod](https://www.runpod.io/)** / **[Together AI](https://www.together.ai/)**.
- 🚀 **Maximum Inference Throughput**: Standardize on **[vllm-project/vllm](https://github.com/vllm-project/vllm)** or **[sgl-project/sglang](https://github.com/sgl-project/sglang)** backed by **[triton-inference-server/server](https://github.com/triton-inference-server/server)** on bare-metal or reserved instances from **[Lambda](https://lambda.ai/)** or **[Nebius](https://nebius.com/)**.
- 🔀 **Multi-Cloud Arbitrage & Fallback**: Run **[skypilot-org/skypilot](https://github.com/skypilot-org/skypilot)** to burst workloads across disparate providers or compare live bidding prices using **[Prime Intellect](https://app.primeintellect.ai/)**.
- 🌐 **Ultra-Scale Distributed Training**: Reserve dedicated NVIDIA Quantum-2 InfiniBand HGX clusters on **[CoreWeave](https://www.coreweave.com/)**, **[Crusoe Cloud](https://www.crusoe.ai/)**, or **[Lambda](https://lambda.ai/)** to eliminate multi-node communication bottlenecks.

---

##  Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-GPU-Cloud-Serverless-Infrastructure&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-GPU-Cloud-Serverless-Infrastructure&type=date&legend=top-left)

---

## 🤝 Support

Thank you so much for exploring and supporting **Awesome GPU Cloud & Serverless Infrastructure**! ❤️

If you find this repository valuable:
- ⭐ **Star** this repository on GitHub to help others discover it.
- 🍴 **Fork** it and submit a pull request with new providers, frameworks, and benchmarks.
- 📢 **Share** it with your network, AI infrastructure teammates, and ML engineering peers.
- ☕ **Buy me a coffee**: If you'd like to support continued maintenance and curation of open AI infrastructure tooling, you can sponsor through the [GitHub Sponsors Dashboard](https://github.com/sponsors/ishandutta2007). Your support is greatly appreciated!

---

## 💡 How to Contribute

Contributions are welcome! Help keep this ecosystem tracker accurate, objective, and up to date: 🤝✨

1. Fork the repository.
2. Add or update entries in `README.md` following the tabular format and guidelines:
   - Provide exact pricing tiers and verified free tier / credit terms.
   - For open-source projects, include the repository URL and descriptive summary.
3. Submit a pull request with a concise description of your changes.

---

## ⚠️ Disclaimer

- This is a **community-curated** list for informational purposes.
- Cloud GPU pricing and promotional credit availability fluctuate frequently; please verify current rates and quotas directly with providers prior to production commitments.
- Certain high-end instances (such as NVIDIA HGX Hopper H100/H200 and Blackwell B200) enforce minimum rental allocations (e.g., full 8-GPU nodes).
# Awesome-GPU-Cloud-Serverless-Infrastructure

## Top GPU Cloud & Serverless Infrastructure Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Serverless GPU Inference, Bare-Metal GPU Clouds & Self-Hosted Container Runtimes*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **GPU Cloud & Serverless Infrastructure**. These tools provide on-demand access to NVIDIA GPUs—either as raw virtual machines, managed Kubernetes clusters, or true serverless runtimes that scale to zero—enabling AI teams to train and serve models without owning datacenter hardware.



**Examples** include CoreWeave, Lambda, Crusoe Cloud, RunPod, Together AI, Nebius AI, FluidStack, Voltage Park, Scaleway, and Prime Intellect (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding vendor lock-in, and running serverless GPU workloads on your own infrastructure—ideal for teams that need cost predictability, data sovereignty, or the ability to burst across multiple providers. The open-source serverless GPU landscape is anchored by **Beam** (the open-source Modal alternative, self-hostable and production-proven), with **RunPod's SDK** providing programmatic control over their managed platform and **NVIDIA's open-source stack** (Triton, TensorRT) offering inference serving primitives that underpin many managed services.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CoreWeave](https://www.coreweave.com/)**  

  NVIDIA-only GPU cloud built for large-scale training and inference. **Pricing structure**: on-demand, spot (up to 60% off with interruption risk), and reserved multi-year contracts (negotiated, up to 60% discount). **Critical caveat**: HGX instances rent **eight GPUs at a time**—Hopper and Blackwell cannot be provisioned as single on-demand GPUs. Only GH200 rents as a single chip at **$6.50/hour**. An 8x H100 node lists at **$49.24/hour** ($6.16/GPU-hour); 8x B200 at **$68.80/hour** ($8.60/GPU-hour) . Best for teams that can commit to full-node workloads and negotiate reserved capacity.



- **[Lambda](https://lambda.ai/)**  

  AI cloud with first-party datacenters and consistent instance behavior. **On-demand pricing** (per GPU-hour, self-serve): 1x H100 SXM **$4.29**, 8x H100 SXM **$3.99**, 8x A100 80GB **$2.79**. **1-Click Clusters** for multi-node training with InfiniBand are the differentiated product for large training runs. **No serverless tier**—Lambda is bare-metal or cluster rental only. Best for teams that want hardware consistency and a straightforward pricing page without broker intermediation.



- **[Crusoe Cloud](https://www.crusoe.ai/cloud/pricing)**  

  GPU cloud with spot, on-demand, and reserved options. **Published on-demand rates**: H200 **$4.29/GPU-hour**, H100 80GB **$3.90/GPU-hour**, A100 80GB SXM **$2.30/GPU-hour**, L40S **$1.50/GPU-hour**, AMD MI300X **$3.45/GPU-hour**. GB200 and some higher-tier models are contact-sales . Best for teams that want flexible contract terms and a mix of raw compute and managed AI services.



- **[RunPod](https://www.runpod.io/)**  

  GPU cloud specializing in **serverless GPU inference** and pod-based development. **Serverless pricing** is per-second: **H100 PRO at $0.00116/second** (~$4.18/hour), **A100 at $0.00076/second** (~$2.74/hour), **B200 at $0.00240/second** (~$8.64/hour). Flex workers scale to zero; active workers run 24/7 with discounts via sales . The **`runpod-python` SDK** allows programmatic deployment of serverless endpoints and GPU pods. Best for developers who want a managed serverless GPU experience with an SDK-first workflow.



- **[Together AI](https://www.together.ai/)**  

  AI platform offering **three distinct tiers**: serverless (per-token), dedicated endpoints (per-minute per replica), and raw GPU clusters. **Dedicated endpoint pricing**: H100 **$5.49/hour**, B200 **$8.99/hour**; H200 and GB300 are contact-sales . Best for teams that want to start serverless and graduate to dedicated or cluster as volume grows.



- **[Nebius AI](https://nebius.com/)**  

  European-headquartered GPU cloud with transparent published pricing. **From October 1, 2026**: **H200 NVLink at $5.40/GPU-hour** (up from $4.50), **H100 NVLink at $4.50/GPU-hour** (up from $3.85) . Best for teams that want published, predictable rates without sales negotiations, particularly in EU regions.



- **[FluidStack](https://www.fluidstack.io/)**  

  Budget-friendly GPU cloud. **H100 SXM**: on-demand **$2.50/hour**, reserved **$1.80/hour** . Entry-level options include RTX 4090 and A6000 at lower rates. **Free egress** and 99.9% SLA. Best for cost-sensitive inference workloads where H100 performance is not strictly necessary.



- **[Voltage Park](https://voltagepark.com/)**  

  GPU cloud with published **H100 on-demand floor at $1.99/GPU-hour**—one of the lowest advertised H100 rates without a contract . H200 and InfiniBand on-demand, plus Long-Term Reserve, are contact-sales. Best for teams that want low-cost H100 access without commitment.



- **[Scaleway](https://www.scaleway.com/)**  

  European cloud provider with GPU instances. **H100 PCIe at €2.73/GPU-hour**—the cheapest openly published H100 option among major providers as of October 2026, versus ~$6.88 on AWS and ~$12.29 on Azure . No egress charges on compute and network. Best for European teams requiring GDPR-aligned data residency and cost-sensitive inference.



- **[Prime Intellect](https://app.primeintellect.ai/)**  

  GPU marketplace aggregating multiple providers with **real-time pricing**. **H100 at $2.35/hour**, H200 at **$4.05/hour**, B200 at **$7.55/hour** (spot **$2.68**), GH200 at **$1.99/hour**, A100 at **$1.23/hour** (spot **$0.68**), A6000 at **$0.54/hour** . Best for teams that want to compare live prices across providers and optimize cost per workload.



## Open-Source GitHub Projects



- **[Beam (beta9)](https://github.com/beam-cloud/beta9)**  

  **The open-source Modal alternative** for serverless GPU compute. Run inference endpoints, background jobs, and sandboxes with a Python/TypeScript decorator—no YAML, no configuration. **Key differentiator**: fully open-source and self-hostable, addressing the vendor lock-in concern with Modal. Production users include Coca-Cola, Magellan AI, and Stratum. Features: fast image builds, GPU support, memory/filesystem snapshotting, GPU checkpoint restore, long sessions (24h+), and gVisor-based isolation. Best for teams that want Modal-like serverless GPU experience on their own infrastructure or with a managed Beam Cloud option.



- **[RunPod Python SDK](https://github.com/runpod/runpod-python)**  

  Official Python SDK for RunPod's serverless GPU platform. Deploy serverless endpoints, manage GPU pods, and integrate RunPod into CI/CD pipelines programmatically. The platform itself is proprietary, but the SDK is open-source and provides a path to scripted, reproducible serverless deployments. Best for teams already using or evaluating RunPod that want infrastructure-as-code control.



- **[NVIDIA Triton Inference Server](https://github.com/triton-inference-server/server)**  

  Open-source inference serving software that standardizes model deployment across frameworks (TensorFlow, PyTorch, ONNX, TensorRT). Supports GPU and CPU, dynamic batching, model ensembles, and HTTP/gRPC APIs. **Not a GPU cloud**—it's the serving layer you run on your own GPU instances or within managed platforms. Many managed inference services are built on Triton underneath. Best for teams building their own inference infrastructure on rented GPU nodes.



- **[NVIDIA TensorRT](https://github.com/NVIDIA/TensorRT)**  

  High-performance deep learning inference optimizer and runtime. Compiles trained models into optimized engines for NVIDIA GPUs, delivering significant latency and throughput improvements. Best for production inference where every millisecond matters, typically paired with Triton.



### Additional Strong Open-Source Options



- **vLLM** — High-throughput LLM serving engine with PagedAttention. Run on rented GPU nodes to serve models with efficient memory utilization.

- **KServe** — Kubernetes-native model serving platform with autoscaling (including scale-to-zero). Run on any Kubernetes cluster with GPU nodes.

- **Frameworks for building custom systems**: Use **Beam** for self-hosted serverless GPU compute with Modal-like DX. Pair **Triton** or **vLLM** as the serving engine on rented GPU nodes from **Lambda**, **Nebius**, or **Crusoe**. Use **RunPod SDK** if you want managed serverless with programmatic control. For cost optimization across providers, use **Prime Intellect's** marketplace to compare live rates before committing.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- GPU pricing changes frequently; all rates cited are from published sources at the time of writing and should be verified before budgeting. Reserved/negotiated rates are typically not published.

- **CoreWeave's minimum provisioning unit is 8 GPUs** for Hopper/Blackwell HGX instances—factor this into cost comparisons against providers that allow single-GPU rental .

- **Nebius raised H100 and H200 prices effective October 1, 2026**—verify current rates before budgeting .

- Self-hosted serverless platforms like **Beam** shift operational responsibility to you—plan for Kubernetes cluster management, GPU driver maintenance, and storage provisioning.



---



**Made for ML engineers, AI infrastructure teams, and developers building on GPU compute without datacenter ownership.**  

Let's make GPU cloud and serverless infrastructure more open, portable, and cost-transparent.
