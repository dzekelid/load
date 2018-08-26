{
  "info": {
    "name": "AWS Elastic Load Balancing API Create Listener",
    "_postman_id": "7a5a8a28-b470-4c4b-875b-abd0b255fc34",
    "description": "Creates a listener for the specified Application Load Balancer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "aad9ce9c-0621-434c-925f-b417cd39746d",
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
              "id": "b4f59621-608b-4f89-bb56-a92b44fb00d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Listeners",
      "item": [
        {
          "id": "79171db7-9d1a-40ca-ae2b-acbc7ca6b6ac",
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
              "id": "b2e6cc35-14f6-4bf6-b841-d20b85d10d1a"
            }
          ]
        }
      ]
    }
  ]
}