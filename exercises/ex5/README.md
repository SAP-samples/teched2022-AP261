# Exercise 5 - Explore Agricultural Origination Portal Integration Aspects

SAP provides seamless integration between SAP Agricultural Origination Portal and SAP Agricultural Contract Management for SAP S/4HANA. This integration is achieved with the help of published integration content in SAP Cloud Integration Suite.

##During this exercise, the following aspects will be explored in SAP Cloud Integration Suite:

* Capabilities of SAP Cloud Integration Suite.
* Explore Event Driven Architecture via SAP Event Mesh
* Published integration packages for integration between SAP Agricultural Origination Portal and SAP Agricultural Contract Management for SAP S/4HANA.


1. Log into SAP Event mesh using the below URL and navigate to message client:
https://teched2022-ap261.enterprise-messaging.cfapps.us10.hana.ondemand.com/#/message_clients
<br>![](/exercises/ex5/images/image1.png)
<br>![](/exercises/ex5/images/image2.png)

2. Explore the following queue and notice the name of the topic it subscribes to
   * Onboarding Queue
   
<br>![](/exercises/ex5/images/image3.png)

3. Login to the SAP Cloud Integration Suite using below URL and navigate to Design
https://teched2022-ap261.integrationsuite-it-aiat001.cfapps.us10.hana.ondemand.com/shell/design

<br>![](/exercises/ex5/images/image4.png)

4. Navigate to the package: SAP Agricultural Contract Management for SAP S/4HANA Transactional Data Integration with SAP Agricultural Origination Portal and open integration flow: Replicate Transactional Data for Business Partners from SAP Agricultural Contract Management for SAP S4HANA to JMS Queue.
	* Open the AMQP adaptor in the start of the flow and check the details.
  * Observe the name of the queue.

<br>![](/exercises/ex5/images/image5.png)
<br>![](/exercises/ex5/images/image6.png)
<br>![](/exercises/ex5/images/image7.png)
<br>![](/exercises/ex5/images/image8.png)
  
  
[OPTIONAL]
5. Create and Deploy a new flow to update contracts data from ACM S/4HANA to AOP:

	* Create a new package: ID_ACM_to_AOP
	
	* Copy the iflow from the existing flow: Sample_Contracts_Update in package Sample_ACM_to_AOP to your package created in previous step. Name the 	   iflow as ID_ACM_to_AOP.

	
	* Configure the URL for ACM Contracts in the HTTP adaptor: Get Contract from S/4HANA 
	
	
	* Configure the URL for AOP Contracts in the HTTP adaptor:  Update Contract to AOP

Summary
You've now explored the event driven integration architecture of SAP Agricultural Origination Portal.

Continue to - Exercise 6 https://github.com/SAP-samples/teched2022-AP261/tree/main/exercises/ex6 to explore the public APIs available for SAP Agricultural Origination Portal.

