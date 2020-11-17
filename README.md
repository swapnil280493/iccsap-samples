# Deploying IBM Content Collector for SAP

 IBM Content Collector for SAP provides advanced archiving capabilities that help SAP users run their businesses more efficiently. It provides access to business information of all types, supports the transfer of older information to lower-cost disks and tapes, and improves system performance. It includes the following advanced capabilities:
 - Helps improve system performance by managing the growth of SAP applications
 - Reduces investments for extra hardware
 - Makes business documents available to authorized users anywhere on your network
 - Increases productivity by making documents easily accessible from an SAP GUI
 - Integrates with FileNet® P8 repositories
 - Integrates with IBM Content Navigator.

## Requirements and prerequisites

Perform the following tasks to prepare to deploy your IBM Content Collector for SAP images on Kubernetes:

- Prepare your IBM Content Collector for SAP environment. These procedures include setting up storage, and configuration files that are required for use and operation. You must complete all of the [preparation steps for IBM Content Collector for SAP]( https://www.ibm.com/support/knowledgecenter/SSRW2R_4.0.0/doc/container/tsk_preparing.html) before you are ready to deploy the container images. 

- Prepare your Kubernetes environment. See [Preparing for deployment with an operator]( https://www.ibm.com/support/knowledgecenter/SSRW2R_4.0.0/doc/container/tsk_preparing.html)

## Deploying with an operator

The IBM Content Collector for SAP operator is built from the Red Hat and Kubernetes Operator Framework, which is an open source toolkit that is designed to automate features such as updates, backups, and scaling. The operator handles upgrades and reacts to failures automatically.

To prepare your operator and deploy your IBM Content Collector for SAP components, follow the instructions for your operator platform:

- [Certified Kubernetes](operator/platform/k8s/README.md)
- [Red Hat OpenShift](operator/platform/ocp/README.md)

## Completing post deployment configuration

After you deploy your container images, you perform some required and some optional steps to get your IBM Content Collector for SAP environment up and running. For detailed instructions, see [Completing post deployment tasks for IBM IBM Content Collector for SAP](https://www.ibm.com/support/knowledgecenter/SSRW2R_4.0.0/doc/container/tsk_comp_post_deploy_tsks.html)
