# ☁️ AWS Well-Architected Framework ☁️

A framework providing design principles and best practices to build and operate secure, reliable, efficient, cost-effective, and sustainable systems on AWS.

✅ Developed from AWS Solutions Architects' experience reviewing thousands of customer architectures.

🔄 Promotes a continuous improvement lifecycle through periodic reviews.

## 🤔 Why Use the Framework?

* 🚀 **Build & Deploy Faster**: Reduce unplanned actions, improve capacity management, leverage automation.
* 🛡️ **Lower/Mitigate Risks**: Identify and address architectural risks before they impact business.
* 💡 **Make Informed Decisions**: Understand current architecture to guide future choices and control business outcomes.
* 📚 **Learn Best Practices**: Benefit from AWS's collective experience.

## ⏳History & Evolution

*   **2012:** 🌱 The journey begins.
*   **2015:** 📜 Formal framework published (initially 4 pillars).
*   **2016:** ✨ **Operational Excellence** pillar added.
*   **2018:** 🛠️ **AWS Well-Architected Tool (WAF Tool)** launched in the console.
*   **2019:** 🤝 **Partner Program** established.
*   **2020:** 🔍 **Lenses** & **API Access** introduced for deeper focus.
*   **2021:** 🌍 **Sustainability** pillar added.
*   **2022:** ☁️ **GovCloud** support & **Trusted Advisor** integration launched.
*   **Ongoing:** 🚀 Continuously updated with new features, lenses, and integrations!

## 🧩 Components of the Framework

- 📖 **Content**: Guidelines including Pillars, Design Principles, Best Practices, Questions, and Lenses.
- 🛠️ **Tools**: AWS Well-Architected Tool (in AWS Console) to measure workloads against best practices.
- 📊 **Data**: Information gathered during reviews used for continuous improvement.

## 🏛️ Framework Content Elements: The Pillars

1.  ⚙️ **Operational Excellence** (Added **2016**)
2.  🛡️ **Security**
3.  💯 **Reliability**
4.  ⚡ **Performance Efficiency**
5.  💰 **Cost Optimization**
6.  🌳 **Sustainability** (Added **2021**)

> **🧠 Mnemonic:**
> `Operator Sahab Rokda Pehle Chahiye, Samjhe?`

- **Operational Excellence**: Running and monitoring systems effectively to deliver business value, while continually improving processes and procedures.
- **Security**: Protecting information, systems, and assets by leveraging cloud technologies and robust security best practices.
- **Reliability**: Ensuring a workload performs its intended function correctly and consistently, including the ability to operate and recover from failures.
- **Performance Efficiency**: Using computing resources efficiently to meet requirements, and maintaining that efficiency as demand changes and technologies evolve.
- **Cost Optimization**: Avoiding unnecessary costs and delivering business value at the lowest possible price point through awareness and optimization.
- **Sustainability**: Minimizing the environmental impacts of running cloud workloads by optimizing for energy efficiency and reduced resource utilization.

**Lenses**: Extend guidance for specific industry or technology domains (e.g., Serverless, ML, HPC, SAP, Financial Services). Used with pillars. Custom lenses are possible.

Design Principles:

**General**: Apply across all pillars (e.g., leverage cloud advantages, improve through game days).

**Pillar-Specific**: Apply only to a specific pillar (e.g., Security principle: Prepare for security events via incident management, simulations, automation).

Questions & Best Practices: Each pillar has questions to validate if best practices are implemented. Answers are contextual and require architectural judgment.

Well-Architected Review Process:

- Involves answering foundational questions based on the framework, pillars, and applicable lenses.
- Validates whether specific best practices are in place for a given workload.
- Identifies areas needing improvement.

# AWS Well-Architected Framework Review (WAFR)

A continuous improvement mechanism to consistently evaluate workloads against AWS best practices.

**Purpose**: Identify critical issues, high/medium risks, and areas for improvement.

**Outcome**: A set of actionable steps based on the six pillars to enhance the workload.

It's a conversation (not just formal meetings or an audit), intended to be lightweight (hours) and blame-free.

