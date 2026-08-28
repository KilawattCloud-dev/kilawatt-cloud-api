⁠# Kilawatt Cloud API (`kilawatt-cloud-api`)

Official API specification, OpenAPI manifests, and integration templates for **Kilawatt Cloud** (`https://api.kilawattcloud.dev`). 

Kilawatt Cloud provides automated, zero-friction, balance-gated GPU orchestration for high-performance AI inference, fine-tuning, and autonomous agent workflows.

---

## ⚡ Quickstart & Authentication

All API requests require a bearer token generated from your Kilawatt Cloud console.

```bash
curl -X POST "https://api.kilawattcloud.dev/v1/clusters/deploy" \

  -H "Authorization: Bearer YOUR_KILAWATT_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "gpu_type": "NVIDIA_B200",
    "gpu_count": 8,
    "max_price_per_hour": 3.00
  }'
