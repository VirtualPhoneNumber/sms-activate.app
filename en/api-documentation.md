---
layout: default
title: "API Documentation - SMS Activate"
description: "Learn how to integrate and use the SMS Activate API for automated virtual number management and SMS verifications."
lang: en
permalink: /api-documentation
---

# API Documentation

Welcome to the **SMS Activate API Documentation**. This guide provides detailed instructions on how to integrate and utilize our API to automate your SMS verification processes, manage virtual phone numbers, and enhance your application's capabilities with real-time phone number services.

## Overview

The SMS Activate API allows developers to seamlessly integrate virtual phone number services into their applications. Whether you're building a system for SMS verification, customer engagement, or need numbers for testing, our API provides a robust solution.

## Key Features

- **Automated Number Allocation:** Programmatically acquire virtual phone numbers from various countries.
- **Real-Time SMS Reception:** Receive SMS messages instantly through API callbacks.
- **Extended Verification Services:** Use our numbers for verifications on platforms like WhatsApp, Instagram, Google Voice, and more.
- **Management Functions:** View, renew, or release numbers directly via API calls.

## Getting Started

1. **Register for Access:** Visit our [Get Started](https://sms-activate.app/get-started) page to sign up and obtain your unique API key.
2. **Read the Documentation:** Familiarize yourself with the available endpoints and their functions.
3. **Integrate:** Use the provided code snippets and libraries to integrate the API into your application.

## Sample Code

Here’s a basic example of how to request a new virtual number using Python:

```python
import requests

api_key = 'your_api_key_here'
response = requests.get(f"https://sms-activate.app/api/get_number?api_key={api_key}&service=whatsapp")
number_details = response.json()

print(number_details)
```

## Support and Resources

For any questions or assistance with the API:
- Contact our [Support Team](/support)
- Visit our [FAQ](/faq) page for common questions
- Check out the [Developer Community](https://developer.sms-activate.app) for discussions and tips

## Useful Links

- [API Pricing](/pricing)
- [How It Works](/how-it-works)
- [Terms of Service](/terms-of-service)

We continuously update our documentation to provide you with all necessary tools for successful integration. Ensure your applications run smoothly with reliable access to virtual numbers through the SMS Activate API.

Explore other services we offer by visiting our [Services page](/services).

**Keywords**: SMS Activate API, integrate sms verification service, automated phone number management, real-time sms reception api, virtual phone number api documentation.