**Mechanism for Continuous Improvement**: Integrates into the workload lifecycle.

- **Learn** (best practices),
- **Measure** (architecture using Framework/Tool/Lenses),
- **Improve** (address issues).

Key Learning: Review early; neglected decisions are more common than bad ones; address identified risks promptly.

4\. Use Cases:

- **Learn cloud architecture best practices**.
- **Technology governance** (ensure readiness, consistency, prioritization).
- **Portfolio management** (using AWS WA Tool for a central registry, risk visibility, informed investment, documenting decisions).

Three Review Phases:

**1\. Prepare**:

- Define the workload (scope: process, tech, infra, team delivering value).
- Identify core team (SMEs for pillars) & sponsor (owns improvement).
- Hold scoping session (confirm workload, select questions/lenses, define review type/approach).
- Gather relevant data.
- Schedule the review (~3 weeks lead time typical).

**2\. Review**:

Conduct the review session(s) using the AWS WA Tool.

**Best Practices**:

- Moderator manages meeting & scope.
- Dedicated note-taker inputs into the tool (rotate role).
- Only one person updates the WA Tool at a time.
- Use S3 for related documentation/diagrams.
- Publish report (current state, notes, recommended actions, H/M risks).

**3\. Improve**:

Risk Prioritization: Identify most critical risks (likelihood x potential impact) based on business goals (TTM, security, reliability etc.). Risk levels: High & Medium.

**Improvement Workflow**:

- Identify risks/opportunities (from Review).
- Determine & prioritize solutions (impact vs. effort, business perspective).
- Implement prioritized solutions.
- Track progress & monitor results.
- Guidance covers people, process, and technology; requires collaboration.

Dashboard: Shows resources for the selected Region, including available upgrades for workloads using older framework/lens versions.

**Defining a New Workload**:

- **Mandatory**: Unique Name, Description, Review Owner (responsible person), Environment (Prod/Pre-prod), Regions.
- **Optional**: Account IDs (no IAM permissions needed by default), Architecture Diagram URL, Industry Type/Industry.

Note: Regions/Industry used primarily for filtering/sorting. Tool can review on-prem or other cloud environments.

Workload Details Overview:

- Edit/delete workload.
- Shows progress (questions answered/total), identified risks.
- Overall workload notes (track progress, changes).
- Applied Lenses (AWS & Custom).
- Pillar Priority: Default order can be customized to match workload priorities, affecting question order and recommendations.

**Milestones**: Snapshots of the review at a point in time. Used to track progress and generate reports based on past states.

**Sharing**: Workloads can be shared with IAM users, other AWS accounts, or entire AWS Organizations for collaboration (e.g., with SA/Partner). Permissions and status (pending/accepted) are viewable.

Review Content (Per Question):

- Pillar and Question Number.
- Key Concept being addressed.
- Explanation and Best Practice Checkboxes.
- Detail bar with further explanation and helpful resources.

**Custom Lenses**:

- Create your own pillars, questions, answers, resources, improvement plans, and risk rules.
- Define H/M risk conditions and custom guidance.
- Shareable across accounts (via JSON template upload/download). Allows consistent measurement using organization-specific standards.

***

# Operational Excellence Pillar

Focuses on running and monitoring systems to deliver business value effectively and continually improve supporting processes and procedures.

Ensures workloads, processes, and procedures reinforce business value. It's about effective operation, beyond just having a secure, reliable, etc., architecture.

## Design Principles:

- **Perform Operations as Code**: Apply software engineering discipline to infrastructure and operations. Automate procedures, limit human error, ensure consistent responses.
- **Make Frequent, Small, Reversible Changes**: Design for regular component updates in small increments to minimize impact and allow rollback if needed.
- **Refine Operations Procedures Frequently**: Continuously improve procedures as they are used and as workloads evolve. Use game days for validation.
- **Anticipate Failure**: Perform pre-mortems, test failure scenarios, validate response procedures through game days.
- **Learn from All Operational Failures**: Drive improvement through lessons learned from events/failures. Share knowledge across the organization.

## Best Practice Focus Areas:

