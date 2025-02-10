# Project
> [!NOTE]
This repository is part of the Azure Proactive Resilience project and the Well Architected Reliability Assessment. It holds automation that pulls from the APRL repo and generates a recommendation object that is consumed downstream by WARA and potentially other tools.


## Contents
- Workflows
    - Build-Recommendation-Object.yaml
- Scripts
    - Build-Recommendation-Object.ps1
- Objects
    - recommendations.json

## How it works
> [!IMPORTANT]
The Build-Recommendation-Object workflow is triggered every 15 minutes. The workflow will clone the APRL repo, run the Build-Recommendation-Object.ps1 script, and then push the recommendation object to the main branch of the WARA repo. The recommendation object is a JSON file that contains all the recommendations from the APRL repo.

> [!NOTE]
This repository is private, but the github pages are public. The recommendation object is hosted on the github pages of this repository. The URL to the recommendation object is [https://<github-username>.github.io/objects/recommendation-object.json](https://azure.github.io/WARA-Build/objects/recommendations.json).

## Contributing

Only current contributors to the Azure Proactive Resilience project can contribute to this repository. If you are interested in contributing, please contact one of the contributors.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
