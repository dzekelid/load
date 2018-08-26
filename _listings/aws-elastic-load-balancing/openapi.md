---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateListener:
    get:
      summary: Create Listener
      description: Creates a listener for the specified Application Load Balancer.
      operationId: createListener
      x-api-path-slug: actioncreatelistener-get
      parameters:
      - in: query
        name: Certificates.member.N
        description: The SSL server certificate
        type: string
      - in: query
        name: DefaultActions.member.N
        description: The default action for the listener
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Port
        description: The port on which the load balancer is listening
        type: string
      - in: query
        name: Protocol
        description: The protocol for connections from clients to the load balancer
        type: string
      - in: query
        name: SslPolicy
        description: The security policy that defines which ciphers and protocols
          are supported
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=CreateLoadBalancer:
    get:
      summary: Create Load Balancer
      description: Creates an Application Load Balancer.
      operationId: createLoadBalancer
      x-api-path-slug: actioncreateloadbalancer-get
      parameters:
      - in: query
        name: Name
        description: The name of the load balancer
        type: string
      - in: query
        name: Scheme
        description: The nodes of an Internet-facing load balancer have public IP
          addresses
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: The IDs of the security groups to assign to the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets to attach to the load balancer
        type: string
      - in: query
        name: Tags.member.N
        description: One or more tags to assign to the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DeleteLoadBalancer:
    get:
      summary: Delete Load Balancer
      description: Deletes the specified Application Load Balancer and its attached
        listeners.
      operationId: deleteLoadBalancer
      x-api-path-slug: actiondeleteloadbalancer-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeListeners:
    get:
      summary: Describe Listeners
      description: Describes the specified listeners or the listeners for the specified
        Application Load Balancer.
      operationId: describeListeners
      x-api-path-slug: actiondescribelisteners-get
      parameters:
      - in: query
        name: ListenerArns.member.N
        description: The Amazon Resource Names (ARN) of the listeners
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=DescribeLoadBalancerAttributes:
    get:
      summary: Describe Load Balancer Attributes
      description: Describes the attributes for the specified Application Load Balancer.
      operationId: describeLoadBalancerAttributes
      x-api-path-slug: actiondescribeloadbalancerattributes-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeLoadBalancers:
    get:
      summary: Describe Load Balancers
      description: Describes the specified Application Load Balancers or all of your
        Application Load Balancers.
      operationId: describeLoadBalancers
      x-api-path-slug: actiondescribeloadbalancers-get
      parameters:
      - in: query
        name: LoadBalancerArns.member.N
        description: The Amazon Resource Names (ARN) of the load balancers
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Names.member.N
        description: The names of the load balancers
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=ModifyLoadBalancerAttributes:
    get:
      summary: Modify Load Balancer Attributes
      description: Modifies the specified attributes of the specified Application
        Load Balancer.
      operationId: modifyLoadBalancerAttributes
      x-api-path-slug: actionmodifyloadbalancerattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The load balancer attributes
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
---