**1\. Organization**: Understand priorities, structure, and culture to support business outcomes.

- **Priorities**: Evaluate external/internal customer needs, governance, compliance, threat landscape, risks/benefits. Balance trade-offs. Regularly review/update priorities.
- **Culture**: Foster executive sponsorship, team empowerment, clear communication, escalation paths, experimentation, skill growth, diversity of thought, and appropriate resourcing.

**2\. Prepare**: Understand workloads and expected behaviors; design for insight and build supporting procedures.

- **Design Telemetry**: Implement metrics, logs, events, traces (application, workload, user activity, dependency, transaction traceability) for observability.
- **Design for Operations**: Use version control, automate testing/validation, config management, build/deployment systems, patch management. Share standards. Use multiple environments. Make small, reversible changes. Automate integration/deployment.
- **Mitigate Deployment Risks**: Plan for failures (revert/remediate), test changes thoroughly, use limited/parallel deployments, automate testing/rollback.
- **Operational Readiness**: Evaluate readiness (personnel, processes, runbooks, playbooks) via checklists/ORRs. Use pre-mortems. Have support plans.

**3\. Operate**: Achieve business outcomes measured by defined metrics. Understand health to identify and respond to risks.

- **Understand Workload Health**: Define KPIs/metrics, collect/analyze centrally, establish baselines, learn patterns, alert on risks/anomalies, validate effectiveness.
- **Understand Operational Health**: Define KPIs/metrics (e.g., MTTD, MTTR), collect/analyze logs/metrics, establish baselines, learn patterns, alert on risks/anomalies (with runbook/playbook), validate effectiveness.
- **Responding to Events**: Anticipate events (planned/unplanned), use runbooks/playbooks, have defined ownership/escalation, prioritize by impact, perform root cause analysis, communicate during outages (internal/external), automate responses.

**4\. Evolve**: Continuous improvement based on operational lessons learned.

**Learn, Share, Improve**: Dedicate time for analysis/experimentation. Analyze failures for lessons learned. Share across teams. Conduct regular reviews. Perform post-incident analysis. Implement feedback loops. Use knowledge management systems. Perform retrospectives. Document/share lessons. Dedicate resources for continuous improvement.

***

# Security Pillar

Encompasses the ability to protect data, systems, and assets on the cloud by applying best practices to every area of security.

## Security Design Principles:

- **Implement a Strong Identity Foundation**: Use least privilege, separation of duties, centralized identity management, eliminate long-term static credentials.
- **Enable Traceability**: Monitor, alert, audit actions and changes in real-time. Integrate logs/metrics for automated investigation.
- **Apply Security at All Layers**: Use a defense-in-depth approach (edge, VPC, load balancer, instance, OS, application, code).
- **Automate Security Best Practices**: Use automated, code-based security mechanisms for scalability and cost-effectiveness.
- **Protect Data in Transit and at Rest**: Classify data, use encryption, tokenization, access control.
- **Keep People Away from Data**: Use mechanisms/tools to reduce/eliminate direct access or manual processing of sensitive data.
- **Prepare for Security Events**: Have incident management policies/processes, run simulations, use automation for detection/investigation/recovery.

## Best Practice Areas:

**1\. Security Foundations**:

- **Shared Responsibility**: Understand AWS responsibilities ("security of the cloud") vs. customer responsibilities ("security in the cloud", varies by service type).
- **Account Management**: Use separate accounts (e.g., prod/dev/test) as hard boundaries for security/billing/access. Manage centrally. Secure the root user (avoid routine use, no programmatic access).
- **Operating Securely**: Identify control objectives, stay current with threats/recommendations, automate testing/validation, use threat modeling, implement AWS security services.

**2\. Identity and Access Management (IAM)**:

- **Identity Management**: Manage human (admins, devs, users) and machine (apps, tools, instances) identities. Use strong sign-in (MFA, passwords), temporary credentials, secure secrets management, centralized identity providers (for workforce), rotate credentials, use groups/attributes for scale.
- **Permissions Management**: Grant least privilege (specific actions / resources / conditions). Use groups/attributes dynamically. Have emergency access process. Remove unused permissions. Define organizational guardrails. Manage access based on lifecycle. Analyze public/cross-account access. Manage third-party access securely (JIT, least privilege).

