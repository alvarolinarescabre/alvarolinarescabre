<h1 align="center">Hi, I'm Alvaro 👋</h1>

<p align="center">
  <b>Platform / SRE Engineer</b> — Kubernetes, Terraform and Go on AWS.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/TU-USUARIO-LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
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
- 📍 TU-CIUDAD, TU-PAÍS.  <!-- rellena o borra -->

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

### Featured project

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

<!-- Añade aquí 2-3 repos más cuando quieras destacarlos:
**[nombre-repo](https://github.com/alvarolinarescabre/nombre-repo)** — una línea describiéndolo.
-->

---

### GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=alvarolinarescabre&show_icons=true&hide_border=true&theme=default&include_all_commits=true&count_private=true" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=alvarolinarescabre&layout=compact&hide_border=true&theme=default&langs_count=8" alt="Top languages">
</p>
