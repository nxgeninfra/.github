<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://computespec.dev/og-image.png">
  <source media="(prefers-color-scheme: light)" srcset="https://computespec.dev/og-image.png">
  <img alt="computespec" src="https://computespec.dev/og-image.png" width="100%">
</picture>

<h1 align="center">One JSON. Any GPU.</h1>

<p align="center">
  <strong>Open specifications for cloud compute resources.</strong><br>
  The vendor-neutral format every comparison tool should speak.
</p>

<p align="center">
  <a href="https://computespec.dev"><img src="https://img.shields.io/badge/Website-computespec.dev-10b981?style=flat-square" alt="Website"></a>
  <a href="https://x.com/nxgeninfra"><img src="https://img.shields.io/badge/Twitter-@nxgeninfra-1DA1F2?style=flat-square&logo=x&logoColor=white" alt="Twitter"></a>
  <a href="https://github.com/nxgeninfra/gis-spec"><img src="https://img.shields.io/badge/Spec-CC_BY_4.0-06b6d4?style=flat-square" alt="License"></a>
  <a href="mailto:hello@computespec.dev"><img src="https://img.shields.io/badge/Contact-hello@computespec.dev-red?style=flat-square" alt="Email"></a>
</p>

---

## The Problem

50+ GPU cloud providers. Zero common format. Every provider names instances differently, prices differently, specs differently. Every comparison tool re-invents normalization from scratch.

## The Solution

**GPU Instance Specification (GIS)** — one JSON document that fully describes any GPU cloud offering from any provider.

```json
{
  "$schema": "https://computespec.dev/gpu/v1/schema.json",
  "provider": "lambda-labs",
  "instance": "gpu_1x_h100_sxm5",
  "gpu": {
    "model": "nvidia-h100",
    "variant": "sxm5",
    "count": 1,
    "vram_gb": 80,
    "tflops_fp16": 989.5,
    "interconnect": "nvlink",
    "architecture": "hopper"
  },
  "pricing": {
    "currency": "USD",
    "billing_unit": "per-hour",
    "on_demand": 2.49
  },
  "normalized": {
    "cost_per_gpu_hour": 2.49,
    "cost_per_tflop_hour": 0.00252,
    "vram_per_dollar": 32.13
  }
}
```

---

## Specifications

| Spec | Description | License | Status |
|------|-------------|---------|--------|
| [**GIS**](https://github.com/nxgeninfra/gis-spec) | GPU Instance Specification | CC BY 4.0 | 🟢 v1.0 Live |
| CIS | CPU Instance Specification | CC BY 4.0 | 📋 Planned (500+ GIS stars) |
| TIS | TPU/ASIC Instance Specification | CC BY 4.0 | 📋 Planned |
| SPS | Spot Pricing Specification | CC BY 4.0 | 📋 Planned |
| SLA-S | SLA Definition Specification | CC BY 4.0 | 📋 Planned |

---

## Repositories

| Repository | Description | License |
|------------|-------------|---------|
| [`gis-spec`](https://github.com/nxgeninfra/gis-spec) | GPU Instance Specification — spec, JSON schema, examples | CC BY 4.0 |

More specs coming as GIS gains adoption. See the [roadmap](https://computespec.dev).

---

## Philosophy

> GPUs are boring when you can describe them in one JSON document.

We don't compete with comparison sites, marketplaces, or price indices. We define the format they could all adopt. The spec is the layer underneath.

---

## Contact

| Channel | Address |
|---------|---------|
| General | [hello@computespec.dev](mailto:hello@computespec.dev) |
| Security | [security@computespec.dev](mailto:security@computespec.dev) |
| Spec feedback | [spec@computespec.dev](mailto:spec@computespec.dev) |
| Support | [support@computespec.dev](mailto:support@computespec.dev) |

---

<p align="center">
  <sub>© 2026 nxgeninfra · <a href="https://computespec.dev">computespec.dev</a> · <a href="https://x.com/nxgeninfra">@nxgeninfra</a></sub>
</p>