**3\. Detection**:

- Identify potential security misconfigurations, threats, or unexpected behavior.
- Best Practices: Configure service/application logging, analyze logs/findings/metrics centrally, automate responses, implement actionable security events (with runbooks/playbooks).

**4\. Infrastructure Protection**:

- Protect systems/services using defense-in-depth against unauthorized access/vulnerabilities.
- **Network Protection**: Use Zero Trust approach. Create network layers, control traffic at all layers, automate protection (threat intel / anomaly detection), implement inspection/filtering.
- **Compute Protection**: Perform vulnerability management (scan / patch), reduce attack surface (harden OS, minimize components), use managed services (RDS, Lambda), automate protection mechanisms, perform actions at a distance (limit interactive access), use code signing.

**5\. Data Protection**:

- **Classification**: Categorize data by criticality/sensitivity to determine protection/retention controls. Automate where possible. Define lifecycle management.
- **Data at Rest**: Implement secure key management (storage, rotation, access control). Enforce encryption. Automate validation/enforcement. Enforce access control (least privilege, prevent public access). Keep people away from data.
- **Data in Transit**: Implement secure key/certificate management. Enforce encryption (especially outside VPC). Automate detection of unintended access (e.g., GuardDuty). Authenticate network communications (TLS, IPsec).

**6\. Incident Response**: Have processes to respond to and mitigate security incidents.

- **Design Goals**: Establish objectives (contain, recover, preserve forensics), document plans, respond in the cloud, preserve evidence centrally, use redeployment for remediation, automate common responses, choose scalable solutions, learn/improve via simulations.
- **Educate**: Equip team with dev skills (automation), AWS security service proficiency, application awareness. Use game days for hands-on learning. Maintain security awareness training.
- **Prepare, Simulate, Iterate**: Pre-provision access/tools. Identify key personnel/resources. Develop plans. Prepare forensics. Automate containment/recovery. Run game days/simulations.

**7\. Application Security**: Reduce likelihood of issues in production workloads.

Best Practices: Train builders on secure development. Automate security testing in lifecycle. Perform regular penetration testing. Perform manual code reviews. Centralize package/dependency management. Deploy programmatically. Assess pipeline security. Embed security ownership in workload teams.

***

# Reliability Pillar

The ability of a workload to perform its required function correctly and consistently for an expected period of time.

Includes the ability to operate and test the workload throughout its lifecycle.

## Reliability Design Principles:

- **Automatically Recover from Failure**: Monitor KPIs (linked to business value), use automation to detect and remediate failures.
- **Test Recovery Procedures**: Actively test failure scenarios and validate recovery procedures using automation (e.g., chaos engineering, game days).
- **Scale Horizontally**: Replace large resources with multiple smaller resources to reduce single point of failure impact; distribute load.
- **Stop Guessing Capacity**: Monitor demand and utilization; automate resource addition/removal to match demand without over/under-provisioning.
- **Manage Change Through Automation**: Implement infrastructure and configuration changes using automation for traceability and consistency.

## Best Practice Areas:

**1\. Foundations**: Prerequisite requirements influencing reliability, often extending beyond a single workload.

- **Manage Service Quotas/Constraints**: Understand, monitor, and manage service limits (quotas) and physical constraints. Automate quota increases. Ensure sufficient quotas for failover.
- **Plan Network Topology**: Design for high availability across multiple environments (cloud/on-prem). Use HA endpoints (DNS, CDN, LB), redundant connectivity (DX, VPN), sufficient IP allocation (non-overlapping). Consider hub-and-spoke.

**2\. Workload Architecture**: Upfront design decisions for software and infrastructure.

