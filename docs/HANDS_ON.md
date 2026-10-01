# Hands-on path after the guided UI

Start with the UI at Level 0. Explain each concept before using a command. Choose Practice lab, run a plan, inspect the exported evidence, and try the changed scenario. The assessment checks both scenarios and five questions.

## Python protocol examples

Activate `.venv`, then:

```bash
python -m academy.server --mode gpu --port 8633 --scenario thermal
# Optional, on an existing compatible NVIDIA machine:
python -m scripts.live_gpu
```

A transparent capacity calculator shows every memory assumption. Synthetic telemetry replays demonstrate memory pressure, heat and falling clock speed, input starvation, and error codes. A bounded whole-GPU scheduler checks Pod resource declarations. The optional nvidia-smi script only reads existing compatible hardware.

## Complete local stack

Run `docker compose up --build -d`, then from the activated environment run:

```bash
python -m scripts.verify_stack
```

This verifies the HTTP training target and a successful Prometheus scrape. Container CI runs the same verifier with internal service URLs. Inspect `compose.yaml` for exact ports and configuration.

The HTTP training target is at http://127.0.0.1:8633; inspect `/health` and `/metrics`. Prometheus is at http://127.0.0.1:9093. Query `up{job="training"}` and preserve metric meanings and units. The GPU exporter exposes a final synthetic sample; application-rate benchmarking needs a changing real workload.



## Take the next step with evidence

Run a supported workload on a real GPU. Confirm the kernel execution path and output, measure actual memory and latency, inspect supported DCGM fields and collection health, and try a real device-plugin-backed Kubernetes workload. Validate distributed partitions, interconnects, and framework behavior before making placement or performance claims.

Default labs do not execute CUDA kernels, DCGM diagnostics, native collectives, or Kubernetes scheduling. Arithmetic estimates are not universal memory formulas or OOM guarantees. Telemetry is synthetic; the HTTP exporter exposes the final replay sample, so it is suitable for scrape and semantic exercises, not a live workload rate benchmark. The Pod example declares resources but does not run a GPU kernel. MIG and sharing are taught rather than provisioned.

Keep a record of what you directly observed, what the teaching model assumed, and what remains unknown. A troubleshooting conclusion should follow the same device or request through time and verify the relevant outcome.
