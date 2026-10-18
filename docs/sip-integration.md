---
title: "SIP AI Voice Agent Integration: NetSapiens, 3CX, FreePBX | SkipHold Docs"
description: "Connect the SkipHold SIP AI voice agent to NetSapiens, Thirdlane, 3CX, FreePBX and other SIP platforms or carriers, by SIP extension registration or SIP trunk."
---

# SIP AI Voice Agent Integration Overview

SkipHold's SIP AI voice agents connect to the phone systems you already run. Calls reach SkipHold AI agents through the SkipHold SIP Bridge, which runs on the SkipHold Telephony servers. For the big picture, see [how SkipHold works](https://skiphold.com/how-it-works).

## How calls flow from your PBX to the AI agent

    Carrier / Gemelos PBX / your PBX  ──►  SkipHold SIP Bridge  ──►  SkipHold AI agent
                                                     ▲                         │
                                                     └──── transfers ──────────┘

1. A call arrives on a carrier number, on Gemelos PBX, or on your PBX / UCaaS platform.
2. The SkipHold SIP Bridge receives it and sends it to the AI agent assigned to that line.
3. The caller's ID is passed through, so the agent knows who's calling.
4. When the agent transfers the call, it goes back through the PBX it came from. This keeps your extensions, ring groups and queues in the loop. See [AI warm transfers](https://skiphold.com/warm-transfers).

## Connection methods: SIP extension registration or SIP trunk

- **SIP extension registration:** the SkipHold SIP Bridge registers on your PBX as a standard SIP extension. To your PBX, the AI agent looks like any other phone. Route calls to that extension, for example as the main number's destination, an after-hours route or an overflow route.
- **SIP trunk:** calls are delivered to SkipHold over a SIP trunk, from a carrier or from your platform.

## Supported PBX, UCaaS and carrier platforms

**Native**
- [Gemelos PBX](https://skiphold.com/native-pbx): SkipHold's own hosted PBX. Tenants link directly to SkipHold companies.

**API integration (beta)**
- [NetSapiens](https://skiphold.com/sip-ai-for-netsapiens)

**SIP interoperability** (third-party PBX / UCaaS platforms)
- [AI receptionist for NetSapiens](https://skiphold.com/integrations/netsapiens)
- [AI receptionist for Thirdlane](https://skiphold.com/integrations/thirdlane)
- [AI receptionist for 3CX](https://skiphold.com/integrations/3cx)
- [AI receptionist for FreePBX](https://skiphold.com/integrations/freepbx)
- [AI receptionist for FusionPBX](https://skiphold.com/integrations/fusionpbx)
- other standards-based SIP platforms

**Carriers**
- [Twilio](https://skiphold.com/integrations/twilio), Telnyx, Bandwidth and other carriers.

All integrations: [SkipHold integrations](https://skiphold.com/integrations).

## What we need from you

For SIP extension registration:
- your PBX's SIP domain (realm)
- the SIP proxy or outbound proxy, if your platform uses one separate from the domain
- the extension number set aside for the AI agent
- that extension's SIP username and password

For a SIP trunk: your trunk details and the numbers to route to SkipHold.

## Platform notes for hosted and self-hosted PBXs

- **Hosted UCaaS platforms** (for example NetSapiens) usually use a shared core proxy that's different from the tenant's SIP domain. Give us both.
- **Self-hosted PBXs** (for example FreePBX) usually use the same host for domain and proxy, sometimes with a port.
- **Number formats:** some PBXs reject destination numbers with a leading "+". SkipHold handles this per platform.
- **Caller ID:** some platforms always present their own trunk caller ID on outbound legs, whatever SkipHold sends.

## Checking and troubleshooting a SIP connection

In the Admin Portal, open **Telephony** to see each connection's status. If a connection isn't active:
- **Registration fails:** check the extension's SIP username and password.
- **No traffic reaches the PBX:** check the proxy / outbound proxy value.
- **Calls ring but transfers fail:** check the number format and your PBX's transfer permissions.

Provisioning and status checks are handled by the SkipHold Telephony API. Need help? Email info@skiphold.com with your organization name, PBX platform, a short description of the issue, and any timestamps or call IDs.

Next: [Provider & Partner Onboarding](partner-onboarding.md) · [Admin Portal Guide](admin-portal-guide.md)

## FAQ

**Does SkipHold work with NetSapiens?**
Yes. SkipHold works with NetSapiens over SIP and also offers a NetSapiens API integration (beta). See [SIP AI for NetSapiens](https://skiphold.com/sip-ai-for-netsapiens).

**Can I add an AI receptionist to 3CX or FreePBX?**
Yes. Register the SkipHold SIP Bridge as an extension on your 3CX or FreePBX system, then route calls to it.

**Should I use extension registration or a SIP trunk?**
Extension registration is the quickest way to add AI to an existing PBX, with no trunk changes. Use a SIP trunk when calls come straight from a carrier or when your platform prefers trunk delivery.

**Is the caller's ID passed to the AI agent?**
Yes. The original caller ID is passed through, so the agent and any transfer destination can see who's calling.

**Do transfers still use my PBX?**
Yes. Transfers go back through the PBX the call came from, so your extensions, ring groups and queues keep working.
