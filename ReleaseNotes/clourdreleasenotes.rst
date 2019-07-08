Release Notes
+++++++++++++

Corolar Cloud v2.1
==================

This release note covers the new features and improvements you will experience when upgrading from previous versions of Corolar Cloud.

Deployment Experience
######################################
* Corolar Cloud now also supports the use of Azure AD B2C for authentication, users can now set up authentication mode to be either AAD or B2C at the time of deployment
* We have updated our deployment guide to include changes made for Corolar Cloud v2.1, please refer to our updated deployment guide for more details
* Enhancement to the Azure usage reporting by providing more visibility into the status of the Corolar Cloud deployment and consumption of Azure resources. The data is collected and governed by Microsoft's privacy policies.

Development User Experience
######################################
* Users now have the ability to set up MLLP receive interfaces to send messages directly to an external system. This would be useful in situations where the source system would want to receive an acknowledgment from the external system before logging or processing the messages further.
* We have implemented a new feature in the Corolar Visual Studio Toolkit, that would allow users to disable input and/or output schema validation when testing the transformation maps.
* We now support for durable functions as an interface development platform. Developers can now use Durable Functions in addition to Logic Apps and onboard them via Management Portal.

Operations User Experience
######################################
* When creating new MLLP interfaces, users can now choose existing service bus topics and queues
* The workflow for managing user permissions have changed in IMP, please refer to our user guide for more details and instructions.


