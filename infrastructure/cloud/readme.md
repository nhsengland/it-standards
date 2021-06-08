# Cloud Infrastructure Standards

NHSEI's strategy calls for the use of Cloud Infrastructure before any consideration of physical infrastructure.

## Platforms

NHSEI are not prescriptive when it comes to the use of different cloud platforms.

However, there is a strong preference for using Microsoft Azure for the following reasons:

1) We have the most experience in our operational and architectural teams. Each of the global cloud platforms (Azure, AWS, Google) are incredibly complex environments with hundreds of services and extremely complex licensing. It is not feasible for us to manage services across multiple cloud platforms and so operational support for non-Azure deployments will need to be procured and managed separately.
2) We already have extensive licensing agreements that can be leveraged.
3) We have supporting logging, auditing and other management services that interface to Azure. These may need more work - both up-front development and ongoing support.

## Approach

In line with industry and government recommendations, the overall approach to the use of cloud infrastructure is to apply the following preferences:

1) SaaS - Software as a Service should be considered first
2) PaaS - Platform as a Service should be considered second
3) IaaS - Infrastructure as a Service should only be considered last

## Architectural Design

It is expected that any service being implemented using the Azure cloud platform MUST be set up using a "Virtual Data-Centre" approach. The same style of approach should also be applied to other platforms.

This approach calls for the service to be wrapped with a Resource Group. The wrapper encompasses one or more subscriptions, one or more Virtual Networks with associated firewalls and any other services required to deliver the service.

The virtual DC may encompass multiple environments if required or multiple virtual DC's could be encompassed by the Resource Group.

The outcome of this approach is that, if needed, all support and development could be outsourced if needed. Also, if necessary, the whole service could be moved to a different tenancy if needed.

_If a platform does not support this approach, architectural approval MUST be sought before any commitments are made._
