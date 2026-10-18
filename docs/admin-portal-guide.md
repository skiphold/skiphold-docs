---
title: "SkipHold Admin Portal Guide: White-Label AI Communications | SkipHold Docs"
description: "Manage SkipHold white-label AI communications: AI agents, Prompt Tools, warm transfers, live monitoring, Conversations, CRM, help desk, telephony and billing."
---

# Admin Portal Guide: Managing White-Label AI Communications and Call Answering

The Admin Portal (https://admin.skiphold.com, or your own branded domain) is where providers and companies manage everything in SkipHold. New here? Start with [Getting Started](getting-started.md).

## Roles and views

| Role | What they manage |
|---|---|
| Provider Admin | All customer companies, users, branding, billing, telephony and provider-wide reporting |
| Company Admin | One company's agents, departments, employees, telephony, conversations and settings |
| Employee | Their own account, their personal Assistant agent and their softphone |

Admins can grant or remove individual permissions per user.

## AI Agents: Receptionist, Manager and Assistant

- Create **Receptionist**, **Manager** (one per department) and **Assistant** (one per employee) agents. See [AI voice agent types](https://skiphold.com/ai-voice-agent-types).
- Choose a role: General Receptionist, Appointment Setter, Lead Qualifier, Document Sender, Support Intake, After Hours, General Personal Assistant or General Manager.
- Set voice (ElevenLabs and other leading voice providers), language (English, Spanish, Portuguese), greeting, personality, business context and instructions.
- Use **Prompt Tools™**, the visual prompt builder with templates and role-based context, to write or analyze instructions.
- In-call tools: transfer, handoff, send SMS, send WhatsApp, DTMF keypad and end call.
- Test with **Start Call** or **Start Chat**. The call routing map shows how calls move between agents and people.

## AI warm transfers and call routing

- Transfers can be blind, or warm with an AI summary for the person picking up. See [AI warm transfers](https://skiphold.com/warm-transfers).
- Screening options let the person accept or decline the call, or have it announced first.
- Fallback rules cover transfers that go unanswered.

## Meeting Join™

- AI agents join Zoom, Google Meet and Microsoft Teams calls by dialing in and entering meeting IDs/PINs via DTMF. See [Meeting Join™](https://skiphold.com/ai-meeting-participant).

## Live call monitoring

- Providers and company admins can watch calls in progress as they happen.

## Departments, Employees and Users

- Departments and employees define where handoffs and transfers go.
- Under Users, invite people and assign roles and permissions.

## Conversations: omni-channel voice, SMS and WhatsApp

- One inbox where AI and human teams work every conversation together, across voice, SMS and WhatsApp.
- Take over any thread from the AI agent, then hand it back.
- Each call shows its recording, transcript and AI summary.
- More at [Conversations](https://skiphold.com/conversations).

## Connections: CRM and help desk

- A built-in CRM and help desk for each company: contacts, companies, tasks, deals with multiple pipelines and stages, tickets and internal notes.
- Also tags, custom fields, quick replies and message templates.
- More at [Connections](https://skiphold.com/connections).

## Telephony and messaging

- Manage phone numbers and connections: carrier numbers, Gemelos PBX, or SIP extension registration / SIP trunk to your PBX. See the [SIP Integration Overview](sip-integration.md).
- See live connection status.
- Set up [SMS](https://skiphold.com/integrations/sms) and [WhatsApp](https://skiphold.com/integrations/whatsapp) messaging, with A2P 10DLC compliance support for US business messaging.

## Native PBX, web phone and softphones

- Gemelos PBX, SkipHold's native hosted PBX.
- Branded desktop and mobile softphones, plus a built-in web phone.
- Video between internal extensions; external calls are audio-only.
- AI agents are reachable from users' softphone directory.

## Integrations and automations

- Automations with n8n and [Zapier MCP](https://skiphold.com/integrations/zapier-mcp).
- Appointment setting via connected calendars, n8n / Zapier MCP automations or your own APIs.
- Custom API tools and webhooks, built on request by the SkipHold team, to connect agents with modern or legacy systems.
- Browse all [SkipHold integrations](https://skiphold.com/integrations).

## Call logs, analytics and notifications

- Call logs with recordings, transcripts and AI summaries for each provider and company.
- Call metrics: total calls, successful calls and average duration.
- Email and SMS alerts for missed calls, voicemails, call summaries and transfers, all carrying your branding.

## Billing (providers)

- Choose a billing mode (details in [Provider & Partner Onboarding](partner-onboarding.md)):
  - **Platform Billing:** charges are processed on SkipHold's Stripe account, so the card transaction shows "SkipHold, LLC" on the cardholder's statement.
  - **Direct Billing:** you use your own Stripe account, so your own business name shows on the card statement.
- Both modes are fully white-label: proposals, invoices, statements and the portal carry your branding.
- Manage the product catalog and bundles, proposals, invoices, charges and payments.
- Reports cover receivables, revenue and signed proposals.
- Billing is powered by Stripe. More at [provider billing](https://skiphold.com/billing).

## Branding (providers)

- Logo, colors (light and dark mode), custom domain, and email sender name, reply-to and footer, with a live preview.

## Settings and My Account

- Company and provider settings.
- Your own profile and password.

## FAQ

**Who can monitor live calls?**
Providers and company admins.

**Can my staff take over a conversation from the AI?**
Yes. In Conversations, any voice, SMS or WhatsApp thread can be taken over by a person and handed back.

**Does SkipHold include a CRM and help desk?**
Yes. Connections is a built-in CRM and help desk with contacts, companies, tasks, deals and pipelines, tickets and internal notes.

**Can agents connect to our own business systems?**
Yes, through n8n and Zapier MCP automations. For anything more, the SkipHold team builds custom API tools and webhooks on request.

**Whose name appears on my customers' card statements?**
With Platform Billing, the card transaction shows "SkipHold, LLC". With Direct Billing, it shows your own business name. Proposals, invoices, statements and the portal carry your branding in both modes.

**Where are call recordings and transcripts?**
In Call Logs and Conversations, along with each call's AI summary.
