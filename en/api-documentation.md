---
layout: default
title: "API Documentation - SMS Activate"
description: "Explore detailed documentation for using the SMS Activate API to integrate virtual phone number services into your applications."
lang: en
permalink: /api-documentation
---

# API Documentation

Welcome to the **SMS Activate API Documentation**. Here, you will find all the necessary information to integrate our robust virtual phone number services into your applications. Whether you're looking to enhance your business communication, implement SMS verification systems, or manage multiple numbers dynamically, our API provides a flexible and powerful solution.

## Getting Started with the API

To begin using the SMS Activate API, follow these steps:
1. **Create an Account:** Register on [SMS Activate](https://sms-activate.app) to obtain your API credentials.
2. **Generate API Key:** Access your dashboard to generate an API key which will be used to authenticate your requests.
3. **Review Documentation:** Familiarize yourself with the available endpoints and their purposes below.

## Key Features of the API

- **Real-Time Number Allocation:** Instantly allocate numbers from over 100 countries for SMS verification purposes.
- **SMS Fetching:** Retrieve SMS messages programmatically as soon as they are received.
- **Number Management:** Release or renew numbers based on your operational requirements.
- **Webhook Implementation:** Set up webhooks to receive real-time notifications for received messages.

## Endpoints Overview

### Authentication Endpoint
- **URL:** `/api/auth`
- **Method:** `POST`
- **Description:** Authenticate users and retrieve an access token.

### Allocate Number
- **URL:** `/api/allocate_number`
- **Method:** `GET`
- **Description:** Allocate a new virtual phone number for receiving SMS.

### Fetch Messages
- **URL:** `/api/fetch_messages`
- **Method:** `GET`
- **Description:** Fetch all messages received by a specific number.

### Manage Number
- **URL:** `/api/manage_number`
- **Method:** `POST`
- **Description:** Renew or release a number based on your needs.

## Example Requests and Responses

```json
// Request for allocating a number
GET /api/allocate_number?country=US&service=WhatsApp
{
    "apiKey": "your_api_key_here"
}

// Response
{
    "status": "success",
    "number": "+1234567890",
    "country": "US"
}
```

## Best Practices for API Integration

- Ensure secure storage and usage of API keys.
- Handle errors gracefully and implement retries for failed requests.
- Use webhooks for efficient real-time updates instead of polling endpoints.

## Support and Further Assistance

For any technical issues or detailed queries not covered in this documentation, please reach out through our [Support Page](/support) or contact us directly via [Email Support](mailto:support@sms-activate.app).

## Related Links

Navigate through other related services:
- [Virtual Phone Numbers](/virtual-phone-numbers)
- [SMS Verification](/sms-verification)
- [Temporary Phone Numbers](/temporary-phone-numbers)

**Ready to start integrating?** Visit the [Get Started page](/get-started) to explore how you can leverage [@PrivatePhoneBot](https://t.me/PrivatePhoneBot) for seamless online verifications and more!

Enhance your application's capabilities with reliable SMS functionalities today!