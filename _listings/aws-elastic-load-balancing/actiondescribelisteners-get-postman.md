{
  "info": {
    "name": "AWS Elastic Load Balancing API Describe Listeners",
    "_postman_id": "97cc190e-9ec6-4a85-bf1e-e64eed23670d",
    "description": "Describes the specified listeners or the listeners for the specified Application Load Balancer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "56eb3d8a-6a96-479f-b726-fa0757f65bb0",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceArns.member.N=ResourceArns.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "505248b1-8b54-45d4-84fd-f925f06e50b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Listeners",
      "item": [
        {
          "id": "49952bc6-0637-4e93-9c66-28f026ec147a",
          "name": "createListener",
          "request": {
            "url": "http://example.com/api/?Action=CreateListener?Certificates.member.N=Certificates.member.N&DefaultActions.member.N=DefaultActions.member.N&LoadBalancerArn=LoadBalancerArn&Port=Port&Protocol=Protocol&SslPolicy=SslPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a listener for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8836df2f-5a92-4409-8878-b16cbb827a94"
            }
          ]
        },
        {
          "id": "cc01c2d2-0128-452f-abce-d41e8f1be3f8",
          "name": "deleteListener",
          "request": {
            "url": "http://example.com/api/?Action=DeleteListener?ListenerArn=ListenerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "703995cb-5786-4551-9bec-c916b40fb572"
            }
          ]
        },
        {
          "id": "f1715851-c41f-4451-ba21-ac9666e3f1ff",
          "name": "describeListeners",
          "request": {
            "url": "http://example.com/api/?Action=DescribeListeners?ListenerArns.member.N=ListenerArns.member.N&LoadBalancerArn=LoadBalancerArn&Marker=Marker&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified listeners or the listeners for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a78581b-a2f5-4407-97ce-a6e43bd3688f"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "6f14fd49-c6fa-4c5d-9cca-b9074d38f0eb",
          "name": "createLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=CreateLoadBalancer?Name=Name&Scheme=Scheme&SecurityGroups.member.N=SecurityGroups.member.N&Subnets.member.N=Subnets.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "982db581-267c-4420-adb2-f4d505028ec9"
            }
          ]
        },
        {
          "id": "67de52e0-4c08-4ce0-af9e-5bb05577e36e",
          "name": "deleteLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLoadBalancer?LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Application Load Balancer and its attached listeners."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9525232-ef96-457a-a561-ad69962bbd4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "3c7108d9-dd9e-4244-a360-0cf2acff1cdd",
          "name": "createRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateRule?Actions.member.N=Actions.member.N&Conditions.member.N=Conditions.member.N&ListenerArn=ListenerArn&Priority=Priority",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a rule for the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "275d8a86-ff93-42a2-b96f-1e250daadfc4"
            }
          ]
        },
        {
          "id": "5f1e61af-dc31-4681-91c2-3d7d7ff03b38",
          "name": "deleteRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRule?RuleArn=RuleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d718a661-9956-439d-b3ec-96917e773ef5"
            }
          ]
        }
      ]
    },
    {
      "name": "Target Groups",
      "item": [
        {
          "id": "5a38b965-74f7-4e44-9d1e-2342101d5833",
          "name": "createTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateTargetGroup?HealthCheckIntervalSeconds=HealthCheckIntervalSeconds&HealthCheckPath=HealthCheckPath&HealthCheckPort=HealthCheckPort&HealthCheckProtocol=HealthCheckProtocol&HealthCheckTimeoutSeconds=HealthCheckTimeoutSeconds&HealthyThresholdCount=HealthyThresholdCount&Matcher=Matcher&Name=Name&Port=Port&Protocol=Protocol&UnhealthyThresholdCount=UnhealthyThresholdCount&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a154d7d4-1cbe-4c40-8049-9343317c15ea"
            }
          ]
        },
        {
          "id": "a88f6b90-62df-46bc-afb8-3816ee8d2b23",
          "name": "deleteTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTargetGroup?TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8344a4e-bba6-43d7-8152-b976378abbfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Targets",
      "item": [
        {
          "id": "cfb5fd51-bf06-48d6-b7a0-2820d5f6f401",
          "name": "deregisterTargets",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargets?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified targets from the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5f2596f-25c6-4f79-8b0b-e45c0ed64157"
            }
          ]
        }
      ]
    }
  ]
}