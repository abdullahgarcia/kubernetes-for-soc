# Assumptions (AS)

| ID   | Description                                                                                                                                                                                                             |
|------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| AS01 | Fault-tolerance and high availability are not in scope for this model                                                                                                                                                   |
| AS02 | Two certificate authorities (CAs) are in scope for this model: one for the cluster and one for etcd.                                                                                                                    |
| AS03 | Within this model, the kube-proxy is running as a service in the host and using a config file.                                                                                                                          |
| AS04 | Container Runtime installation and related files are out of scope for this model.                                                                                                                                       |
| AS05 | Within this model, there are no business-type K8s workloads scheduled in the master node.                                                                                                                               |
| AS06 | Within this model, K8s admission controllers include: ResourceQuota, LimitRanger, PodSecurity(Policy), and ImagePolicyWebhook.                                                                                          |
| AS07 | Within this model, K8s authorisation is limited to: RBAC, Node, and Webhook.                                                                                                                                            |
| AS08 | Within this model, K8s encryption is implemented via EncryptionConfiguration and applies for data at rest only.                                                                                                         |
| AS09 | Within this model, K8s MutatingAdmissionController enables: disable service account token auto-mount, PodSecurityContext/ContainerSecurityContext, AppArmor, container sandboxing, and application logging consumption. |
| AS10 | Within this model, K8s authentication is limited to: client certificates, service account tokens, and OIDC tokens.                                                                                                      |
| AS11 | AV02, AV03, AV07, AV08, AV09, AV10, AV12, and AV13 are being taken into account under the assumption that the hosts holding the cluster control plane's components are publicly exposing them.                          |