- **Design Service Architecture**: Use Service-Oriented Architecture (SOA) or microservices. Segment workload based on resilience needs. Build services focused on specific domains. Provide clear API service contracts (versioning, rate limits, performance).
- **Design Distributed Systems (Prevent Failures)**: Identify system type (hard/soft real-time, offline). Implement loose coupling (queues, streams, LB). Perform constant work (avoid large load changes). Make responses idempotent.
- **Design Distributed Systems (Mitigate/Withstand Failures)**: Implement graceful degradation (soft dependencies). Use throttling. Control/limit retries (exponential backoff, jitter, fail fast, limit queues). Set appropriate client timeouts. Make services stateless. Implement emergency levers.

**3\. Change Management**: Anticipating and accommodating changes reliably.

- **Monitor Workload Resources**: Use logs/metrics (CloudWatch, 3rd party) for health insight. Monitor all components and AWS Health Dashboard. Define metrics, automate responses/alarming, conduct regular reviews. Monitor end-to-end tracing (X-Ray).
- **Design for Changes in Demand**: Use automation for elasticity (scaling resources automatically). Scale reactively (on impairment) and proactively (based on demand). Use load testing.
- **Implement Change**: Use runbooks for standard activities. Integrate functional and resiliency testing (chaos engineering) into deployment pipelines. Deploy using immutable infrastructure.

**4\. Failure Management**: Implementing resiliency to withstand and recover from failures. (Prerequisite: Trained personnel aware of reliability goals).

- **Back Up Data**: Identify critical data, define RTO/RPO. Automate backups (schedule/trigger). Secure and encrypt backups. Perform periodic recovery tests.
- **Use Fault Isolation**: Deploy across multiple locations (AZs, Regions). Use bulkhead architectures (limit blast radius, e.g., cells, partitions). Automate recovery for single-location components.
- **Withstand Component Failures**: Monitor all components. Fail over to healthy resources. Automate healing (statelessness helps). Rely on data plane during recovery (not control plane). Use static stability (pre-provision capacity for AZ failure). Send notifications on impact. Architect to meet SLAs.
- **Test Reliability**: Use playbooks for failure investigation. Perform post-incident analysis. Test functional, scaling, performance requirements. Use chaos engineering regularly. Conduct game days.
- **Plan for Disaster Recovery (DR)**: Set RTO/RPO based on business needs. Define DR strategy (backup/restore, active-passive, active-active). Test failover regularly. Manage configuration drift at DR site. Automate recovery and traffic routing.

***

# Performance Efficiency Pillar

Focuses on using computing resources efficiently to meet requirements and maintaining efficiency as demand changes and technologies evolve.

## Performance Efficiency Design Principles:

- **Democratize Advanced Technologies**: Consume complex technologies (ML, NoSQL) as services instead of building/managing them, freeing teams to focus on product development.
- **Go Global in Minutes**: Deploy workloads in multiple AWS Regions to reduce latency and improve user experience globally.
- **Use Serverless Architectures**: Remove operational burden of managing servers by using serverless compute, storage, and event services.
- **Experiment More Often**: Leverage cloud resources to quickly test different configurations, instance sizes, storage types, or services.
- **Mechanical Sympathy**: Understand how cloud services are consumed and align technology choices with workload goals and data access patterns.

## Best Practice Areas:

1\. Selection: Choosing the right resource types, sizes, and configurations.

- **Performance Architecture**: Use a data-driven approach. Understand available services/options. Define a process (use cases, docs, benchmarks) factoring in cost. Use managed services where possible. Leverage policies/reference architectures. Benchmark existing workloads. Load test new architectures.
- **Compute Architecture**: Evaluate instance, container, function options. Understand configuration options (family, size, GPU, I/O). Collect metrics for rightsizing. Match resource profile (memory/compute intensive) to workload. Use elasticity. Evaluate continually.
- **Storage Architecture**: Understand storage characteristics (shared access, size, IOPS, latency, patterns, persistence). Evaluate block, file, object, instance storage. Evaluate config options (PIOPS, SSD, magnetic, archival). Choose based on access patterns/metrics (object often more efficient than block).
- **Database Architecture**: Understand requirements (availability, consistency, latency, durability, scale, query needs). Choose solutions matching data characteristics/access patterns. Evaluate options (parameter groups, storage, memory, compute, replicas, caching). Load test. Collect metrics. Optimize storage based on access patterns/metrics (indexing, caching).
- **Network Architecture**: Understand impact of network decisions (latency, bandwidth, protocols, location, jitter). Evaluate cloud networking features. Choose appropriate connectivity (dedicated, VPN). Use load balancing/encryption offloading. Choose optimal protocols (TCP tuning, UDP, SRD). Choose location based on network needs. Optimize configuration based on metrics.

