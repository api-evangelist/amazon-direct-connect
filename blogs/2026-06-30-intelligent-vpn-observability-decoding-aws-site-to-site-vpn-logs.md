---
title: "Intelligent VPN observability: Decoding AWS Site-to-Site VPN logs"
url: "https://aws.amazon.com/blogs/networking-and-content-delivery/intelligent-vpn-observability-decoding-aws-site-to-site-vpn-logs/"
date: "2026-06-30"
author: "Ravi Kulkarni"
feed_url: "https://aws.amazon.com/blogs/networking-and-content-delivery/feed/"
---
This article presents an automated observability pipeline for AWS Site-to-Site VPN connections that detects anomalies and analyzes BGP and IKE logs using Amazon Bedrock. The serverless architecture uses CloudWatch Logs subscription filters, Amazon SQS FIFO for deduplication, and Amazon SNS for email delivery, covering troubleshooting scenarios like prefix quota violations, AS path loops, connection collisions, and IKE tunnel failures.
