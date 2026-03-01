# 🗺️ ROADMAP — Security Metrics & KPIs

Este roadmap organiza as entregas do repositório em **milestones** para construir um sistema de métricas de Segurança com foco em **liderança**, **decisão executiva**, **governança de dados** e **priorização por risco**.

📌 Objetivo do repositório:
Fornecer um conjunto de artefatos (KPI/KRI catalog, glossário operacional, templates executivos e dashboards fictícios) para responder:
**o que mudou, por quê, qual o impacto e o que decidir/fazer a seguir**.

---

## ✅ Definição de pronto (Definition of Done)

Uma entrega está “pronta” quando:
- Está em **PT-BR**, clara e aplicável.
- Define **objetivo + quando usar** no topo.
- Inclui **definição operacional** (fórmula, fonte, frequência, owner) quando aplicável.
- Define **threshold/gatilho** (quando escalonar / qual ação esperar) quando aplicável.
- Inclui exemplo fictício (dataset, mockup ou relatório preenchido) quando fizer sentido.
- Está **linkada** no README raiz e no README da pasta correspondente.

---

## 🧱 M0 — Repo Product Ready (higiene + navegação)
**Objetivo:** repo com cara de produto (navegável e rastreável).

### Entregas
- [x] `ROADMAP.md` (este arquivo)
- [x] `CHANGELOG.md`
- [x] `LICENSE`
- [x] `DISCLAIMERS.md`
- [x] README raiz com Quick Start + links válidos
- [ ] Padronizar READMEs por pasta (00–03)

### Pacote de commits sugerido
- `chore: add roadmap, changelog, license and disclaimers`
- `docs: update root README quickstart + repo map`
- `docs: standardize folder readmes`

---

## 🧭 M1 — Executive Pack v2 (decisão-orientada)
**Objetivo:** “o essencial para liderança” (1-pager + relatório mensal).

### Entregas (00-executive-pack/)
- [ ] Revisar:
  - [ ] `security-executive-1pager-template.md` (decisão-orientada)
  - [ ] `monthly-executive-report-template.md` (1–3 páginas, com “decisions needed”)
- [ ] Adicionar:
  - [ ] `executive-pack-how-to.md`
  - [ ] `executive-summary-example-filled.md` (fictício)
  - [ ] `decision-log-template.md`
  - [ ] `status-metrics-weekly-template.md` (opcional)

### Pacote de commits sugerido
- `docs: upgrade executive 1pager and monthly report to decision-driven format`
- `docs: add executive pack how-to + decision log`
- `docs: add filled executive examples (fictional)`

---

## 📚 M2 — KPI/KRI Catalog v2 (por domínio + ownership)
**Objetivo:** catálogo aplicável (owner, cadência, fonte, limiar e ação).

### Entregas (01-kpi-catalog/)
- [ ] Revisar `kpi-catalog.md` (padrão por métrica: definição, fórmula, fonte, frequência, owner, threshold, ação)
- [ ] Adicionar:
  - [ ] `kpi-kri-minimum-set.md`
  - [ ] `kpi-by-domain-grc.md`
  - [ ] `kpi-by-domain-vm.md`
  - [ ] `kpi-by-domain-ir.md`
  - [ ] `data-quality-and-anti-patterns.md`

### Pacote de commits sugerido
- `docs: refactor KPI catalog to include owner, cadence, thresholds`
- `docs: add minimum KPI/KRI set (leadership-ready)`
- `docs: add KPIs by domain (GRC/VM/IR) + anti-patterns`

---

## 📘 M3 — Glossário operacional v2 (definições auditáveis)
**Objetivo:** consistência e replicabilidade (evitar “métrica discutível”).

### Entregas (02-glossary/)
- [ ] Revisar `security-metrics-glossary.md` (padrão operacional)
- [ ] Adicionar:
  - [ ] `metric-definition-template.md`
  - [ ] `metric-source-map.md`
  - [ ] `calculation-examples.md`
  - [ ] `ownership-and-review.md`

### Pacote de commits sugerido
- `docs: upgrade metrics glossary to operational definitions`
- `docs: add metric definition template + source map`
- `docs: add calculation examples + ownership governance`

---

## 🚦 M4 — Thresholds & Triggers (gatilhos executivos)
**Objetivo:** transformar métrica em decisão/ação (escalonamento e prioridades).

### Entregas (criar 04-thresholds/)
- [ ] `04-thresholds/README.md`
- [ ] `kri-thresholds-and-triggers.md`
- [ ] `sla-breach-and-escalation.md`
- [ ] `risk-appetite-alignment.md`
- [ ] `exceptions-and-waivers-metrics.md`

### Pacote de commits sugerido
- `docs: add thresholds & triggers framework (KRI + escalation)`
- `docs: add SLA breach escalation guidance by domain`
- `docs: add risk appetite alignment + waivers/exceptions metrics`

---

## 🧪 M5 — Datasets fictícios v2 (séries temporais)
**Objetivo:** permitir dashboards realistas com tendência/hotspots.

### Entregas (03-dashboards/sample-dataset/)
- [ ] Enriquecer `kpi-sample-data.csv` (time series + thresholds)
- [ ] Adicionar:
  - [ ] `kri-sample-data.csv`
  - [ ] `sla-aging-sample-data.csv`
  - [ ] `risk-register-sample-data.csv`
  - [ ] `ir-sample-data.csv`
  - [ ] `vm-sample-data.csv`
- [ ] `03-dashboards/sample-dataset/README.md` (data dictionary)

### Pacote de commits sugerido
- `data: enrich KPI dataset to support trends and thresholds`
- `data: add sample datasets for GRC/VM/IR + SLA aging`
- `docs: add sample dataset dictionary`

---

## 📊 M6 — Dashboards v2 (mockups + como usar em reunião)
**Objetivo:** virar material de liderança (o que olhar e que decisão tomar).

### Entregas (03-dashboards/dashboard-mockups/)
- [ ] Revisar `dashboard-mockups/README.md`
- [ ] Adicionar:
  - [ ] `executive-dashboard-outline.md`
  - [ ] `dashboard-mockup-executive.png` (print simples)
  - [ ] `dashboard-mockup-domain-vm.png`
  - [ ] `dashboard-mockup-domain-ir.png`
  - [ ] `dashboard-mockup-domain-grc.png`
  - [ ] `how-to-run-metrics-review-meeting.md`
  - [ ] `metrics-review-deck-outline.md`

### Pacote de commits sugerido
- `docs: add executive dashboard outline + how-to meeting guide`
- `docs: add dashboard mockups by domain (executive/VM/IR/GRC)`
- `docs: add metrics review deck outline`

---

## 🗂️ M7 — Case Studies (3 casos “pasta de entrevista”)
**Objetivo:** métricas → decisão → ação → melhora (prova final).

### Entregas (criar 05-case-studies/)
- [ ] `05-case-studies/README.md`
- [ ] `case-01-sla-aging-turnaround/`
- [ ] `case-02-ir-mttd-mttr-improvement/`
- [ ] `case-03-risk-to-investment-prioritization/`

**Formato padrão**
- `contexto.md` • `metricas-e-sinais.md` • `decisoes.md` • `acoes.md` • `resultado.md` • `next-steps.md`

### Pacote de commits sugerido
- `cases: add case studies structure + template`
- `cases: add case 01 (SLA aging turnaround)`
- `cases: add case 02 (IR MTTD/MTTR improvement)`
- `cases: add case 03 (risk-to-investment prioritization)`
