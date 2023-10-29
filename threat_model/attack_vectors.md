# Attack Vectors (AV)

| ID   | Description                                                                   |
|------|-------------------------------------------------------------------------------|
| AV01 | Publicly exposed host with vulnerable non-K8s endpoint(s)/service(s)/port(s). |
| AV02 | Compromised kubeconfig file.                                                  |
| AV03 | Compromised K8s service account token with cluster details.                   |
| AV04 | Malicious container image in public registry.                                 |
| AV05 | Publicly exposed vulnerable K8s workload: e.g. RCE.                           |
| AV06 | Malicious 3rd party dependency.                                               |
| AV07 | kube-apiserver vulnerability.                                                 |
| AV08 | kube-apiserver's options configured incorrectly.                              |
| AV09 | kube-apiserver's authorization configured incorrectly.                        |
| AV10 | etcd's authentication configured incorrectly.                                 |
| AV11 | Compromised credentials of publicly exposed host.                             |
| AV12 | Container runtime configured incorrectly.                                     |
| AV13 | Compromised OIDC token with cluster details.                                  |
| AV14 | Host with vulnerable non-K8s endpoint(s)/service(s)/port(s).                  |
| AV15 | Legitimately obtained kubeconfig file.                                        |
| AV16 | Legitimately obtained K8s service account token with cluster details.         |
| AV17 | Malicious container image in private registry.                                |
| AV18 | Vulnerable K8s workload: e.g. RCE.                                            |
| AV19 | kubelet vulnerability.                                                        |
| AV20 | kubelet's options configured incorrectly.              |
| AV21 | Compromised credentials of host.                       |
| AV22 | Legitimately obtained OIDC token with cluster details. |
| AV22 | Legitimately obtained credentials of host.             |
