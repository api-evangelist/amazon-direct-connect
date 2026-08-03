# Amazon Direct Connect

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Amazon Direct Connect links your internal network to an AWS Direct Connect location over a standard Ethernet fiber-optic cable. One end of the cable is connected to your router, the other to an AWS Direct Connect router. With this connection in place, you can create virtual interfaces directly to public AWS services, bypassing internet service providers in your network path.

- **URL:** https://aws.amazon.com/directconnect/
- **Run:** [![Run in Postman](https://run.pstmn.io/button.svg)](https://www.postman.com/api-evangelist/amazon-web-services/collection/)

**Tags:** Hybrid Cloud, Network Engineering, Dedicated Connection, AWS, Direct Connect

**Created:** 2026-04-19 | **Modified:** 2026-04-19

## APIs

- **Amazon Direct Connect API** - Amazon Direct Connect REST API for managing dedicated network connections, virtual interfaces, gateways, and link aggregation groups between on-premises networks and AWS.
  - **Base URL:** https://directconnect.us-east-1.amazonaws.com
  - **Version:** 2012-10-25
  - **OpenAPI:** [amazon-direct-connect-openapi.yaml](openapi/amazon-direct-connect-openapi.yaml)

### Common Properties

| Property | URL |
|---|---|
| Documentation | https://docs.aws.amazon.com/directconnect/latest/UserGuide/ |
| Getting Started | https://docs.aws.amazon.com/directconnect/latest/UserGuide/getting_started.html |
| Terms of Service | https://aws.amazon.com/service-terms/ |
| Privacy Policy | https://aws.amazon.com/privacy/ |
| Sign Up | https://portal.aws.amazon.com/billing/signup |
| GitHub Organization | https://github.com/aws |
| Status Page | https://health.aws.amazon.com/health/status |

### Features

| Feature | Description |
|---|---|
| Dedicated Connections | Physical Ethernet connections between customer premises and AWS at 1Gbps, 10Gbps, or 100Gbps |
| Virtual Interfaces | Logical network partitions supporting private, public, and transit interface types |
| Direct Connect Gateways | Virtual gateways enabling access to multiple VPCs across regions from a single connection |
| Link Aggregation Groups | Bundled connections providing increased bandwidth and redundancy |
| BGP Peering | Border Gateway Protocol sessions for dynamic routing on virtual interfaces |
| Hosted Connections | Connections provided by AWS Direct Connect partners for lower bandwidth requirements |

### Use Cases

| Use Case | Description |
|---|---|
| Hybrid Cloud Networking | Extend on-premises data centers into AWS with consistent, low-latency connectivity |
| Data Migration | Transfer large datasets to AWS with predictable bandwidth and without traversing the internet |
| Real-time Applications | Support latency-sensitive workloads requiring consistent network performance |
| Compliance | Meet regulatory requirements mandating private, dedicated network paths to cloud services |
| Multi-VPC Connectivity | Connect on-premises networks to multiple VPCs across regions via Direct Connect gateways |

### Integrations

| Integration | Description |
|---|---|
| Amazon VPC | Connect on-premises networks directly to Virtual Private Clouds via private virtual interfaces |
| AWS Transit Gateway | Access Transit Gateway from on-premises using transit virtual interfaces |
| AWS CloudFormation | Automate Direct Connect resource provisioning using infrastructure-as-code templates |
| AWS CloudTrail | Audit all Direct Connect API calls for compliance and security monitoring |
| Amazon Route 53 | Combine with private hosted zones for on-premises DNS resolution of AWS resources |

## Artifacts

### OpenAPI

| Name | Description | File |
|---|---|---|
| Amazon Direct Connect OpenAPI | OpenAPI 3.x specification for the Amazon Direct Connect API | [amazon-direct-connect-openapi.yaml](openapi/amazon-direct-connect-openapi.yaml) |

### JSON Schema

| Schema | Description | File |
|---|---|---|
| Connection | Dedicated physical connection between customer premises and AWS | [amazon-direct-connect-connection-schema.json](json-schema/amazon-direct-connect-connection-schema.json) |
| VirtualInterface | Logical network partition on a Direct Connect connection | [amazon-direct-connect-virtual-interface-schema.json](json-schema/amazon-direct-connect-virtual-interface-schema.json) |
| DirectConnectGateway | Virtual gateway enabling access to multiple VPCs across regions | [amazon-direct-connect-direct-connect-gateway-schema.json](json-schema/amazon-direct-connect-direct-connect-gateway-schema.json) |
| Lag | Link aggregation group bundling multiple connections | [amazon-direct-connect-lag-schema.json](json-schema/amazon-direct-connect-lag-schema.json) |
| Interconnect | Connection between AWS and a Direct Connect partner | [amazon-direct-connect-interconnect-schema.json](json-schema/amazon-direct-connect-interconnect-schema.json) |
| BGPPeer | BGP peering session on a virtual interface | [amazon-direct-connect-b-g-p-peer-schema.json](json-schema/amazon-direct-connect-b-g-p-peer-schema.json) |
| Location | Available Direct Connect colocation facility | [amazon-direct-connect-location-schema.json](json-schema/amazon-direct-connect-location-schema.json) |

### JSON Structure

| Schema | Description | File |
|---|---|---|
| Connection | JSON Structure for Connection | [amazon-direct-connect-connection-structure.json](json-structure/amazon-direct-connect-connection-structure.json) |
| VirtualInterface | JSON Structure for VirtualInterface | [amazon-direct-connect-virtual-interface-structure.json](json-structure/amazon-direct-connect-virtual-interface-structure.json) |
| DirectConnectGateway | JSON Structure for DirectConnectGateway | [amazon-direct-connect-direct-connect-gateway-structure.json](json-structure/amazon-direct-connect-direct-connect-gateway-structure.json) |

### JSON-LD

| Name | Description | File |
|---|---|---|
| Amazon Direct Connect Context | JSON-LD 1.1 context for Amazon Direct Connect types and properties | [amazon-direct-connect-context.jsonld](json-ld/amazon-direct-connect-context.jsonld) |

## Capabilities

### Shared API Definitions

| Name | Description | File |
|---|---|---|
| Amazon Direct Connect API | Shared Naftiko capability definition for Direct Connect API operations | [direct-connect-api.yaml](capabilities/shared/direct-connect-api.yaml) |

### Workflows

| Workflow | Description | Tools | Personas | File |
|---|---|---|---|---|
| Hybrid Network Connectivity | End-to-end hybrid network management using Amazon Direct Connect | 12 | Network Engineer, Cloud Architect | [hybrid-network-connectivity.yaml](capabilities/hybrid-network-connectivity.yaml) |

## Vocabulary

| Name | Description | File |
|---|---|---|
| Amazon Direct Connect Vocabulary | Unified taxonomy mapping operational and capability dimensions | [amazon-direct-connect-vocabulary.yaml](vocabulary/amazon-direct-connect-vocabulary.yaml) |

## Rules

| Name | Description | File |
|---|---|---|
| Amazon Direct Connect Spectral Rules | Spectral governance rules for Amazon Direct Connect API quality | [amazon-direct-connect-spectral-rules.yml](rules/amazon-direct-connect-spectral-rules.yml) |

## Maintainers

- Kin Lane - kin@apievangelist.com
