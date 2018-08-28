---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Set Load Based Auto Scaling
  version: 1.0.0
  description: Specify the load-based auto scaling configuration for a specified layer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachElasticLoadBalancer:
    get:
      summary: Attach Elastic Load Balancer
      description: Attaches an Elastic Load Balancing load balancer to a specified
        layer.
      operationId: attachElasticLoadBalancer
      x-api-path-slug: actionattachelasticloadbalancer-get
      parameters:
      - in: query
        name: ElasticLoadBalancerName
        description: The Elastic Load Balancing instances name
        type: string
      - in: query
        name: LayerId
        description: The ID of the layer that the Elastic Load Balancing instance
          is to be attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attach
      - Elastic
      - Load
      - Balancer
  /?Action=DescribeElasticLoadBalancers:
    get:
      summary: Describe Elastic Load Balancers
      description: Describes a stack's Elastic Load Balancing instances.
      operationId: describeElasticLoadBalancers
      x-api-path-slug: actiondescribeelasticloadbalancers-get
      parameters:
      - in: query
        name: LayerIds
        description: A list of layer IDs
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Elastic
      - Load
      - Balancers
  /?Action=DescribeLoadBasedAutoScaling:
    get:
      summary: Describe Load Based Auto Scaling
      description: Describes load-based auto scaling configurations for specified
        layers.
      operationId: describeLoadBasedAutoScaling
      x-api-path-slug: actiondescribeloadbasedautoscaling-get
      parameters:
      - in: query
        name: LayerIds
        description: An array of layer IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Load
      - Based
      - Auto
      - Scaling
  /?Action=DetachElasticLoadBalancer:
    get:
      summary: Detach Elastic Load Balancer
      description: Detaches a specified Elastic Load Balancing instance from its layer.
      operationId: detachElasticLoadBalancer
      x-api-path-slug: actiondetachelasticloadbalancer-get
      parameters:
      - in: query
        name: ElasticLoadBalancerName
        description: The Elastic Load Balancing instances name
        type: string
      - in: query
        name: LayerId
        description: The ID of the layer that the Elastic Load Balancing instance
          is attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Elastic
      - Load
      - Balancer
  /?Action=SetLoadBasedAutoScaling:
    get:
      summary: Set Load Based Auto Scaling
      description: Specify the load-based auto scaling configuration for a specified
        layer.
      operationId: setLoadBasedAutoScaling
      x-api-path-slug: actionsetloadbasedautoscaling-get
      parameters:
      - in: query
        name: DownScaling
        description: An AutoScalingThresholds object with the downscaling threshold
          configuration
        type: string
      - in: query
        name: Enable
        description: Enables load-based auto scaling for the layer
        type: string
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      - in: query
        name: UpScaling
        description: An AutoScalingThresholds object with the upscaling threshold
          configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Load
      - Based
      - Auto
      - Scaling
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---