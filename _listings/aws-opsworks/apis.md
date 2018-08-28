---
name: AWS OpsWorks
x-slug: aws-opsworks
description: AWS OpsWorks is a configuration management service that uses Chef, an
  automation platform that treats server configurations as code. OpsWorks uses Chef
  to automate how servers are configured, deployed, and managed across your Amazon
  Elastic Compute Cloud (Amazon EC2) instances or on-premises compute environments.
  OpsWorks has two offerings, AWS Opsworks for Chef Automate, and AWS OpsWorks Stacks.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Load
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/apis.md
specificationVersion: "0.14"
apis:
- name: AWS OpsWorks API - Attach Elastic Load Balancer
  x-api-slug: actionattachelasticloadbalancer-get
  description: Attaches an Elastic Load Balancing load balancer to a specified layer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/actionattachelasticloadbalancer-get-openapi.md
- name: AWS OpsWorks API - Describe Elastic Load Balancers
  x-api-slug: actiondescribeelasticloadbalancers-get
  description: Describes a stack's Elastic Load Balancing instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/actiondescribeelasticloadbalancers-get-openapi.md
- name: AWS OpsWorks API - Describe Load Based Auto Scaling
  x-api-slug: actiondescribeloadbasedautoscaling-get
  description: Describes load-based auto scaling configurations for specified layers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/actiondescribeloadbasedautoscaling-get-openapi.md
- name: AWS OpsWorks API - Detach Elastic Load Balancer
  x-api-slug: actiondetachelasticloadbalancer-get
  description: Detaches a specified Elastic Load Balancing instance from its layer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/actiondetachelasticloadbalancer-get-openapi.md
- name: AWS OpsWorks API - Set Load Based Auto Scaling
  x-api-slug: actionsetloadbasedautoscaling-get
  description: Specify the load-based auto scaling configuration for a specified layer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Amazon Web Services, Orchestration, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/load/master/_listings/aws-opsworks/actionsetloadbasedautoscaling-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.marketplace.metering.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.opsworks.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/opsworks/latest/APIReference/Welcome.html
- type: x-website
  url: https://aws.amazon.com/opsworks/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---