**2\. Review**: Evaluating and evolving workloads for performance.

Evolve Workload: Continually review and adopt new services, patterns, and features that improve performance or efficiency. Define a process for evaluation (testing, analysis). Actively drive adoption based on evaluation.

**3\. Monitoring**: Measuring and alerting on performance.

Monitor Resources: Use monitoring/observability services to record performance metrics (DB transactions, latency, throughput). Analyze metrics via dashboards/reports. Establish KPIs. Set alarms for deviations. Review metrics regularly. Monitor and alarm proactively. Escalate if automation fails.

**4\. Trade-offs**: Making conscious decisions to improve performance by potentially sacrificing other attributes.

Using Trade-offs: Identify where performance increases yield benefits (efficiency, UX). Understand patterns/services that improve performance (e.g., edge caching). Identify what can be traded (consistency, durability, space for time/latency). Evaluate impact of trade-offs (e.g., eventual consistency impact on users). Measure impact of improvements. Use strategies like caching, read replicas, sharding, compression, buffering/streaming.

***

# Cost Optimization Pillar

Focuses on avoiding unnecessary costs and achieving the lowest possible price while still meeting reliability, availability, and performance requirements.

Involves trade-offs (e.g., speed to market vs. cost) and requires ongoing effort (Cloud Financial Management - CFM). Aims to maximize the economic benefits of the cloud.

## Cost Optimization Design Principles:

- **Practice Cloud Financial Management (CFM)**: Dedicate time/resources to build capability in technology/usage management. Grow capability through knowledge, programs, processes.
- **Adopt a Consumption Model**: Pay only for resources consumed; increase/decrease usage based on business needs (e.g., stop dev/test environments).
- **Measure Overall Efficiency**: Monitor business output vs. delivery costs to understand gains from changes.
- **Stop Spending on Undifferentiated Heavy Lifting**: Let AWS handle data center operations, OS/app management (via managed services) to focus on business value.
- **Analyze and Attribute Expenditure**: Use cloud tools to track cost/usage and attribute IT costs to revenue streams/workload owners for ROI measurement and optimization opportunities.

## Best Practice Areas:

**1\. Practice Cloud Financial Management (CFM)**:

- Establish a cross-functional cost optimization team (Finance, Tech, Business - e.g., CCoE).
- Establish partnership between Finance & Tech.
- Set cloud budgets/forecasts (dynamic processes).
- Implement cost awareness in processes & training.
- Report/notify on costs (e.g., AWS Budgets). Hold regular reviews.
- Monitor proactively (tooling/dashboards). Keep up-to-date on services/features.
- Foster a cost-aware culture.
- Quantify the business value of cost optimization.

**2\. Expenditure and Usage Awareness:**

- **Governance**: Establish cost policies, goals, and targets. Map account structure to organization for allocation. Use roles/groups/IAM for cost control. Track project lifecycles.
- **Monitor Cost/Usage**: Configure information sources (CUR, Cost Explorer). Use tagging for filtering/allocation. Identify cost attribution categories. Establish business metrics. Use cost management tools. Allocate costs to measure efficiency (e.g., using Athena on CUR).
- **Decommission Resources**: Track resource lifecycles. Implement decommissioning process (manual/automated). Enforce data retention policies. Delete unused/orphaned resources.

**3\. Cost-Effective Resources:**

