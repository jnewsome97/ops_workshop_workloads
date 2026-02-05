# OpenShift Days: Ops Track Workshop - Workloads Collection

Ansible collection containing custom workloads for the OpenShift Days: Ops Track Workshop.

## Installation

```yaml
requirements_content:
  collections:
  - name: https://github.com/jnewsome97/ops_workshop_workloads.git
    type: git
    version: main
```

## Included Roles

### Workshop Infrastructure
- `ocp4_workload_days_ops_track` - Workshop setup, Showroom configuration, cluster diagnostics
- `studentvm_ocp4` - Student VM configuration

### Custom Days Workloads (with fixes/enhancements)
- `ocp4_days_workload_aws_cli` - Configure AWS CLI in showroom terminal
- `ocp4_days_workload_compliance_operator` - Compliance Operator deployment
- `ocp4_days_workload_metallb` - MetalLB with DNS fixes
- `ocp4_days_workload_ols` - OpenShift Lightspeed
- `ocp4_days_workload_openshift_data_foundation` - ODF with OCP 4.20 fixes
- `ocp4_days_workload_rhacm` - RHACM with alert fixes
- `ocp4_days_workload_rhdh` - Simplified Developer Hub

### Workloads (not in core_workloads)
- `ocp4_workload_oadp` - OADP Backup/DR
- `ocp4_workload_hcp_kubevirt` - Hosted Control Planes on KubeVirt
- `ocp4_workload_rhacm_cloud_credentials` - RHACM cloud credentials
- `ocp4_workload_acm_multicluster_observability` - ACM observability
- `ocp4_workload_kubernetes_image_puller` - Pre-pull container images
- `ocp4_workload_kubevirt` - OpenShift Virtualization

## Usage

Reference workloads using fully-qualified collection name:

```yaml
workloads:
- jnewsome97.ops_workshop_workloads.ocp4_workload_days_ops_track
- jnewsome97.ops_workshop_workloads.studentvm_ocp4
- jnewsome97.ops_workshop_workloads.ocp4_days_workload_aws_cli
```

## License

GPL-2.0-or-later
