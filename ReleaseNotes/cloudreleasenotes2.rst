Release Notes
++++++++++++++

Corolar Cloud v2.0
==================
Cost optimization and performance improvements have been our major focus for this release. This release note covers the new features and improvements you will experience when upgrading from Corolar Cloud version 1.4.1 or earlier.

Deployment Experience
######################################
Corolar Cloud v2.0 will use Azure DevOps platform for deployment. Leveraging Azure DevOps allows Dapasoft to deliver value to customers continuously. See our Deployment Guide if you need help with getting started.

Development Experience
######################################
* We improved the MLLP adapter to reduce MLLP interface operations cost and improve the deployment and management experience of MLLP adapters via Corolar Interface Management Portal (IMP).
* We have simplified the Corolar Cloud APIs by pre-populating several parameters with default values, so it’s easier for you to use it within a LogicApp.
* We have created a new Service Bus Management API in this release so that you can easily create and manage Service Bus Queues and Topics with a single API
* We have created a new C-CDA Validation API so that you can validate a C-CDA message before parsing it through the interface.
* IMP will automatically query and list all the LogicApp interfaces within an adopted resource group, so you no longer have to add tags to LogicApps in Azure Portal.
* We are now leveraging the new authentication parameter in the Azure LogicApp API calls for additional security
* Corolar Cloud fully supports the ARM VNet

Operational Experience
##################################
* We now support export and import of MLLP configuration file, so you can now promote MLLP adapters by simply importing configuration files into an environment.
* We have enhanced LogicApp Interface management capabilities in IMP, so you can now delete all the logs and exceptions associated with a LogicApp
* We have updated Operations Dashboard in the IMP to include ‘Running Status’ for all the interfaces, so it’s easier for you to filter/sort between running and stopped interfaces from the portal.
* The IMP Operations Dashboard is now synchronous so that you will see interface status changes faster

Corolar Cloud v1.4.1
======================
Hotfix for 1.4.1
#################
New features
*************
* API Management Service
    * Installs and configures Azure Service Management
    * Exposes Corolar APIs as virtual endpoints

* Endpoint Security
    * IP Restrictions used to close API Apps to external communication

Bug Fixes
*********
* Artifact (schema/maps) cache occasionally fail, and take 1h to retry
    * API settings adjusted to reduce failures, more frequent retry interval
* Some correctly tagged Logic Apps not appearing in IMP onboarding tab
    * IMP adjustment to improve reliability