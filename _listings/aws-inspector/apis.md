---
name: AWS Inspector
description: Amazon Inspector is an automated security assessment service that helps
  improve the security and compliance of applications deployed on AWS. Amazon Inspector
  automatically assesses applications for vulnerabilities or deviations from best
  practices. After performing an assessment, Amazon Inspector produces a detailed
  list of security findings prioritized by level of severity.nTo help you get started
  quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped
  to common security best practices and vulnerability definitions. Examples of built-in
  rules include checking for remote root login being enabled, or vulnerable software
  versions installed. These rules are regularly updated by AWS security researchers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Telemetry Metadata
- Tags For Resources
- Stack Network
- Security
- Rules Packages
- Resource Groups
- Findings
- Event Subscriptions
- Cross Account Access Roles
- Attributes To Findings
- Attributes From Findings
- Assessment Templates
- Assessment Targets
- Assessment Runs
- Assessment Run Agents
- Amazon Web Services
- Agents
created: "2018-03-10"
modified: "2018-03-10"
url: https://raw.githubusercontent.com/streamdata-gallery/agents/master/_listings/aws-inspector/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS Inspector API
  description: Amazon Inspector is an automated security assessment service that helps
    improve the security and compliance of applications deployed on AWS
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: ""
  baseURL: :///
  tags: Agents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/agents/master/_listings/aws-inspector/action-previewagents-get.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/inspector/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/inspector/faqs/
- type: x-getting-started
  url: https://docs.aws.amazon.com/inspector/latest/userguide/inspector_quickstart.html
- type: x-partners
  url: https://aws.amazon.com/inspector/partners/
- type: x-pricing
  url: https://aws.amazon.com/inspector/pricing/
- type: x-testimonials
  url: https://aws.amazon.com/inspector/customers/
- type: x-website
  url: https://aws.amazon.com/inspector/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---