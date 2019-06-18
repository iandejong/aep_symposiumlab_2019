## Exercise 1.3: Launch & Platform Data Ingestion Configuration
In this exercise, the goal is to install and configure Launch and Platform to capture data from our La boutique demo website.

### Learning Objectives
- Learn how to integrate Adobe Experience Platform Launch onto a webpage
- Create Launch rules to stream data to Experience Platform using the new Adobe Experience Platform extension
- Map data elements to XDM
- Launch on a real site

### Lab Resources

- Launch URL: [https://launch-demo.adobe.com](https://launch-demo.adobe.com)

### Lab Tasks
- Create Launch property and add streaming endpoint to webpage
- Create data elements and rules to stream a data beacon into Experience Platform
- Observe the beacon firing, and landing in Experience Platform


### Story

After setting up our website, we now want to make sure that new Profile data (from sign-ups) and behavioral ExperienceEvent data (browsing habits, actionable triggers, etc) are recorded and updated in near real-time. We can do this by utilizing Adobe Experience Platform Launch on our website. For this exercise, we will step into the shoes of the owners of La Boutique, a fashion retail website, and see how we can bring in behavioral and profile data from website interactions into Experience Platform.


### [Exercise 1.3.1 - Configure Launch Extensions](./ex2.md)
In this exercise, you'll be configuring the required Launch extensions for your property.

### [Exercise 1.3.2 - Configure Launch Rules](./ex5.md)
After the configuration of your Launch property with extensions and data elements, and the configuration of your datasets in the Platform UI, you're now ready to configure your Launch rules to send real data into Platform.

### [Exercise 1.3.3 - Publish your Launch Property](./ex6.md)
With all Launch configuration done now, let's publish your Launch property.

#### Go back
[overview](../README.md)
