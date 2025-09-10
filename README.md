## The Twelve Trials: A Cloud-Native Challenge

This project is a comprehensive, self-guided challenge to build and deploy a full-stack, cloud-native application entirely in an offline, local environment. It's designed to test and solidify skills across the entire DevOps lifecycle, from infrastructure provisioning to application deployment and observability. The entire system must function without an internet connection, relying on local resources and registries.

### Core Technologies

* **Infrastructure as Code:** Terraform & Ansible (with idempotency)
* **Containerization:** Docker
* **Orchestration:** Kubernetes (K3s) with native manifests (Deployments, Services, ConfigMaps, Secrets, Ingress)
* **Version Control & CI/CD:** Gitea & Gitea Actions/ArgoCD for GitOps
* **Service Mesh:** Linkerd (for observability and mTLS)
* **Authentication:** Keycloak (for JWT-based authentication)
* **Application:** A Rust-based API
* **Database:** CloudNativePG (CNPG)
* **Documentation:** Mermaid diagrams (for architecture, pipeline, and auth flow)

### Project Deliverables

* **Fully Functional System:** The entire application stack must run and be accessible offline.
* **Idempotent Infrastructure:** All provisioning and configuration scripts must be repeatable without causing errors or unexpected changes.
* **Operational GitOps Pipeline:** A working CI/CD pipeline that automatically syncs code changes from a Git repository to the Kubernetes cluster.
* **Secure & Observable Mesh:** Linkerd must be correctly implemented to provide mTLS and visual observability of service traffic.
* **Complete Documentation:** A `README.md` file containing detailed instructions, architectural diagrams, and a clear explanation of how the system works.
