# HPC cluster (supercomputer)

A High-Performance Computing (HPC) cluster consists of several compute nodes interconnected by a fast computer network (e.g., InfiniBand). Compute nodes are individual servers within the cluster that perform computational tasks. HPC clusters can be used for parallel computing, executing a complicated task simultaneously on several compute nodes, and distributed computing, performing smaller independent tasks on separate nodes or processor cores. HPC cluster allows solving complex problems faster and has the ability to tackle larger datasets.

Users access the HPC cluster remotely via the Linux command-line interface using secure shell (SSH) protocol. Multiple users can work concurrently, each with their own computing tasks and workflows, and within their working directory to store data.

## Request access
To receive access to the HPC cluster RUDENS
- research groups, course instructors, and individual students working on thesis/research must fill in the [APPLICATION FORM](https://docs.google.com/forms/d/e/1FAIpQLSemd1JlJB2lyW0Fal6OA3MM7cmxpqh0GQt145lrzmqqIFQIeA/viewform).  After receiving the application, the HPC Centre will review it and contact you on the following steps.
- students involved in the study course and need HPC as part of their course curriculum should receive an invitation from their course instructor.

## Getting started

If your application is approved, you will receive an e-mail inviting you to a project in the Waldur self-service portal. The invitation will expire in 2 weeks.

### Connect to Waldur self-service portal
Follow the link to the National Open HPC Platform: [https://nohap.hpc-net.lv](https://nohap.hpc-net.lv)
```{include} ./include/waldur_access.md
```
### Invite participants
```{include} ./include/waldur_invite.md
```
### Request HPC resource
You must belong to a project/study course to perform this step. 

First, check whether your project already has active HPC allocation. Go to Project view and check the Resources section for the existing RTU HPC (RUDENS) resource.  
![HPC resource](images/waldur_project_HPC_1.jpg)

Allocation is a certain amount of computing resources (CPU hours, GPU hours, memory) that is allocated for project use, and it is expressed in its price in EUR. Usually, there should be only one active allocation per project that all project members can use. If allocated credit is spent, you may request a new allocation or extend the existing one by depositing additional funds.

To start using the HPC cluster, press on the allocated resource name (in the example, "HPC cluster allocation"). In the resource view, you will get additional information about your username and access details.
**Request new HPC resource**. If your project doesn't have active HPC allocation, you can request it through the marketplace. Press the `Add resource` button and look for RUDENS (RTU HPC) offering. 
![marketplace HPC](images/waldur_project_HPC_2.jpg)

By pressing `Deploy,` the form will open where you should specify your deposit (in EURs) and an arbitrary name for the resource. Then press `Create`, and the request will be submitted to the RTU HPC center for review and approval.
![deploy HPC](images/waldur_project_HPC_3.jpg)

### Connect to the HPC cluster

You need an SSH key to connect to the HPC cluster RUDENS. Passwords are not supported for the accounts requested through the self-service portal. If you don't have an SSH key, you can generate one using instructions in [SSH Academy](https://www.ssh.com/academy/ssh/keygen) or [our HPC user-guide](https://hpc-guide.rtu.lv/appendix.html#generating-keys-on-windows-using-mobaxterm).

Before connection, your SSH public key must be uploaded to the Waldur self-service portal. 
- Go to the top right of the screen and click on your name to open the account window. 
- Click on the `Credentials` link to open a sub-menu where you can select `SSH keys`. 
- Copy contents of your public SSH key. 
- Wait a few minutes while the key is synchronized to the cluster.

**On Linux/macOS systems**, if the generated keys are stored in the default directory ~/.ssh/, connect to a cluster by using the `Access resource` button in the self-service portal or manually open the command line (terminal) and run the following command:
   ```
   ssh username@ui-2.hpc.rtu.lv
   ```
**For Windows SSH clients**, such as Putty or MobaXterm, the path to private key file must be specified in the connection settings.
 - For Putty: click `Connection` => `SSH` => `Auth` => `Browse` for the private key
 - For MoabXterm: click `Settings` => `Configuration` => `SSH` tab => in the agent section click on the `+` sign to import your private key

In the Session sectoin specify your username and the login node Host name as shown in the example. We recomend saving the session for future use.
![Putty](images/putty_window.png)

**Note: if the login node requests the password during connection, your SSH key is not recognized or configured correctly.**

### Start using the HPC cluster

[Follow the link to the user guide on using the HPC cluster RUDENS.](https://hpc-guide.rtu.lv)

## HPC demo-cases

Reusable examples (with codes) of HPC applications in various scientific domains: [https://gitlab.com/eurocc-latvia](https://gitlab.com/eurocc-latvia).

- Assessment of Wind Loads Using HPC
- Building Management System AI Model
- Crystal Growth
- Dielectric Constant Measurement Uncertainty Estimation using HPC
- Estimation of RF to DC Converter Power Conversion Efficiency Sensitivity to Component Parameters
- HPC Array Job Example
- Metagenomic analysis
- Metal Casting HPC Model
- MHD Mixing HPC Model
- Microchannel Flow in a Heated Plate
- Oceanographic HPDA
- Room Thermal Comfort and Epidemiological Safety
- Seasonal Weather Forecast HPDA

Demonstrations are prepared by EuroCC National HPC Competence Centre of Latvia.

## Additional guides

[MATLAB Parallel computing server](https://hpc.rtu.lv/matlabmdcs-hpc/?lang=en)

[ANSYS HPC Remote solver setup guide](https://hpc-guide.rtu.lv/appendix.html#ansys-remote-solver-manager-rsm)
