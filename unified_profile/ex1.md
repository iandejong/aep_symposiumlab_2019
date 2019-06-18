## Exercise 1 - Visit the Luma website

In this exercise, you'll follow a script and walk through the Luma website on your local machine.

The URL to access the Luma website is: [http://luma.adobe.com](http://luma.adobe.com:8080)
 
### Story
In this exercise, the goal is to have you walk through the Luma customer journey and act like a real customer.

You can access the demo website by going to [http://luma.adobe.com](http://luma.adobe.com:8080)

On this website, we've implemented Adobe Experience Platform. Every activity is considered an 'Experience Event', is sent like that to Adobe Experience Platform in real-time, and hydrates the Real-Time Customer Profile.

In this journey, you'll start as an anonymous customer who browses the Luma website and after a couple of steps, you'll become a known customer which will fuel Adobe Experience Platform's Real-Time Customer Profile.


### Exercise 1.1 - Visit the Luma website

Let's start.

Go to to [http://luma.adobe.com](http://luma.adobe.com:8080).

![Demo](./images/1_1.png)

In the site's menu, click on 'Men' to visit that page.

![Demo](./images/luma2.png)

In the site's menu, click on 'WOMEN' to visit that page.

![Demo](./images/luma3.png)

In the site's menu, click back on 'HOME' to visit that page.

![Demo](./images/1_1.png)

On the Home page, scroll down and click on the first product 'Harmony Lumaflex™ Strength Band Kit' to visit that page.

![Demo](./images/lumahome_product.png)
![Demo](./images/product_rope.png)

In the site's menu, click back on 'HOME' to visit that page.

![Demo](./images/1_1.png)

After visiting the Luma home page, go to the Login/Register page and fill out your own details to register. Click "Create Account" to create your account.

![Demo](./images/luma_login.png)

Go back to the Homepage of the Luma website and open the Adobe Experience Platform X-ray panel. The X-ray panel is a live and dynamic panel that updates in real-time and shows the kind of information that is available in Adobe Experience Platform.

By opening the Real Time Customer Profile panel, you should see something similar to the below, showing the different identities that are part of your profile, together with the declared personal information that you filled out on the registration form.

![Demo](./images/luma_xray.png)

By opening the Experience Events panel, you should be seeing an entry for each page you've visited. Please note that Adobe Experience Platform captures and stores all data by linking it to an ID, regardless of whether the customer was anonymous or known. You'll notice that all your page views are shown here, also for the pages that were visited while you were still unknown.

![Demo](./images/luma_xray_exp.png)

Now let's buy a product. On the Home page, scroll down and click on the second product 'Zeppelin Yoga Pant' and then click 'ADD TO CART'.
You should see the basket icon, in the top right hand corner, update to show the item has been added.

![Demo](./images/luma_product_addcart2_2.png)

In the site's menu, click back on 'HOME' to visit that page.
Scroll down and click on the third product 'Autumn Pullie'.
Click 'ADD TO CART' twice to add two of these products to your cart.

![Demo](./images/luma_product_addcart3.png)


You should see the amount of products being updated on the shopping basket in the upper right corner of your screen. 

![Demo](./images/luma_basket.png)

Click on the shopping basket icon to start the checkout process.

On the Cart page, select your payment method and delivery type. Click Purchase to finalize the purchase.

![Demo](./images/luma_checkout.png)

On the purchase confirmation page, you'll see your order confirmation.

![Demo](./images/luma_checkout_confirm.png)

Open the X-ray panel again, to see the updated Experience Events, where you should see additional Browse Activity and also, the products that you added to your basket.

![Demo](./images/luma_xray_cart.png)

With this information on the X-ray panel, let's now have a look inside Adobe Experience Platform.

---

[Next Step: Exercise 2 - Visualize your own real-time customer profile](./ex2.md)

[Back to LAB Home](../README.md)
