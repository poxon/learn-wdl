# WDL Execution Environment Setups

Here is a list of execution environments for WDL scripts.  

Local
- laptop
- HPC

Public Cloud
- AWS - this [link](https://docs.opendata.aws/genomics-workflows/quick-start/) to AWS Cloud Formation template to set up AWS EC2 cromwell instance
  - requires AWS EC2 key pair
  - requires AWS S3 bucket
- GCP
  - This [tutorial](https://wdl-runner.readthedocs.io/en/latest/GettingStarted/TutorialOverview/#tutorial-scenario) shows running a multi-stage workflow on GCP
      - The workflow is launched with Google Life Sciences API
      - The workflow is defined using WDL
      - The workflow stages are orchestrated by cromwell
      - The workflow runs on multiple Google Compute Engine VMs
      - a master node is created for cromwell
      - cromwell submits each workflow stage as one or more separate pipelines

Bioinformatics Platforms 
- Terra.bio - runs on GCP
  - Here is a [link](https://app.terra.bio/#workspaces/fc-product-demo/Terra-Workflows-Quickstart) to a Terra.bio workspace which includes 3 versions of a WDL workflow
  - Requires an account on Terra.bio (can use free $ 300 in GCP credits to try this out)