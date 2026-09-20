<h1 align="center">Hi, I'm Alvaro 👋</h1>

<p align="center">
  <b>Platform / SRE Engineer</b> — Kubernetes, Terraform and Go on AWS.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/alvaro-linares-cabre"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:alvarolinarescabre@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://komarev.com/ghpvc/?username=alvarolinarescabre&style=flat-square&color=blue" alt="Profile views">
</p>

---

### About me

I build and run the infrastructure that applications live on: clusters, pipelines,
observability and the automation that keeps all of it reproducible.

- 🔭 Currently working on **EKS platforms with GitOps** (Argo CD, Karpenter, Gateway API).
- 🌱 Digging into **eBPF-based networking and cost-aware autoscaling**.  <!-- ajusta esto -->
- 💬 Ask me about **Kubernetes, Terraform, AWS or Go**.
- 📍 Madrid, Spain.

---

### Toolbox

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/VictoriaMetrics-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white)

---

### Featured projects

**[go-counter-href-10-sites](https://github.com/alvarolinarescabre/go-counter-href-10-sites)** —
a Go service that fetches HTML pages and counts the words inside absolute `href` links,
shipped with the **whole AWS platform that runs it**: EKS + Terraform, Argo CD GitOps,
Karpenter, Gateway API through an NLB, Helm packaging, HPAs with zero-downtime rollouts,
VictoriaMetrics + Grafana, and an in-cluster k6 load test.

```text
GitHub push → Actions (build → ECR → bump tag) → Argo CD → EKS
                                                    ↓
                              NLB → kgateway (HPA) → counter-api (HPA) → :9090/metrics
```

**[vpn-bgp-multi-cloud](https://github.com/alvarolinarescabre/vpn-bgp-multi-cloud)** —
a step-by-step guide to wiring **AWS, Azure and Google Cloud together over site-to-site VPNs
with dynamic BGP routing**, in a hub-and-spoke topology. It covers non-overlapping RFC 1918
ranges per cloud (AWS `172.31.0.0/16`, GCP `10.0.0.0/8`, Azure `192.168.0.0/24`), a distinct
ASN per provider (65000 / 65001 / 65002), the APIPA link-local addressing each BGP session
needs, and the console walkthrough for every side — Azure Virtual Network Gateways, AWS
Customer/Virtual Private Gateways and Site-to-Site VPN connections, and GCP Cloud Router +
HA VPN — ending with ping tests between instances in the three clouds. Full guide in the
[wiki](https://github.com/alvarolinarescabre/vpn-bgp-multi-cloud/wiki), plus a
[webinar](https://www.youtube.com/watch?v=Hhlqp3n9SMw) walking through it.

```text
Azure (ASN 65002) ──BGP/IPsec──┐
                               ├── AWS (ASN 65000)  ← hub
  GCP (ASN 65001) ──BGP/IPsec──┘
```

**[paradigma_post_peewee](https://github.com/alvarolinarescabre/paradigma_post_peewee)** —
the companion code for my
[Paradigma Digital blog post](https://www.paradigmadigital.com/dev/como-hacer-bases-datos-con-peewee/)
on **PeeWee**, a lightweight Python ORM. A small SQLite-backed example that models an academy
(teachers and classes linked by a foreign key), and walks through the full CRUD surface: table
creation from model classes, single and bulk inserts inside an atomic transaction, updates and
deletes with `where` clauses, and a grouped `select` + `join` across both tables.

---