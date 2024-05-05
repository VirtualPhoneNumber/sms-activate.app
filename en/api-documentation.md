---
layout: default
title: "API Documentation - SMS Activate"
description: "Explore the detailed API documentation for integrating SMS verification services with your systems using SMS Activate."
lang: en
permalink: /api-documentation
---

# API Documentation

Welcome to the API documentation for SMS Activate. This section provides comprehensive details and guidelines on how to integrate our virtual phone number services into your applications and systems efficiently. Whether you're looking to automate SMS verifications or enhance your application's communication capabilities, our API offers robust solutions tailored to meet your needs.

## Overview

Our API allows developers to access and manage virtual phone numbers programmatically for various use cases including SMS verification, call management, and more. It supports a wide range of operations such as number allocation, message retrieval, and real-time notifications.

## Getting Started

To begin using the SMS Activate API, you need to:

1. **Create an Account:** Sign up at [SMS Activate](https://sms-activate.app/get-started) to obtain your API key.
2. **API Key:** Securely store your unique API key which is essential for all requests.
3. **Read the Documentation:** Familiarize yourself with the available endpoints and their specific requirements.

## Key Endpoints

- **Get Number:** Allocate a new virtual phone number for receiving SMS.
- **Send SMS:** Send outgoing messages from your allocated number.
- **Check Status:** Retrieve the current status of a given phone number.
- **Release Number:** Release the number after use or when it is no longer needed.

## Example Requests

Here are some basic examples of how to use the API:

### Request a Number

```bash
curl -X GET 'https://api.sms-activate.app/get-number?api_key=YOUR_API_KEY&service=whatsapp'
```

### Check Message Status

```bash
curl -X GET 'https://api.sms-activate.app/check-status?api_key=YOUR_API_KEY&number_id=12345'
```

## Best Practices

- **Security:** Always keep your API key confidential to prevent unauthorized access.
- **Error Handling:** Implement robust error handling to manage different scenarios gracefully.
- **Resource Management:** Release numbers when not in use to avoid unnecessary charges.

## Support and Resources

For any technical issues or questions regarding the API integration, please refer to our [Support Page](/support) or contact us directly through [Email Support](mailto:support@sms-activate.app).

To explore further details about other services, visit our [Services Page](/services).

**Useful Links:**
- [Home](/)
- [Get Started with SMS Activate](/get-started)
- [FAQ](/faq)

By leveraging our detailed API documentation and following the outlined best practices, you can enhance your application's capabilities with efficient and reliable communication tools provided by SMS Activate.