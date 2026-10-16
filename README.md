# Awesome-Bioinformatics-Pipelines

## Top Bioinformatics Pipelines Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Reproducible Genomic Workflows, HPC/Cloud Portability & Community-Curated Standards*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Bioinformatics Pipelines**. These tools enable researchers to assemble, execute, and share reproducible genomic analysis workflows—from quality control and read alignment to variant calling and annotation—across local workstations, HPC clusters, and cloud platforms.



**Examples** include Seven Bridges, DNAnexus, Illumina BaseSpace, Terra.bio, Nextflow Tower, Galaxy Cloud, Cromwell Cloud, Arvados, BC Platforms, and LifeOmic (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, workflow portability, and open scientific pipelines—ideal for bioinformaticians, research institutions, and developers seeking transparent, vendor-independent genomic infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global bioinformatics and cloud genomics market is valued at approximately **$20B–$23.5B in 2025–2026** and projected to exceed **$63B–$118B by the mid-2030s** (~15%–21% CAGR), driven by exponential drops in sequencing costs, clinical multi-omics adoption, and AI-accelerated drug discovery. The sector remains **moderately fragmented**: sequencing hardware and primary upstream data generation are heavily concentrated around dominant players (e.g., Illumina), but downstream secondary workflow orchestration, tertiary analysis, and clinical interpretation remain fragmented across diverse proprietary SaaS suites, academic clouds, and open-source orchestration standards.



## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing | Free Tier Limit | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Illumina BaseSpace](https://www.illumina.com/products/by-type/informatics-products/basespace-sequence-hub.html)** | ~$40B–$41.5B Market Cap / $4.34B–$4.6B Annual Revenue | Starting at $0/mo (Pay-As-You-Go, $1/BIC credit consumption for compute/DRAGEN analysis) | 30-day free trial with 1 TB cloud storage and 100–250 promotional BioInsight credits (BICs) | Illumina's cloud platform for sequencing data analysis, storage, and sharing with native sequencer upload. |
| **[DNAnexus](https://www.dnanexus.com/)** | ~$600M Valuation / ~$80M–$85M Annual Revenue | Starting at $450,000/yr (Base enterprise platform contract list on AWS Marketplace; variable compute units from $50/unit) | Free base account registration; pilot programs (e.g. UK Biobank RAP) include £40 initial credit valid for 90 days (no open compute free tier) | Governed cloud data workspace for omics, phenotypes, multi-language pipelines (CWL, WDL, Nextflow), and clinical analytics. |
| **[Seven Bridges](https://www.sevenbridges.com/)** | ~$130M Standalone Valuation / €27M Annual Revenue (Velsera parent) | Starting at $0 platform fee on NCI Cancer Genomics Cloud (pure pass-through cloud compute/storage rates, e.g. AWS EC2/S3 costs) | $300 free cloud compute and storage credits upon registration via NCI Cancer Genomics Cloud (covers ~40–50 analyses) | CWL-centered commercial & cancer research platform hosting NCI CGC with 850+ curated workflows and multi-cloud execution. |
| **[Nextflow Tower (Seqera Platform)](https://seqera.io/)** | ~$50M–$100M Valuation / ~$9.5M–$18.5M Annual Revenue | Starting at $0/mo (Cloud Basic); Pro/Enterprise starting tiers require custom team quotes | Free forever plan with up to 3 users, 3 concurrent pipeline runs, 250 run histories, 100 datasets, and 100 GB/mo Fusion storage | Official Nextflow management and control plane for collaborative pipeline monitoring, access control, and multi-cloud/HPC execution. |
| **[BC Platforms](https://www.bcplatforms.com/)** | ~$20M+ Growth Funding / ~$25M Annual Revenue | Starting at $48,000/yr (Base 12-month BC Mosaic instance contract on AWS Marketplace) | No perpetual free tier or public self-serve trial (private pilot/demo access provided upon sales qualification) | Genomics data management, biobank governance, and cohort discovery platform for clinical interpretation and precision medicine. |
| **[LifeOmic](https://lifeomic.com/)** | Acquired by Fountain Life / ~$3.5M Annual Revenue | Starting at $17/mo to $40/mo (Consumer/clinician LIFE Ascent tier; enterprise PHC billed by custom storage and compute volume) | Free forever plan for basic consumer health tracking; 7-day free trial for premium clinical mobile apps (enterprise PHC requires custom pilot demo) | Precision health cloud with genomics data management, clinical EHR integration, and longevity diagnostics. |
| **[Terra.bio](https://terra.bio/)** | Non-profit / Consortium-backed (Broad Institute, Microsoft & Verily) | $0 platform fee (100% direct pass-through for Google Cloud or Azure compute, disk, and bucket storage) | $300 in free Google Cloud credits for new users with up to 5 exploratory active workspaces (eligible for NIH STRIDES credits) | Biomedical analysis platform with Jupyter notebooks, WDL/Cromwell execution, and large collaborative cancer/consortia workspaces. |
| **[Galaxy Cloud](https://usegalaxy.org/)** | Academic / Consortia funded (ELIXIR, NIH, NSF) | $0/mo (Open-access community-hosted public cloud servers) | Free forever with 250 GB storage quota per user (expandable to 500 GB for verified ELIXIR researchers; 50 GB per dataset limit) | Accessible web-based GUI workflow system with a massive open tool catalog and zero command-line prerequisite. |
| **[Cromwell Cloud](https://cromwell.readthedocs.io/)** | Open-source foundation (Broad Institute) / Commercial integrations | $0 platform fee (Managed execution via Terra or self-deployed on cloud compute pass-through) | Included within Terra.bio's $300 free trial cloud credit allocation | Broad Institute's WDL execution engine optimized for GATK4 best-practice pipelines and scalable workflow orchestration. |
| **[Arvados](https://arvados.org/)** | Commercialized by Curii Corp / Open-source foundation | Starting at $0 software license (Open-source self-hosted; enterprise managed cluster support via Curii contracts) | Free forever for self-hosted instances (all open-source code under AGPL-3.0); commercial managed clusters require custom evaluation agreement | Open-source biomedical big-data platform running CWL workflows with Git-based tracking and Keep content-addressable storage. |





## Open-Source GitHub Projects



- **[nf-core (tools)](https://github.com/nf-core/tools)**  

  **The companion tool for building Nextflow bioinformatics pipelines** (MIT) . **The community-curated standard for reproducible bioinformatics pipelines**—**nf-core has become the de facto standard for Nextflow pipelines**, with **84+ repositories** covering genomics, transcriptomics, proteomics, metabolomics, and more . **nf-core/tools version 4.0.0** (April 2026) brings **linting improvements**, **strict syntax linting in templates**, **module and subworkflow management enhancements**, **nf-test integration**, and **Nextflow 25.10.4** . **The framework enforces best practices**—modular design, containerized execution, CI testing, and peer review . **The reference implementation for community-curated pipelines** .



- **[Nextflow](https://github.com/nextflow-io/nextflow)**  

  **Dataflow workflow engine for scalable and reproducible science** (Apache-2.0) . **The most widely adopted workflow management system for bioinformatics** alongside Snakemake . **Decouples pipeline logic from execution layer**—the same workflow code runs on laptop, HPC cluster, or cloud by changing configuration profiles rather than modifying workflow logic . **Portable across executors** (Slurm, LSF, SGE, PBS, Kubernetes, AWS Batch, Google Life Sciences) . **The foundation of nf-core and Seqera Platform** .



- **[Snakemake](https://github.com/snakemake/snakemake)**  

  **Rule-based workflow management system** (MIT) . **The original Python-based workflow engine**—alongside Nextflow, accounts for the vast majority of new bioinformatics pipelines . **Python-native syntax** with automatic parallelization, checkpoint/restart, explicit resource declarations, and portability across clusters and cloud . **Supported by WESkit** alongside Nextflow .



- **[WDL / Cromwell](https://github.com/broadinstitute/cromwell)**  

  **Workflow Description Language and Broad's execution engine** (BSD-3-Clause) . **The standard for GATK4-based pipelines** . **Rust WDL parser (stjude-rust-labs/wdl)** was archived December 2025—would need fresh effort for Rust integration . **WDL is mostly used inside Broad/GATK workflows** . **Cromwell Cloud** provides managed execution .



- **[bcbio-nextgen](https://github.com/bcbio/bcbio-nextgen)**  

  **Open, community effort for validated and scalable variant calling, RNA-seq, and small RNA analyses** . **Runs on multiple heterogeneous platforms via CWL**—Curoverse's Arvados, UCSC's Toil, and Seven Bridges' rabix bunny . **WDL conversion provides in-progress support for Broad's Cromwell and DNAnexus APIs** . **The original open-source variant calling pipeline** .



- **[Galaxy Project](https://github.com/galaxyproject/galaxy)**  

  **Web-based GUI workflow platform** (AFL-3) . **The most accessible entry point** for researchers without command-line expertise. **Galaxy Cloud and BRC Analytics** address infrastructure limitations and enhance accessibility . **ToolShed** provides a large catalog of bioinformatics tools. **Don't reimplement Galaxy—provide tool wrappers** .



- **[WESkit](https://gitlab.com/one-touch-pipeline/weskit)**  

  **Implementation of the GA4GH Workflow Execution Service (WES) interface** (MIT) . **Streamlines execution, monitoring, and documentation of data processing workflows** across numerous projects . **Supports both Snakemake and Nextflow**—enables consistent automation and centralized monitoring . **Seamless integration into cloud environments**, contributing to the GA4GH cloud framework . **Best for**: research groups aiming for long-term reproducibility and scalable collaboration; suitable for larger teams and service units .



- **[Toil](https://github.com/DataBiosphere/toil)**  

  **Scalable, efficient, and portable workflow engine for batch workflows** (Apache-2.0) . **Used by UCSC for CWL execution** . **Python-based with support for CWL and WDL** .



- **[CWL (Common Workflow Language)](https://github.com/common-workflow-language/common-workflow-language)**  

  **Open standard for describing analysis workflows and tools** . **Portable across computing platforms**—the CWL project's own description emphasizes portability . **Supported by Seven Bridges, Arvados, Toil, and others** . **The most standards-based approach** to workflow description.



- **[GenBoard](https://ieeexplore.ieee.org/document/11628869)**  

  **Containerized web platform for real-time monitoring and management of genomic analysis pipelines** (IEEE 2026) . **Decouples pipeline monitoring from execution** through an event-driven architecture built on **Apache Kafka** . **Features**: **interactive DAG visualization**, **per-task resource metrics**, **execution timelines**, **integrated dataset management**, **multi-tenant architecture with organization-based data isolation**, **role-based access control**, and **dual authentication** for interactive users and programmatic pipeline clients . **The most modern open-source pipeline observability platform**—addresses the gap in Nextflow's limited real-time observability support .



### Additional Strong Open-Source Options



- **[WARP (Broad Institute)](https://github.com/broadinstitute/warp)** — **WDL Analysis Research Pipelines** (BSD-3-Clause) . **Cloud-optimized pipelines for Broad Institute Genomics Platform** and large consortia including the **Human Cell Atlas and BRAIN Initiative** . **Rigorously scientifically validated, high scale, reproducible, and open source** .

- **[Pachyderm](https://github.com/pachyderm/pachyderm)** — Data-lineage engine for version-controlled data pipelines (Apache-2.0) .

- **[Galaxy ToolShed](https://toolshed.g2.bx.psu.edu/)** — Community repository of Galaxy tool wrappers .

- **[Stjude-rust-labs/wdl](https://github.com/stjude-rust-labs/wdl)** — Rust WDL parser, **archived December 2025** . **Would need fresh effort for Rust integration** .

- Community **n8n** workflows for pipeline execution notification and result routing.



**Frameworks for building custom systems**: Combine **Nextflow** or **Snakemake** for workflow orchestration with **nf-core/tools** for community-curated pipeline standards, **WDL/Cromwell** for GATK-based pipelines, **WESkit** for GA4GH-compatible execution management, and **GenBoard** for real-time observability—creating a fully self-hosted, enterprise-grade bioinformatics pipeline platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Bioinformatics pipelines handling genomic and patient data must comply with **HIPAA, GDPR, and institutional review board (IRB) requirements**. **Data residency and consent management are critical**—verify deployment regions before processing protected health information.

- **Open-source bioinformatics pipelines are mature and production-ready.** Nextflow and Snakemake account for the vast majority of new bioinformatics pipelines . nf-core provides 84+ community-curated pipelines with rigorous testing and peer review . **These are genuine alternatives to commercial platforms.**

- **The workflow engine landscape is mature and entrenched.** Snakemake and Nextflow together dominate new pipeline development . **Rust workflow engines have no community traction**—the realistic Rust play is first-class integration with Snakemake and Nextflow, not replacement .

- **Decoupling pipeline logic from execution is the core value.** Modern workflow systems separate the analytical logic ("what to run") from the execution environment ("how to run")—the same workflow code runs on laptop, HPC, or cloud by changing configuration profiles rather than modifying workflow logic . **This is essential for malaria genomic surveillance, where analysis may be performed in both well-resourced laboratories and endemic countries with constrained infrastructure** .

- **Cloud costs require careful design.** DNAnexus and Seven Bridges pricing is not public—enterprise subscription and optional modules require commercial review . **Cohort Browser requires an Apollo license** on DNAnexus; JupyterLab and Nextflow access have their own license requirements .

- **Self-hosted open-source solutions require proper HPC/cloud infrastructure, workflow containerization, and ongoing maintenance.** **Genomic data is irreplaceable**—backup strategies and data integrity checks are non-negotiable.



---



**Made for bioinformaticians, research institutions, and developers building transparent genomic pipeline solutions.**  

Let's make Bioinformatics Pipelines more open, data-driven, and reproducible.
