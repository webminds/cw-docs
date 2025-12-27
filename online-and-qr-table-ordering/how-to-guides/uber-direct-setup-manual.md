# Uber Direct Setup Manual

## Uber Direct Setup Manual

### **Requirements** <a href="#requirements" id="requirements"></a>

To enable Uber deliveries, the restaurant should have all the following:

* Stripe + Setup done by us
* Restaurant from the following countries:
  * Australia
  * New Zealand

### Enabling Uber <a href="#enabling-uber" id="enabling-uber"></a>

Uber DaaS is a reliable and convenient way to get your food delivered quickly and efficiently. Here's how to enable it:

{% hint style="success" %}
Uber direct advanced feature provided without any additional cost. If you need it, please contact your sales manager to subscribe.
{% endhint %}

1. Set Uber as Default Delivery

Once you have enabled Uber DaaS, you can select the Default Delivery Provider in the Settings > Services > Deliveries (as shown in the image below)

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### Notes: <a href="#notes" id="notes"></a>

* Make sure that your Map Data Source is Google Maps. Go to Settings > System > Location > Map Data Source.

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

* Currency must match the country’s location and Uber country availability. Go to Settings > System > General > Currency.

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

* Uber requires valid phone number from your store (Must have the country code). Go to Settings > System > Location > Phone Number.

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### Checkout Details <a href="#checkout-details" id="checkout-details"></a>

Once a customer checkout an order, the Uber (if set as the Default Delivery Provider in Admin Dashboard) will be displayed as the Delivery Provider.

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

**The Delivery Estimation will provide the:**

**Delivery Provider** - which is Uber

**Estimated Fee** - the total fee

**Tips** - entered by the user and will be sent to the Uber driver directly

**Estimated Delivery Time** - time from now to drop off

**The acceptable Payment Method will be the following:**

**Credit Card** - if enabled and with Stripe Connect account ID provided

**Apple Pay** | **Google Pay (Stripe**) - if enabled

### Order Workflow <a href="#order-workflow" id="order-workflow"></a>

Once the customer made the order, in Admin Dashboard, the order’s thumbnail will be replaced to the Uber logo (denoting that it will use Uber)

**Order: UNCONFIRMED**

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

**Order: CONFIRMED**

The order **SHOULD** go through to the **CONFIRMED** status to trigger the Uber delivery request.

Once the order is set to CONFIRMED, the Delivery Tracking URL will be available both in the ADMIN and the CUSTOMER.

![](<../../.gitbook/assets/image (24).png>)Admin Order View

![](<../../.gitbook/assets/image (25).png>)Customer Order View

![](<../../.gitbook/assets/image (29).png>)Sample Screenshot of the Tracking URL

\
SMS sent by Uber to the recipient.

\
**Order: READY**

![](<../../.gitbook/assets/image (27).png>)Customer Order View

It is expected that the driver is still on route to the restaurant or is waiting in the restaurant.

**Order: ON ROUTE**

![](<../../.gitbook/assets/image (28).png>)Admin Order View

**Order: CANCELLED**

If the Order is cancelled (initiated by the customer or the store), the Uber delivery will be automatically cancelled as well
