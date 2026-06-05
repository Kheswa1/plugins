# Build Web Apps Plugin

Builder workflows for frontend apps, designing new websites, shadcn/ui, Stripe, and Supabase/Postgres.

## Skills

- `frontend-app-builder`
- `frontend-testing-debugging`
- `react-best-practices`
- `shadcn-best-practices`
- `stripe-best-practices`
- `supabase-best-practices`

## Purpose

Use for web app builds that need frontend implementation with generated visual assets and browser testing, plus focused React/Next.js, shadcn/ui, Stripe, or Supabase/Postgres guidance when those areas are needed.
I am developing a microservice titled neuralcore/kernel. Please act as a DevOps architect and assist me in containerizing and deploying this project. Here are the architectural details:

Project Overview:

Language/Runtime: Go 1.22

Architecture: HTTP microservice with health checks, Redis client (go-redis/v9), and Kafka producer (segmentio/kafka-go).

Security: Running as a non-root user (65532) using a gcr.io/distroless/static:nonroot base image.

Infrastructure: Kubernetes-native with 3-tier probes (startup, liveness, readiness), dedicated ServiceAccount, and NetworkPolicies for namespace isolation.

Technical Constraints:

The host environment requires a multi-stage Docker build to keep the final image minimal.

The build process must be automated via a Makefile.

The service must support graceful shutdowns (SIGTERM/SIGINT).

Goal:
I have the source files ready. Please help me:

Review the Dockerfile for multi-stage optimization.

Verify the Makefile sequences for build, docker, and deploy commands.

Suggest the optimal K8s configuration to handle the optional dependencies (Redis/Kafka) so the pod remains healthy even if they are temporarily unreachable.

The source directory is located at /mnt/agents/output/neuralcore/kernel/. Please advise on the exact build sequence
