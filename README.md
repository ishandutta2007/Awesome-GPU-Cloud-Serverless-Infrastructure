# Awesome-GPU-Cloud-Serverless-Infrastructure

# Top GPU Cloud & Serverless Infrastructure Ecosystem

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
  NVIDIA-only GPU cloud built for large-scale training and inference. **Pricing structure**: on-demand, spot (up to 60% off with interruption risk), and reserved multi-year contracts (negotiated, up to 60% discount). **Critical caveat**: Hopper and Blackwell HGX instances rent **eight GPUs at a time**—you cannot provision a single H100 on-demand. Only GH200 rents as a single chip at **$6.50/hour**. An 8x H100 node costs **$49.24/hour** ($35,945/month if running continuously); 8x B200 is **$50,224/month** on-demand . Best for teams that can commit to full-node workloads and negotiate reserved capacity.

- **[Lambda](https://lambda.ai/)**  
  AI cloud with first-party datacenters and consistent instance behavior. **On-demand pricing** (per GPU-hour, self-serve): 1x H100 SXM **$4.29**, 8x H100 SXM **$3.99**, 8x A100 80GB **$2.79** . **1-Click Clusters** for multi-node training with InfiniBand (2 weeks to 1 year commitments) are the differentiated product for large training runs. **No serverless tier**—Lambda is bare-metal or cluster rental only. Best for teams that want hardware consistency and a straightforward pricing page without broker intermediation.

- **[Crusoe Cloud](https://www.crusoe.ai/cloud/pricing)**  
  GPU cloud with spot, on-demand, and reserved options. Positions itself on avoiding GPU lock-in with tailored agreements. Offers managed inference and serverless fine-tuning alongside raw GPU instances. CPU instances start at **$0.04/vCPU-hour** . Best for teams that want flexible contract terms and a mix of raw compute and managed AI services.

- **[RunPod](https://www.runpod.io/)**  
  GPU cloud specializing in **serverless GPU inference** and pod-based development. The **`runpod-python` SDK** allows programmatic deployment of serverless endpoints and GPU pods. Pricing varies by GPU type and serverless vs. pod mode. Best for developers who want a managed serverless GPU experience with an SDK-first workflow.

- **[Together AI](https://www.together.ai/)**  
  AI platform offering **three distinct tiers**: serverless (per-token), dedicated endpoints (per-minute per replica), and raw GPU clusters. **Dedicated endpoint pricing**: H100 **$5.49/hour**, B200 **$8.99/hour** . **GPU cluster pricing** (raw compute, you run the stack): H100 **$3.99** on-demand / **$3.09** reserved (181+ days); H200 **$5.99** / **$3.99**; B200 **$8.19** / **$6.79** . Best for teams that want to start serverless and graduate to dedicated or cluster as volume grows.

- **[Nebius AI](https://nebius.com/)**  
  European-headquartered GPU cloud with transparent published pricing. **H100 NVLink**: **$4.50/hour** (from Oct 2026); **H200**: **$5.40/hour**; **B200**: **$8.50/hour**. Preemptible options start from **$0.79/hour** for H100 and **$0.99/hour** for B200 . Best for teams that want published, predictable rates without sales negotiations.

- **[FluidStack](https://www.fluidstack.io/)**  
  Budget-friendly GPU cloud with 10 configurations. **Entry-level**: RTX 4090 at **$0.50/hour**, A6000 at **$0.70/hour**, A100 40GB at **$0.95/hour**. H100 SXM on-demand at **$2.50/hour** (reserved at **$1.80/hour**) . **Free egress** and 99.9% SLA. Best for cost-sensitive inference workloads where H100 performance is not strictly necessary.

- **[Voltage Park](https://voltagepark.com/)**  
  GPU cloud with published FAQ pricing: **H100 starting at $1.99/hour** without a contract . On-demand, InfiniBand, and long-term reserve tiers are quote-based for larger volumes. Best for teams that want low-cost H100 access without commitment.

- **[Scaleway](https://www.scaleway.com/)**  
  European cloud provider with GPU instances (H100, L40S) available through Kubernetes node pools. Data residency in EU. Pricing varies by instance type; less transparent than dedicated GPU clouds. Best for European teams requiring GDPR-aligned data residency.

- **[Prime Intellect](https://app.primeintellect.ai/)**  
  GPU marketplace aggregating multiple providers with **real-time pricing**. **H100 at $2.35/hour**, H200 at **$4.05/hour**, B200 at **$7.55/hour** (spot **$2.68**), GH200 at **$1.99/hour**, A100 at **$1.23/hour** (spot **$0.68**) . Best for teams that want to compare live prices across providers and optimize cost per workload.

## Open-Source GitHub Projects

- **[Beam (beta9)](https://github.com/beam-cloud/beta9)**  
  **The open-source Modal alternative** for serverless GPU compute. Run inference endpoints, background jobs, and sandboxes with a Python/TypeScript decorator—no YAML, no configuration. **Key differentiator**: fully open-source and self-hostable, addressing the vendor lock-in concern with Modal. Production users include Coca-Cola, Magellan AI, Shippabo, and Stratum. Features: fast image builds, GPU support, memory/filesystem snapshotting, GPU checkpoint restore (stop/resume sandboxes preserving running processes), long sessions (24h+), and gVisor-based isolation. Custom container runtime and distributed storage layer enable low cold-start for large images. Best for teams that want Modal-like serverless GPU experience on their own infrastructure or with a managed Beam Cloud option.

- **[RunPod Python SDK](https://github.com/runpod/runpod-python)**  
  Official Python SDK for RunPod's serverless GPU platform. Deploy serverless endpoints, manage GPU pods, and integrate RunPod into CI/CD pipelines programmatically. The platform itself is proprietary, but the SDK is open-source and provides a path to scripted, reproducible serverless deployments. Best for teams already using or evaluating RunPod that want infrastructure-as-code control.

- **[NVIDIA Triton Inference Server](https://github.com/triton-inference-server/server)**  
  Open-source inference serving software that standardizes model deployment across frameworks (TensorFlow, PyTorch, ONNX, TensorRT). Supports GPU and CPU, dynamic batching, model ensembles, and HTTP/gRPC APIs. **Not a GPU cloud**—it's the serving layer you run on your own GPU instances or within managed platforms. Many managed inference services are built on Triton underneath. Best for teams building their own inference infrastructure on rented GPU nodes.

- **[NVIDIA TensorRT](https://github.com/NVIDIA/TensorRT)**  
  High-performance deep learning inference optimizer and runtime. Compiles trained models into optimized engines for NVIDIA GPUs, delivering significant latency and throughput improvements. Best for production inference where every millisecond matters, typically paired with Triton.

### Additional Strong Open-Source Options

- **vLLM** — High-throughput LLM serving engine with PagedAttention. Run on rented GPU nodes to serve models with efficient memory utilization.
- **KServe** — Kubernetes-native model serving platform with autoscaling (including scale-to-zero). Run on any Kubernetes cluster with GPU nodes.
- **Frameworks for building custom systems**: Use **Beam** for self-hosted serverless GPU compute with Modal-like DX. Pair **Triton** or **vLLM** as the serving engine on rented GPU nodes from **Lambda** or **Nebius**. Use **RunPod SDK** if you want managed serverless with programmatic control. For cost optimization across providers, use **Prime Intellect's** marketplace to compare live rates before committing.

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
- Self-hosted serverless platforms like **Beam** shift operational responsibility to you—plan for Kubernetes cluster management, GPU driver maintenance, and storage provisioning.

---

**Made for ML engineers, AI infrastructure teams, and developers building on GPU compute without datacenter ownership.**  
Let's make GPU cloud and serverless infrastructure more open, portable, and cost-transparent.
