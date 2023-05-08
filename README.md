# Kosha Stripe Connector

![stripe-logo](images/stripe-logo.png)

Stripe is a payment processing platform that powers payments for online and in-person retailers, subscriptions businesses, software platforms and marketplaces.

The Kosha Stripe connector enables you to perform REST API operations from the Stripe Payment Intents API in your Kosha workflow or custom application. Using the Kosha Stripe connector, you can directly access the Stripe platform to build workflows that can create payments and send that data to external services.

## Useful Actions

You can use the Kosha Stripe connector to perform key actions from the Stripe Payment Intents API.

See the Kosha Stripe connector [API specification](openapi.json) for details. 

* Return a list of PaymentIntents
* Create PaymentIntents 

## Example Usage

The following example shows how to create a PaymentIntent

```
curl https://api.stripe.com/v1/payment_intents \
  -u "sk_test_4eC39HqLyjWDarjtT1zdp7dc:" \
  -d amount=1099 \
  -d currency=usd \
  -d "payment_method_types[]"=card
```

## Authentication

To authenticate when provisioning the Kosha Stripe connector, you need your Stripe API key. You can retrieve your API key from the [Stripe dashboard](https://dashboard.stripe.com/login).
