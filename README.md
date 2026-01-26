# MealBox – Auth Service

## Purpose
Auth Service handles user authentication and authorization for the MealBox platform.

## Responsibilities
- User signup
- User login
- JWT token generation and validation

## Technology
- Language: Java (Spring Boot)
- Build Tool: Maven
- Container: Docker (non-root)
- Orchestration: Kubernetes / OpenShift

## API Endpoints (Initial)
- POST /auth/signup
- POST /auth/login
- GET  /auth/health

## Port
- Application Port: 8080

## Health Checks
- Liveness: /auth/health
- Readiness: /auth/health

## CI/CD Expectations
- Unit tests must pass
- SonarQube quality gate must pass
- Trivy scan must not fail on CRITICAL vulnerabilities
- Docker image must be non-root
- Deployment must pass health checks

## Environments
- dev: kind
- stage: OpenShift Sandbox
- prod: AWS (logical)

## Maintainer
- DevOps Practice Project – MealBox
