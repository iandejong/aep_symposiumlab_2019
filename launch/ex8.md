## Exercise 1.2.8 - Verify Data Ingestion from website into Platform

After implementing the Launch Tag on your website, you should start to see calls being sent towards Platform.

These calls are sent to the DCS Endpoint that you configured in exercise 1.2.2.

To verify if calls are being sent, open your website by going to [http://localhost:8888/index.html](http://localhost:8888/index.html) in Chrome and at the same time open the Chrome Developer Tools.

![Verify Calls](./images/devtools.png)

![Verify Calls](./images/sitedevtools.png)

Open the Chrome Developer Tools on the "Network"-view and then refresh your page.

By refreshing your page, you'll see all the calls being sent from the page to various servers, including the calls to the DCS Endpoint of Platform.

![Verify Calls](./images/sitecalls.png)

To easily find the calls to Platform, you can apply a filter by entering "dcs" in the Filter-field.

![Verify Calls](./images/dcsfilter.png)

This should give you 1 call to Platform, which is the call that sends in ExperienceEvent-data on every pageload.

![Verify Calls](./images/plcall.png)

Select the call to the DCS Endpoint, and scroll down until you see "Request Payload".

![Verify Calls](./images/payload.png)

Click on "view source" to view the full raw call to Platform.

![Verify Calls](./images/rawcall.png)

Select the full raw text and copy it.

![Verify Calls](./images/selectedraw.png)

Go to [https://jsonformatter.org/json-pretty-print
](https://jsonformatter.org/json-pretty-print
) and paste the copied raw text in the left window.

![Verify Calls](./images/makepretty.png)

Click on "Make Pretty" to see a readable version of the call to Platform.

![Verify Calls](./images/prettycall.png)

Next, go to to the Login/Register-page [http://localhost:8888/login-register.html](http://localhost:8888/login-register.html)

Make sure the Chrome Developer Tools-window is still open.

![Verify Calls](./images/register.png)

Enter your First Name, Last Name, Email and Password and click "Create Account".

![Verify Calls](./images/createaccount.png)

With the "dcs"-filter in the Network-tab active, you're now seeing 2 calls being sent to Platform.

![Verify Calls](./images/2calls.png)

Select the first call and scroll down until you see the Request Payload.

![Verify Calls](./images/profilepayload.png)

Click on "view source" and copy the full raw payload.

![Verify Calls](./images/rawprofile.png)

Go to [https://jsonformatter.org/json-pretty-print
](https://jsonformatter.org/json-pretty-print
) and paste the copied raw text in the left window, then click on "Make Pretty" to see the full payload in a readable format.

![Verify Calls](./images/prettyprofile.png)

If you see 2 calls going out to the DCS Endpoint, that means that Launch is correctly activating calls to Platform.

Now we need to verify whether these calls are successfully received by Platform.

To log in to Platform, go to [https://platform.adobe.com/home](https://platform.adobe.com/home). 

Go to "Datasets" and locate your 2 Datasets. As a reminder, the shared datasets we're using are called:

* Website Interaction Dataset name: 
  
  * **Website Interactions - EMEA EE Dataset (API)**
      ![Platform Setup](./images/ee.png)

* Website Registration name: 
  
  * **Website Registrations - EMEA Profile Dataset (API)**
      ![Platform Setup](./images/p.png)

Datasets in the UI of Platform are usually updated every 15minutes.

You can immediately see if the ingestion of the last batch of data for this dataset was successful:

![Verify Calls](./images/datasetstatus.png)

And by opening the "Website Interactions - EMEA EE Dataset (API)"-dataset you can see all individual ingested batches for this dataset.

![Verify Calls](./images/alleebatches.png)

By clicking on "Preview", you can see a preview of the ingested data.

![Verify Calls](./images/previewbtn.png)

![Verify Calls](./images/eepreview.png)

You can do the same thing for the "Website Registrations - EMEA Profile Dataset (API)"- dataset:

![Verify Calls](./images/profilebatches.png)

Also have a look at the "Preview" of Profile Data to retrieve your ingested data.

![Verify Calls](./images/profilepreviewdata.png)

If both of your Datasets have successfully received the data coming from your website, you've finished this exercise! Congratulations!

[Next Step: Exercise 3 - Data Ingestion](../data_ingestion/README.md)



