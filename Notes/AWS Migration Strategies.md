# AWS Migration Strategies — The 7️⃣ Rs (Cheat Sheet) ☁️🚀

> A **migration strategy** is the approach used to move a workload to AWS. AWS groups common approaches into **seven strategies**—the **7 Rs**. Choosing the right one depends on **business value, risk, time, dependencies, and skills**.

---

## TL;DR 🧭
- For **large migrations**, favor **Rehost**, **Replatform**, **Relocate**, and **Retire** for speed and scale. ⏩
- **Refactor/Re-architect** is powerful but **not ideal to do during a big wave**—migrate first, modernize later. 🛠️➡️🌐

---

---

## At-a-Glance Matrix 📊

| Strategy | Nickname | App Changes | Speed to Cloud | Cost-Effect Potential | When It Shines |
|---|---|---:|:---:|:---:|---|
| 📴 **Retire** | Decommission | None | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | No value, obsolete, zombie/idle apps |
| 📌 **Retain** | Keep-as-is | None | — | — | Compliance, high risk, dependencies, recent upgrades |
| 🏗️ **Rehost** | Lift & Shift | Minimal/None | ⭐⭐⭐⭐ | ⭐⭐ | Fast scale-out, broad estate moves |
| 🔁 **Relocate** | Move platform-in-place | None | ⭐⭐⭐⭐⭐ | ⭐⭐ | Move en masse within same tech family/VPC/Account |
| 🛒 **Repurchase** | Drop & Shop (SaaS) | Replace app | ⭐⭐⭐ | ⭐⭐⭐⭐ | Swap to SaaS/modern license |
| 🔧 **Replatform** | Lift, Tinker & Shift | Low–Medium | ⭐⭐⭐ | ⭐⭐⭐ | Managed/serverless DBs, containers, OS/CPU savings |
| 🧬 **Refactor / Re-architect** | Cloud-native redesign | High | ⭐ | ⭐⭐⭐⭐⭐ | Agility, scale, microservices, deep modernization |

> ⭐ speed: more stars = faster migration; ⭐ cost-effect: more stars = greater long-term savings potential.

---

## Strategy Details (with common triggers & tips) 🧩

### 📴 Retire
- **What:** Decommission/archival; shut down the stack.
- **Use when:** No business value, security risk (EOL OS), or persistently **zombie (<5% CPU/RAM)** or **idle (5–20%)** apps; no inbound traffic in last 90 days.
- **Outcome:** Cuts hosting/licensing/security surface.

👉 Best practice: Assess with discovery/utilization data to target “quick wins.”

---

### 📌 Retain
- **What:** Keep in source environment (for now).
- **Use when:** Data residency/compliance, high migration risk, **upstream dependencies**, **recent refresh**, **low business value**, waiting for **vendor SaaS**, **specialized hardware/mainframe** (AS/400, Solaris), or even purposely keeping zombie/idle on-prem for now.
- **Outcome:** Defers migration until constraints clear.

---

