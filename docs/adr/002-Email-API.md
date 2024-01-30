# Notifications provider

- **Status**: proposed
- **Deciders**: -
- **Date**: 28/01/2024

## Context and Problem Statement

We need a provider to send emails and SMS.

## Decision Drivers

- Ease of integration.
- Costs of using the service.
- Documentation, if good, complete.
- Service support.
- Developer community.

## Considered Options

- [Twilio](https://www.twilio.com/es-mx/docs)
- [SendGrid](https://docs.sendgrid.com/for-developers)
- [Amazon SES](https://aws.amazon.com/es/ses/developer-resources/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc)

### Twilio

- Pro, wide Coverage: Offers services for SMS and phone calls worldwide.
- Pro, Clear Documentation: Twilio has extensive documentation and code examples to make integration easy.
- Pro, support for Multiple Channels: In addition to SMS, it provides voice and verification services.
- Cons, cost: Can be relatively more expensive compared to some alternatives, especially for large volumes.
- Pro, Services and community: it provides good technical support through its help center and community forums. It is known for its good customer service.
- Cons, complexity: It can be complex for smaller or simpler projects.

### SendGrid

- Pro, scale: It is suitable for sending large volumes of emails.
- Pro, good Analysis Tools: Offers advanced analytical tools to monitor email performance.
- Pro, integration with Twilio: Now part of Twilio, allowing you to integrate SMS and email services from a single platform.
- Pro, Services and community: it has good documentation and resources for developers. Its community is not that big, but it is active. The technical support is quite fast and effective.
- Cons, Email Verification support: SendGrid does not provide specific functions for email address verification.

### Amazon SES

- Pro, Scalability: Designed for scalability and handling of large volumes.
- Pro, Integration with Other AWS Services: Can easily integrate with other AWS services.
- Pro, Free Use Plan: Offers a free level with certain usage limits.
- Cons, Learning Curve: May have a learning curve if you are new to the AWS platform.
- Cons, Initial Restrictions: There may be initial restrictions that you must overcome to avoid shipping limitations.