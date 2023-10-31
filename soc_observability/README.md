# SOC Observability

This document is broken down into premises.

## Technology + Security Practices vs Usage

**1. Comprehending the technology and being well-versed in the associated security best practices, while essential, is not sufficient. It is equally important to possess an understanding of the intended utilization of the technology.**

Think about it, you work for a company that is intending to use a specific technology to support and/or deliver business value.

This means that there are specifics about how the company intends to use such technology.

Let's look at an example: a company has decided to create a Kubernetes-based platform that will deliver clusters which will only support workloads that do not sustain any type of external connectivity.

If you didn't take into account the constrain about external connectivity, you would most likely end up dealing with:

- false positives
- alert fatigue
- lack of proper incident response
- high mean response time
- missing legitimate malicious activity

## SOC In The Room

**2. It is necessary for a representative from the SOC to actively participate and be present during the architectural design phase of the technology utilization.**

It is more often than not, that architects and engineers will be in a room designing how to use a specific technology to support and/or deliver business value. And once things are up and running, they reach out to the SOC hoping for security monitoring and incident response.

Unfortunately, this approach most of the time has an overall adverse effect on the timely delivery of the SOC capabilities.

## Log Sources & Operational Requirements

**3. Comprehend the required sources of logging for the SOC and ascertain the means by which the satisfaction of operational prerequisites can be guaranteed.**

This goes hand in hand with the previous premises.

In the case of Kubernetes, log sources can include:

- application logs
- container logs
- kubelet logs
- control plane component logs: e.g. [kube-apiserver](https://kubernetes.io/docs/tasks/debug/debug-cluster/audit/)
- node logs
- network logs
- third-party plugins/components logs

Understanding which logs will be needed and the level of details for each is as important as understanding where will they be saved, how the SOC will confirm the logs are actually flowing correctly into the SIEM, etc.
