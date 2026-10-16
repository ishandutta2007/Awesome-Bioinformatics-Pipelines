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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Seven Bridges](https://www.sevenbridges.com/)**  

  **The most CWL-centered commercial platform**—native authoring and execution model maps directly to the published Common Workflow Language standard . Hosts the **NCI Cancer Genomics Cloud** with more than **850 curated tools and workflows** . Supports CWL 1.0/1.1/1.2, Nextflow packaged as ZIP, and WDL through wrappers (with different caching and job behavior) . **Deployment**: virtual private cloud, local HPC, or hybrid; current project locations name AWS us-east-1 and Google Cloud us-west1, with Azure regions on request . **Limitation**: nonpublic license rates—priced through Sales .



- **[DNAnexus](https://www.dnanexus.com/)**  

  **Governed data workspace** for omics, phenotype, notebooks, applications, and workflows under a managed project boundary . **Multi-language ingestion**: native workflows, CWL, WDL, and licensed Nextflow provide migration paths . Documented compute catalog includes **AWS, Azure, and Oracle Cloud Infrastructure GPUs** . Exchanges with ELNs, LIMS, and clinical data management systems; enterprise identity services can be used for organization login . **Limitation**: public pricing not available—enterprise subscription and optional modules require commercial review; Cohort Browser requires an Apollo license .



- **[Illumina BaseSpace](https://www.illumina.com/products/by-type/informatics-products/basespace-sequence-hub.html)**  

  Illumina's cloud platform for sequencing data analysis, storage, and sharing. **Native integration with Illumina sequencing instruments** for seamless data upload. Hosts a large catalog of apps and workflows for secondary analysis.



- **[Terra.bio](https://terra.bio/)**  

  **Biomedical data analysis platform** developed by the Broad Institute, Microsoft, and Verily. Features **Jupyter notebooks, WDL/Cromwell workflows, and data sharing** across institutions. **Trusted by the Human Cell Atlas, BRAIN Initiative, and large consortia** .



- **[Nextflow Tower (Seqera Platform)](https://seqera.io/)**  

  **Nextflow control plane**—pipeline model is explicitly version-controlled, access-controlled, and reproducible . **The cleanest fit when Nextflow source and configuration are already authoritative** . **Portability spans executors rather than multiple workflow languages**—official training material names **Slurm, LSF, SGE, and PBS** among supported HPC schedulers .



- **[Galaxy Cloud](https://usegalaxy.org/)**  

  **Web-based GUI workflow platform** with a large tool catalog . **AFL-3 licensed**. Galaxy Cloud and BRC Analytics were developed to address infrastructure limitations and enhance accessibility and reproducibility . **The most accessible entry point** for researchers without command-line expertise.



- **[Cromwell Cloud](https://cromwell.readthedocs.io/)**  

  **Broad's WDL execution engine**—Scala-based, BSD-3-Clause . **The execution engine behind GATK4-based pipelines** . Available as a managed service through Terra and other platforms.



- **[Arvados](https://arvados.org/)**  

  **Open-source platform for managing and processing genomic and biomedical data** . **Curoverse's Arvados runs bcbio pipelines via CWL** . **The open-source alternative to commercial genomics platforms**—used by academic and research institutions.



- **[BC Platforms](https://www.bcplatforms.com/)**  

  **Genomics data management and analytics platform** for healthcare and research. Features **biobank management, cohort discovery, and clinical interpretation**.



- **[LifeOmic](https://lifeomic.com/)**  

  **Cloud platform for precision health** with genomics data management, clinical data integration, and analytics. **The most focused on clinical genomics** workflows.



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
