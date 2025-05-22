# Terraform-based-architecture-setup-for-achieving-High-availability
I've created a Terraform-based architecture setup for achieving 99.99% availability using AWS components like VPC, ALB, ECS Fargate, and multi-AZ design. This is a good foundation for production use.

Multi-AZ Deployment (Minimum for 99.99%)
Spread compute, databases, load balancers across multiple Availability Zones.
Ensure auto-scaling groups have cross-zone balancing.

Global DNS (Route 53 / Cloudflare) with geo-routing and failover.
Replicate databases across regions using logical or physical replication.
Use global load balancers or GSLBs for routing.

Graceful degradation: Serve limited features on partial failures
Health checks: Liveness, readiness, startup probes in K8s

kumar-abhishek.cloud
