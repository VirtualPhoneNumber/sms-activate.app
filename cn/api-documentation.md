---
layout: default
title: "API 文档 - SMS Activate"
description: "探索如何通过 SMS Activate 的 API 整合短信验证服务到您的系统。"
lang: cn
permalink: /cn/api-documentation
---

# API 文档

欢迎使用 SMS Activate 的 API 文档页面。在这里，我们提供详细的指南和示例，帮助您快速并有效地将我们的短信验证服务整合到您的应用程序或系统中。

## 主要特点

- **实时短信交付**：确保您可以即时接收验证码。
- **高度兼容性**：支持超过 700 种网站和应用程序。
- **灵活的号码管理**：轻松更换和管理虚拟号码。
- **Webhook 集成**：自动化您的工作流程，提高效率。
- **全球覆盖**：提供多个国家的号码，满足国际化需求。

## 开始使用

要开始使用 SMS Activate 的 API，请按照以下步骤操作：

1. 访问 [SMS Activate 网站](https://sms-activate.app) 并注册账户。
2. 在用户仪表板中生成 API 密钥。
3. 参考本文档设置 API 调用。

## API 能力

### 获取号码

`GET /api/get-number`

参数：
- `country`: 国家代码
- `service`: 服务标识符（例如，whatsapp, google）

返回：
- `number`: 分配的虚拟电话号码
- `session_id`: 会话标识符

### 发送验证码

`POST /api/send-code`

参数：
- `session_id`: 会话标识符
- `message`: 验证码信息

返回：
- `status`: 发送状态

### 验证代码接收

`GET /api/check-code`

参数：
- `session_id`: 会话标识符

返回：
- `code`: 接收到的验证码
- `status`: 验证状态

## 示例代码

```python
import requests

# 获取虚拟号码
response = requests.get("https://sms-activate.app/api/get-number?country=CN&service=whatsapp")
number_details = response.json()

# 发送验证码
send_response = requests.post("https://sms-activate.app/api/send-code", data={"session_id": number_details['session_id'], "message": "Your code is 1234"})
print(send_response.json())

# 检查验证码接收情况
check_response = requests.get("https://sms-activate.app/api/check-code?session_id=" + number_details['session_id'])
print(check_response.json())
```

## 更多资源和支持

如果您在整合过程中遇到任何问题，或需要更多帮助，请通过 [联系我们](/cn/contact) 页面与我们的技术支持团队联系。同时，不要忘记访问我们的 [常见问题解答](/cn/faq) 页面获取更多信息。

立即体验 [@PrivatePhoneBot](https://t.me/PrivatePhoneBot)，享受便捷、安全的短信验证服务！

[首页](/cn/) | [服务](/cn/services) | [短信验证](/cn/sms-verification) | [虚拟号码](/cn/virtual-phone-numbers) | [临时号码](/cn/temporary-phone-numbers) | [精英号码](/cn/elite-phone-numbers) | [免费号码](/cn/free-phone-numbers) | [开始使用](/cn/get-started)

此页面旨在为开发者提供必要工具，以便轻松集成和使用 SMS Activate 提供的服务。