# Kubernetes Chaos Engineering Lab

Hands-on chaos experiments using **Chaos Mesh** to test resilience of Kubernetes workloads.

## Experiments included

- Pod kill / failure
- Network latency & packet loss
- CPU / Memory stress
- DNS chaos

## Prerequisites

```bash
# Install Chaos Mesh (example)
helm repo add chaos-mesh https://charts.chaos-mesh.org
helm install chaos-mesh chaos-mesh/chaos-mesh -n chaos-mesh --create-namespace
```

## How to run an experiment

```bash
kubectl apply -f experiments/pod-kill.yaml
kubectl apply -f experiments/network-latency.yaml
```

Always run chaos in non-production first and have runbooks ready.

Created for SRE/DevOps portfolio – https://github.com/hkotaga-source
