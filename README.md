# secbyte-kubernetes-docker-container-security-hardening-forensics-ctf-labs
A practical collection of cybersecurity CTF labs covering Kubernetes cluster security (RBAC lockdown, control plane architecture, pod security admission, container escape prevention, secret management,Docker container defense (Docker security assessments, runtime hardening, image vulnerability auditing, acontainer forensic investigations).
# Kubernetes Cluster Security, RBAC Lockdown, Docker Container Hardening & Container Forensics CTF Labs

Welcome to the **Kubernetes Cluster Security, RBAC Lockdown, Docker Container Hardening & Container Forensics CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on cloud-native container security, cluster defense, runtime hardening, and containerized forensic triage—spanning **Kubernetes Architecture, Control Plane & Cluster Fundamentals (Cluster architecture, control plane component security, workload isolation baselines)**, **Kubernetes Misconfigurations, Attack Vectors & Cluster Hardening (Cluster misconfiguration exploits, pod security admission, container escape prevention, RBAC lockdown, secret encryption, network policy microsegmentation)**, and **Docker Security Assessments, Container Hardening & Forensics (Docker daemon auditing, capability stripping, container image security, runtime container crime scene forensics)**.

---

## Lab Collection Index

### 1. Kubernetes Architecture, Control Plane & Cluster Security Fundamentals
* **Kubernetes Fundamentals: Cluster Security & Misconfigurations**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-fundamentals-cluster-security-and-misconfiguratio](https://learn.secbyte.org/ctf/kubernetes-fundamentals-cluster-security-and-misconfiguratio)  
  *Focus:* Understanding basic Kubernetes security boundaries, identifying common cluster misconfigurations, auditing unauthenticated API server access, and securing node-to-master communications.

* **Kubernetes Architecture: Cluster Control & Workload Security**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-architecture-cluster-control-and-workload-securit](https://learn.secbyte.org/ctf/kubernetes-architecture-cluster-control-and-workload-securit)  
  *Focus:* Auditing the Kubernetes control plane—securing the API server, etcd datastore, controller manager, and kubelet endpoints; enforcing workload security profiles.

<Image src="image_agent_tag_2415121998592398402" alt="Kubernetes Security Architecture Diagram showing Control Plane and Worker Node components" caption="Kubernetes Control Plane & Worker Node Security Architecture" />

---

### 2. Kubernetes Attacks, Pod Escapes & Cluster Hardening
* **Kubernetes Attack Techniques: From Misconfig to Cluster Compromise**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-attack-techniques-from-misconfig-to-cluster-compr](https://learn.secbyte.org/ctf/kubernetes-attack-techniques-from-misconfig-to-cluster-compr)  
  *Focus:* Exploiting multi-stage Kubernetes attack chains—pivoting through exposed dashboards, leveraging elevated service accounts, and escalating privileges to master nodes.

* **Kubernetes Cluster Hardening: From Misconfigurations to Defense**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-cluster-hardening-from-misconfigurations-to-defen](https://learn.secbyte.org/ctf/kubernetes-cluster-hardening-from-misconfigurations-to-defen)  
  *Focus:* Applying comprehensive cluster security baselines—disabling anonymous authentication, configuring API server admission controllers, and hardening worker nodes.

* **Kubernetes Pod Security: Misconfigurations to Escape Prevention**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-pod-security-misconfigurations-to-escape-preventi](https://learn.secbyte.org/ctf/kubernetes-pod-security-misconfigurations-to-escape-preventi)  
  *Focus:* Preventing container escape vectors—restricting privileged pods (`privileged: true`), blocking host IPC/PID/network namespace sharing, enforcing read-only root file systems, and enforcing Pod Security Standards (Restricted/Baseline).

* **Kubernetes Secrets: From Misconfigurations to Compromise**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-secrets-from-misconfigurations-to-compromise](https://learn.secbyte.org/ctf/kubernetes-secrets-from-misconfigurations-to-compromise)  
  *Focus:* Auditing Kubernetes Secret objects—extracting base64-encoded secrets from unencrypted etcd storage, restricting secret access permissions, and configuring encryption at rest.

* **Kubernetes RBAC Lockdown**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-rbac-lockdown](https://learn.secbyte.org/ctf/kubernetes-rbac-lockdown)  
  *Focus:* Auditing and hardening Role-Based Access Control (RBAC)—identifying wildcard permissions (`*`), eliminating dangerous ClusterRoleBindings, enforcing least privilege for ServiceAccounts, and pruning unused roles.

* **Kubernetes Network Policies: Segmentation Under Pressure**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-network-policies-segmentation-under-pressure](https://learn.secbyte.org/ctf/kubernetes-network-policies-segmentation-under-pressure)  
  *Focus:* Designing zero-trust network microsegmentation—writing CNI NetworkPolicies (`ingress` and `egress` rules), blocking pod-to-pod lateral movement, and enforcing namespace isolation.

### 3. Docker Security Assessments, Runtime Hardening & Forensics
* **Docker Security Fundamentals: Harden, Detect, Respond**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-security-fundamentals-harden-detect-respond](https://learn.secbyte.org/ctf/docker-security-fundamentals-harden-detect-respond)  
  *Focus:* Understanding container isolation mechanics (Linux cgroups, namespaces, seccomp profiles), identifying unsafe Docker defaults, and configuring runtime container monitoring.

* **Docker Security Assessment: From Misconfigurations to Containment**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-security-assessment-from-misconfigurations-to-contain](https://learn.secbyte.org/ctf/docker-security-assessment-from-misconfigurations-to-contain)  
  *Focus:* Auditing Docker host setups—detecting exposed Docker Unix sockets (`/var/run/docker.sock`), analyzing container breakout risks, and auditing container image dependencies.

<Image src="image_agent_tag_2415121998592398511" alt="Docker container architecture diagram showing namespaces, cgroups, and storage drivers" caption="Docker Container Isolation & Runtime Engine Security" />

---

* **Docker Hardening: From Unsafe Defaults to Secure Operations**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-hardening-from-unsafe-defaults-to-secure-operations](https://learn.secbyte.org/ctf/docker-hardening-from-unsafe-defaults-to-secure-operations)  
  *Focus:* Hardening Dockerfiles and runtime containers—dropping unnecessary Linux capabilities (`--cap-drop=ALL`), running non-root user instructions (`USER 10001`), enforcing resource limits, and pinning image digests.

* **Docker Forensics: Container Crime Scene**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-forensics-container-crime-scene](https://learn.secbyte.org/ctf/docker-forensics-container-crime-scene)  
  *Focus:* Executing digital forensics on compromised containers—analyzing overlay filesystem layers, extracting volatile memory artifacts from running containers, parsing container execution logs (`docker logs`), and tracing container escapes.

---

## Learning Path

### Path A: Kubernetes Security Engineer & Cluster Hardening Specialist
1. **Cluster Architecture & Fundamentals:** Start with [Kubernetes Fundamentals](https://learn.secbyte.org/ctf/kubernetes-fundamentals-cluster-security-and-misconfiguratio) and [Kubernetes Architecture](https://learn.secbyte.org/ctf/kubernetes-architecture-cluster-control-and-workload-securit).
2. **Attacks, RBAC & Hardening:** Master defense in [Kubernetes Attack Techniques](https://learn.secbyte.org/ctf/kubernetes-attack-techniques-from-misconfig-to-cluster-compr), [Kubernetes Cluster Hardening](https://learn.secbyte.org/ctf/kubernetes-cluster-hardening-from-misconfigurations-to-defen), [Pod Security](https://learn.secbyte.org/ctf/kubernetes-pod-security-misconfigurations-to-escape-preventi), [Secrets Security](https://learn.secbyte.org/ctf/kubernetes-secrets-from-misconfigurations-to-compromise), [RBAC Lockdown](https://learn.secbyte.org/ctf/kubernetes-rbac-lockdown), and [Network Policies](https://learn.secbyte.org/ctf/kubernetes-network-policies-segmentation-under-pressure).

### Path B: Docker Security & Container Runtime Specialist
1. **Docker Fundamentals & Assessment:** Audit runtime security in [Docker Security Fundamentals](https://learn.secbyte.org/ctf/docker-security-fundamentals-harden-detect-respond) and [Docker Security Assessment](https://learn.secbyte.org/ctf/docker-security-assessment-from-misconfigurations-to-contain).
2. **Dockerfile & Container Hardening:** Apply operational baselines in [Docker Hardening](https://learn.secbyte.org/ctf/docker-hardening-from-unsafe-defaults-to-secure-operations).

### Path C: Cloud-Native Incident Responder & Forensic Examiner
1. **Container Forensics:** Reconstruct breaches in [Docker Forensics: Container Crime Scene](https://learn.secbyte.org/ctf/docker-forensics-container-crime-scene).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, Kubernetes manifests (`.yaml`), Dockerfiles, cluster RBAC configs, or container storage layers.
4. Audit RBAC ClusterRoleBindings, configure API server admission rules, construct network policies, drop Docker capabilities, or analyze volatile memory from compromised containers to capture flags.

---

## Target Audience

* **Cloud Security Engineers & Kubernetes Administrators:** Audit k8s API server settings, enforce RBAC least privilege, configure network policy microsegmentation, and secure etcd.
* **DevSecOps Engineers & Container Security Specialists:** Harden Dockerfiles, drop Linux capabilities, audit container images for CVEs, and enforce Pod Security Standards.
* **Incident Responders & Forensic Examiners:** Perform digital forensics on compromised Docker containers, trace pod escape vectors, and investigate cloud-native breaches.
* **Cybersecurity Students:** Acquire practical hands-on experience in containerization security, Kubernetes cluster administration, and cloud-native defense.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized container breakouts, cluster scanning, or exploitation against external production clusters without explicit permission is strictly prohibited.