- **Evaluate Service Cost**: Define balance between cost and other pillars. Analyze all components. Calculate TCO (incl. ops/mgmt). Select cost-effective software/licensing (open-source preferred, outcome-based licenses). Perform cost analysis over time.
- **Select Resource Type/Size/Number**: Perform cost modeling. Select based on workload data/characteristics (benchmarking). Select automatically based on metrics (rightsizing, feedback loops).
- **Select Pricing Model**: Analyze components for commitment discounts (Savings Plans, RIs) vs. dynamic (Spot, On-Demand). Use cost management tool recommendations. Factor in Region costs. Use cost-efficient third-party agreements. Perform analysis at management account level.
- **Plan Data Transfer**: Monitor charges. Model requirements. Select components/services to optimize/reduce costs (WAN optimization, CDN, caching, Direct Connect).

**4\. Manage Demand and Supply Resources**:

- Analyze workload demand over time (seasonal trends, lifetime).
- Implement buffers or throttling to smooth peaks.
- Supply resources dynamically (demand-based/time-based auto scaling) to avoid over/under-provisioning. Balance just-in-time supply with HA/failure needs.

**5\. Optimize Over Time**:

- Establish a workload review process (frequency based on cost/criticality).
- Review/analyze workloads frequently to adopt new services or re-architect.
- Automate operations tasks to reduce manual effort and cost.
- Decommission resources no longer needed.

***

# Sustainability Pillar

Focuses on minimizing the environmental impacts of running cloud workloads, especially energy consumption and efficiency.

Aims to help customers measure architectures against sustainability best practices, identify improvements, and reduce resource usage.

Involves trade-offs and adheres to the shared responsibility model (AWS: sustainable infrastructure; Customer: sustainable architectures on the cloud).

Driven by customer demand, regulations, employee demand, impact investing, and competitive positioning.

## Sustainability Design Principles:

1. **Understand Your Impact**: Measure workload impact (incl. customer use, decommissioning), establish KPIs (e.g., resources/emissions per unit of work), model future impact, evaluate changes.
2. **Establish Sustainability Goals**: Set long-term goals (e.g., reduce resources per transaction), model ROI, plan for growth with reduced impact intensity.
3. **Maximize Utilization**: Rightsize workloads, implement efficient design to maximize hardware energy efficiency, eliminate idle resources.
4. **Anticipate and Adopt New Offerings**: Monitor and adopt more efficient hardware/software; design for flexibility.
5. **Use Managed Services**: Leverage shared services (e.g., AWS Cloud, Fargate, S3 Lifecycle, Auto Scaling) to maximize resource utilization and benefit from AWS's operational efficiencies.
6. **Reduce Downstream Impact**: Minimize energy/resources required by customers to use your services (e.g., reduce need for device upgrades). Test impact on devices.

## Best Practice Areas:

**1\. Region Selection**: Choose Regions based on business requirements and sustainability goals (considering carbon footprint).

**2\. Alignment to Demand**:

- Scale infrastructure dynamically to match user load precisely (avoid overprovisioning).
- Align SLAs with sustainability goals (minimize resources needed).
- Decommission unused assets.
- Optimize geographic placement to reduce network distance/resources.
- Optimize team resource usage.
- Use buffering/throttling to flatten demand curves.

**3\. Software and Architecture Patterns**:

- Optimize for asynchronous/scheduled jobs (e.g., queue-driven patterns).
- Remove/refactor unused or low-utilization components.
- Optimize code hotspots (time/resource consumption).
- Optimize impact on customer devices.
- Use patterns supporting efficient data access/storage.

**4\. Data Patterns**:

- Implement data classification to use energy-efficient storage tiers appropriately.
- Use lifecycle policies for data deletion to minimize storage.
- Use elasticity/automation for block/file storage growth.
- Remove unneeded/redundant data. Use shared storage to avoid duplication.
- Minimize data movement across networks (use shared file systems/object storage).
- Optimize backups (only required data, exclude ephemeral storage).

**5\. Hardware and Services**:

- Use minimum hardware needed.
- Use instance types with least impact; continually adopt newer, more efficient types.
- Use managed services for operational efficiency.
- Optimize use of hardware accelerators.

**6\. Process and Culture**:

- Adopt efficient development/test/deployment practices (validate improvements, minimize test costs, small improvements).
- Keep workloads updated (efficient features, remove issues).
- Increase utilization of dev/test/build resources.
- Use managed device farms for efficient testing.
