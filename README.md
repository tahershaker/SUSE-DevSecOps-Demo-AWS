# SUSE DevSecOps Demo AWS

__SUSE__ DevSecOps solutions [__Rancher Prime__, __Longhorn__, __NeuVector Prime__] demonstration lab environment. Automate deployment, building, configuration and installation.

---

<p align="center">
    <img src="Images/front-image.png">
</p>

---

## Repository Purposes

As a __SUSE__ Solution Architect, it is frequently requested - as a responsibility - to perform demos and online sessions to customers, partners, and new prospects. To perform this reasonability, the SA(s) require to have a lab environment deployed and configured with the required tools and applications. Building a lab environment is very time-consuming and going through this process every time an SA has a demos or an online sessions is not the best way to utilize time. Thus, this GitHub repository is built to help SA(s) with this task.

This GitHub repository is created to support mainly __SUSE__ SA(s) in automatically build, deploy, install, & configure a lab environment on top of AWS cloud to be able to deliver a demo or an Online Sessions to customers partners or prospects showing the features and capabilities of __SUSE__ DevSecOps solutions [__Rancher Prime__, __Longhorn__, __NeuVector Prime__]. 

It is also possible for any user that would like to test __SUSE__ Solution to use this GitHub repository as he/she see fit, However, __SUSE__ do not maintain this GitHub Repository and have no responsibilities for any code provided in this repository and it is highly recommended to refer to the official documentation.

---

## Disclaimer

- This GitHub repository is created by __Taher Shaker__, who is at that time works at __SUSE__ as a Solution Architect.
- The purpose of this GitHub repository is only for demonstration and any code or deployment/installation info should not be used in production environments.
- __SUSE__ do not maintain this GitHub repository and have no responsibility for any info or code available in this GitHub repository, thus, it is highly recommended to refer to the __SUSE__ official documentation.

---

## About This GitHub Repository

This repository is created to help automating the deployment of a simple demo-purpose __Rancher Prime__ kubernetes environment on top of AWS cloud with all the required __SUSE__ DevSecOps solutions along with all other required tools and applications to be able to demonstrate __SUSE__ DevSecOps solutions capabilities and features. This GitHub repository holds several TerraForm & bash scripts as well as Linux commands to be executed manually to build the lab environment. Also there will be a step-by-step guide to help us build and deploy this lab environment. As most (nearly 90%) of the lab can be automatically provisioned using TerraForm, TerraForm is not used to provision this lab environment in full (end-to-end) and other bash scripts and manual Linux commands are used to have a fully functional lab environment.

This GitHub repository holds the following:
- __TerraForm Module__: A TerraForm module to deploy the infrastructure components on AWS such as VPC, Internet Gateway, Subnets, Security Groups, IAM Users, S3 Buckets, EC2 Instances (with SLES OS installed and configured), etc...
- __Bash Scripts__: Several bash scripts to be used on the EC2 instances to deploy and configure __Rancher Prime__, Cert-Manager, CIS Benchmarks, Keycloak Authentication, Harbor Registry, and much more.
- __Linux Commands__: Several Linux commands to be used manually to complete the required configuration that can not be added to the bash scripts - for example - due to these configurations requires some pre-requisite.
- __Step-By-Step Guide__: A Step-By-Step Guide to guide the SA/User to use this repository scripts and some configurations that must be done through the UI.
- __Files To Be Imported__: A couple of files to be imported into some solutions - for example Keycloak - to perform the required configurations for these tools.

Before using this GitHub repository, please refer to the [Lab Architecture Section](/Lab-Architecture/README.md) to understand what is going to be deployed, installed and configured.

> __Please Note:__

When using this GitHub repository, some inputs need to be changed/edited in the code. Most of the inputs required is added to the scripts in the form of variables. Still please check the code to understand exactly what is going to be deployed and change anything that you see fit. Please read carefully the instructions provided in the `Prerequisite - and/or - Adjust Code` sections.

---

## How To Use This GitHub Repository

The overall sequence for using this GitHub repository should be as follows:
- Review the lab architecture.
- Familiarize yourself with the code available in this repository.
- Check all prerequisite are installed on your laptop/machine.
- Perform any changes you need to change.
- Use the TerraForm to deploy the infrastructure.
- Use the Bash Scripts to install & configure the infrastructure with the required tools.
- Use the manual Linux Commands to complete any remaining configuration.
- Use the Solutions UI to finish the lab environment and to be ready to use.

To use this GitHub repository and deploy the demo lab, follow the below step-by-step guide available in [this page](/Lab-Deployment/README.md#step-by-step-guide):

---

__Enjoy__ :smile:

