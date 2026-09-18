@"
# Kubernetes Multi-Cluster Disaster Recovery

Multi-Cluster Kubernetes Disaster Recovery using Velero, Amazon S3,
cross-region EKS recovery, stateful workload restoration, failover,
failback, and measured RTO/RPO.

## Project Objective

Build and demonstrate a Kubernetes disaster recovery solution that
recovers Kubernetes resources and persistent application data after
primary cluster or regional failure.

## Architecture

Primary EKS Cluster
        |
        | Velero Backup
        v
Amazon S3
        |
        | Restore
        v
DR EKS Cluster
        |
        v
Recovered Application

## Project Stages

- [ ] Stage 1 — Cluster Backup with Velero
- [ ] Stage 2 — Same-Cluster Restore
- [ ] Stage 3 — Cross-Region / Second-Cluster Recovery
- [ ] Stage 4 — Failover and Failback Drill
- [ ] Stage 5 — Automation, Monitoring and Report

## Repository Structure

```text
velero/
  install/
  backup/
  schedules/

restore/
  same-cluster/
  cross-region/

drill/
  failover/
  failback/
  rto-rpo/

docs/
  k8s-dr-report.md
  research.md
  runbook.md
  screenshots/