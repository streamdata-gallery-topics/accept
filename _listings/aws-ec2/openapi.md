swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptReservedInstancesExchangeQuote:
    get:
      summary: Accept Reserved Instances Exchange Quote
      description: Accepts the Convertible Reserved Instance exchange quote described
        in the GetReservedInstancesExchangeQuote call.
      operationId: acceptreservedinstancesexchangequote
      x-api-path-slug: actionacceptreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ReservedInstancesListingId
        description: The ID of the Reserved Instance listing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=AcceptVpcPeeringConnection:
    get:
      summary: Accept Vpc Peering Connection
      description: Accept a VPC peering connection request.
      operationId: acceptvpcpeeringconnection
      x-api-path-slug: actionacceptvpcpeeringconnection-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: PeerOwnerId
        description: The AWS account ID of the owner of the peer VPC
        type: string
      - in: query
        name: PeerVpcId
        description: The ID of the VPC with which you are creating the VPC peering
          connection
        type: string
      - in: query
        name: VpcId
        description: The ID of the requester VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection