# Containerized PACS: DCM4CHEE + OHIF Viewer

## Project Overview
This repository details the deployment of a professional Picture Archiving and Communication System (PACS) using Docker. It provides a full-stack imaging solution for the healthcare sector, allowing for study storage, retrieval, and zero-footprint web-based viewing[cite: 1].

## Document
The document is available "PACS_Installation_SOP"

## Technical Stack
- **OS:** Ubuntu 22.04[cite: 1]
- **Orchestration:** Docker Compose[cite: 1]
- **Core Archive:** DCM4CHEE-ARC-PSQL (running on Wildfly)[cite: 1]
- **Database:** PostgreSQL (pacsdb)[cite: 1]
- **Identity & Config:** OpenLDAP[cite: 1]
- **Diagnostic Viewer:** OHIF Viewer (Port 3000)[cite: 1]
- **Management:** Portainer (Port 9000)[cite: 1]

## Key Configurations
- **Modality Integration:** Configured to accept DICOM studies on Port 11112[cite: 1].
- **DICOMWeb API:** Integrated OHIF with DCM4CHEE using WADO/QIDO roots for seamless image streaming[cite: 1].
- **Data Persistence:** Managed via Docker Volumes for long-term storage of studies and metadata[cite: 1].

## Architecture Diagram
![PACS Architecture](./images/containerized_pacs_architecture.png)