---
layout: post
title:  "Integrating razorpay into your webapp"
date:   2019-03-23 21:03:36 +0530
categories: Javascript NodeJS
---
Integrate Razorpay Standard Checkout with your website to start accepting online payments from your customers. Razorpay supports a slew of payment methods such as netbanking, credit and debit cards, wallets and UPI. Our Standard Checkout library provides all the essential features for integrating Razorpay Checkout with the client-side of your application. This is available only for web-based integrations.

```javascript
const Razorpay = require('razorpay');

let rzp = Razorpay({
	key_id: 'KEY_ID',
	secret: 'name'
});

// capture request
rzp.capture(payment_id, cost)
	.then(function (data) {
		return 2;
	})
```
Types of Standard Checkout Integration#
There are 2 types of Standard Checkout Integration available. Select the integration method as per your business requirements.

Automatic Checkout#

An easy integration method to integrate with your product.
This method provides the default Razorpay Pay with Razorpay button that invokes the Checkout form. The Checkout form options are passed as data attributes inside a script tag. You can add any additional, hidden or visible fields to the form, which will be submitted along with the form.


Manual Checkout#

Provides a greater control of the payment process. Use this method when you have multiple products or a complex way to pre-calculate amount for a payment (in javascript). The Checkout form is invoked by the custom button on your site and form options are passed as variables in a key-value pair format within a script tag.

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
