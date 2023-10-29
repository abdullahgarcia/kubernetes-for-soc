# Threat Objects

| ID   | Description                                                                    |
|------|--------------------------------------------------------------------------------|
| TO01 | Cluster's CA x509 cert/key pair.                                               |
| TO02 | kube-apiserver's server x509 cert/key pair.                                    |
| TO03 | kube-apiserver's etcd-and-kubelet client x509 cert/key pairs.                  |
| TO04 | Cluster's service accounts signing x509 cert/key pair.                         |
| TO05 | kubernetes-admin's kubeconfig file: client x509 cert/key pair embedded.        |
| TO06 | kube-scheduler's kubeconfig file: client x509 cert/key pair embedded.          |
| TO07 | kube-controller-manager's kubeconfig file: client x509 cert/key pair embedded. |
| TO08 | kube-apiserver's static pod manifest file.                                     |
| TO09 | kube-controller-manager's static pod manifest file.                            |
| TO10 | kube-scheduler's static pod manifest file.                      |
| TO11 | Cluster's audit log directory.                                  |
| TO12 | Cluster's audit policy file.                                    |
| TO13 | Cluster's encryption provider config file.                      |
| TO14 | x509 certificate for the CA that signed OIDC's web certificate. |
| TO15 | etcd's CA x509 cert/key pair.                                   |
| TO16 | etcd's server x509 cert/key pair.                               |
| TO17 | etcd's data directory.                                          |
| TO18 | Cluster's desired state.                                        |
| TO19 | Master node's etcd's CA x509 cert.                                              |
| TO20 | Master node's kubelet's kubeconfig file: client x509 cert/key pair embedded.    |
| TO21 | Master node's kubelet' service file.                                            |
| TO22 | Master node's kubelet's binary.                                                 |
| TO23 | Master node's kubelet's config file.                                            |
| TO24 | Master node's kubelet's directory.                                              |
| TO25 | Master node's kube-proxy's kubeconfig file: client x509 cert/key pair embedded. |
| TO26 | Master node's kube-proxy' service file.                                         |
| TO27 | Master node's kube-proxy's binary.                                              |
| TO28 | Master node's kube-proxy's config file.                                         |
| TO29 | Master node's CNI directories.                                                  |
| TO30 | Worker node's kubelet's kubeconfig file: client x509 cert/key pair embedded.    |
| TO31 | Worker node's kubelet' service file.                                            |
| TO32 | Worker node's kubelet's binary.                                                 |
| TO33 | Worker node's kubelet's config file.                                            |
| TO34 | Worker node's kubelet's directory.                                              |
| TO35 | Worker node's cluster's CA x509 cert.                                           |
| TO36 | Worker node's kube-proxy's kubeconfig file: client x509 cert/key pair embedded. |
| TO37 | Worker node's kube-proxy' service file.      |
| TO38 | Worker node's kube-proxy's binary.           |
| TO39 | Worker node's kube-proxy' config file.       |
| TO40 | Worker node's CNI directories.               |
| TO41 | Cluster's admission control config file.     |
| TO42 | Cluster's authorization webhook config file. |