### 🏗️ Rehost (Lift & Shift)
- **What:** Move as-is to AWS **without code changes**.
- **Use when:** Need speed, broad estate moves across physical/virtual/other cloud; minimize downtime (cutover-dependent).
- **Why:** Easier to **optimize once in AWS** (integrate native services later).
- **Helpful tools:** [AWS Application Migration Service](https://aws.amazon.com/application-migration-service/when-to-choose-aws-mgn/), [Migration Factory](https://aws.amazon.com/solutions/implementations/aws-cloudendure-migration-factory-solution/), [VM Import/Export](https://aws.amazon.com/ec2/vm-import/).

---

### 🔁 Relocate
- **What:** **Bulk move** servers/apps to a **cloud version of same platform**, or shift across **VPC/Region/Account** (e.g., RDS to another VPC).
- **Use when:** You want the **fastest path** with **no architecture change** and minimal disruption.
- **Outcome:** Quickest operational move; preserves existing platform model.

---

### 🛒 Repurchase (Drop & Shop)
- **What:** Replace with a **SaaS/cloud product** that delivers more value (anywhere access, no infra, pay-as-you-go).
- **Use when:** Upgrading version, switching to third-party equivalent, replacing custom builds to avoid recode.
- **Checklist after buy:** 🤝 Train users • 🗃️ Migrate data • 🔐 Integrate auth (e.g., AD) • 🌐 Configure secure networking.
- **Caveat:** Validate **security & compliance** before purchase.

---

### 🔧 Replatform (Lift, Tinker & Shift)
- **What:** Move with **select optimizations** to cut cost or leverage managed/serverless.
- **Common moves:** 
  - SQL Server ➜ **Amazon RDS for SQL Server**  
  - Windows ➜ **Linux** (port .NET Framework ➜ **.NET Core** via [Porting Assistant](https://aws.amazon.com/porting-assistant-dotnet/))
  - x86 ➜ **AWS Graviton** for cost/perf  
  - VMs ➜ **Containers** (no code changes) using [AWS App2Container](https://aws.amazon.com/app2container/)
- **Why:** Reduce ops toil/licensing, improve security, boost performance.

---

### 🧬 Refactor / Re-architect
- **What:** Redesign for **cloud-native** (microservices, event-driven, serverless) to maximize agility, performance, and cost efficiency.
- **Use when:** Monolith blocks delivery, legacy mainframe costs soar, code is unmaintainable/untestable, or **partial data must remain on-prem** (segregate sensitive tables).
- **Note for large programs:** High complexity—**migrate first, modernize after** to avoid program risk.

---

## Choosing the Right R (Quick Heuristics) 🧠✅

- **Need speed/low change?** ➜ **Rehost** or **Relocate**  
- **Want some easy wins?** ➜ **Replatform** (managed DBs, containers, Graviton, OS shift)  
- **App is obsolete?** ➜ **Retire**  
- **Vendor has a great SaaS?** ➜ **Repurchase**  
- **Constraints today (compliance/deps)?** ➜ **Retain** (plan revisit date)  
- **Strategic modernization?** ➜ **Refactor** (often **post-migration**)

---

## Large Migration Guidance 🏁
- **Wave 1–N:** Prioritize **Rehost / Relocate / Replatform / Retire** for coverage and speed.  
- **Post-Cutover:** Targeted **Refactor** tracks for high-ROI candidates.

---

## Handy Links 🔗
- 7 Rs overview: Retire · [Retain](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#retain) · [Rehost](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#rehost) · [Relocate](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#relocate) · [Repurchase](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#repurchase) · [Replatform](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#replatform) · [Refactor](https://docs.aws.amazon.com/prescriptive-guidance/latest/large-migration-guide/migration-strategies.html#refactor)  
- Retire best practices: [Assessing applications to retire](https://docs.aws.amazon.com/prescriptive-guidance/latest/migration-retiring-applications/)  
- Pattern catalogs: [Rehost](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migration-rehost-pattern-list.html) · [Relocate](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migration-relocate-pattern-list.html) · [Replatform](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migration-replatform-pattern-list.html) · [Re-architect](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migration-rearchitect-pattern-list.html)

---

## One-Page Decision Checklist 🧾✨
- [ ] Business value clear (retain/retire candidates identified)  
- [ ] Compliance/data residency assessed (retain/segment?)  
- [ ] Dependencies mapped (order of moves known)  
- [ ] Downtime tolerance & cutover method defined  
- [ ] Target ops model chosen (managed/serverless/containers)  
- [ ] Cost levers considered (SaaS, Graviton, OS/license)  
- [ ] Modernization **now** (small) vs **later** (big refactor) decided

> 🎯 **Rule of thumb:** *Move fast to AWS with minimal risk, then iterate toward cloud-native excellence.*
