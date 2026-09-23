# BrightDesk Demo Knowledge Base

BrightDesk is a fictional B2B customer-support platform used only to demonstrate the RAG workflow in this repository.

## Product overview

BrightDesk helps small and mid-sized businesses manage customer conversations from email, website chat, and supported messaging channels in one shared inbox.

## Plans

### Starter
- Up to 3 support agents
- Shared inbox
- Website chat widget
- Basic reporting
- Email support

### Growth
- Up to 15 support agents
- Everything in Starter
- HubSpot integration
- Slack notifications
- Workflow automations
- API access
- Priority email support

### Scale
- Unlimited support agents
- Everything in Growth
- SSO/SAML
- Advanced permissions
- Audit logs
- Custom data retention options
- Dedicated onboarding support

## Billing

BrightDesk offers monthly and annual billing.

Customers on monthly plans may cancel before the next renewal date. Service remains available through the end of the paid billing period.

Annual subscriptions are billed upfront. Customers should contact support for contract-specific questions.

## Usage limits

Starter includes 2,000 automated workflow actions per month.

Growth includes 20,000 automated workflow actions per month.

Scale plans use custom limits agreed during onboarding.

If a customer exceeds the included automation allowance, BrightDesk does not silently delete or lose conversations. Additional automation actions may pause until the allowance resets or the customer upgrades.

## Integrations

BrightDesk supports:
- HubSpot on Growth and Scale
- Slack on Growth and Scale
- Zapier on all paid plans
- REST API on Growth and Scale

Salesforce integration is not included in the standard plans in this demo knowledge base.

## API

The REST API is available on Growth and Scale plans.

API authentication uses bearer tokens created by an account administrator.

## Security

BrightDesk encrypts data in transit using TLS.

SSO/SAML is available on Scale.

Audit logs are available on Scale.

This demo does not make claims about certifications such as SOC 2, ISO 27001, HIPAA, PCI DSS, or GDPR certification. If a user asks about a certification not explicitly listed, the assistant should say it cannot confirm that from the available documentation and offer human follow-up.

## Data retention

Starter and Growth use the standard platform retention policy.

Scale customers can discuss custom retention requirements during onboarding.

## Support

Starter: email support.

Growth: priority email support.

Scale: dedicated onboarding support plus priority support.

BrightDesk does not advertise 24/7 phone support in this demo.

## Human escalation

The assistant should recommend human follow-up when:
- the knowledge base does not contain the answer,
- the user asks for legal, contractual, compliance, or security guarantees not explicitly documented,
- the user requests a custom enterprise quote,
- the user has an account-specific billing or technical problem.

## Lead capture

If a visitor asks for a demo, quote, sales call, or follow-up, the assistant may ask for:
- name,
- work email,
- company.

The assistant should still answer general product questions before asking for contact details.
