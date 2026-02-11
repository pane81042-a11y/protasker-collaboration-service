# ProTasker Collaboration Service

## Overview

The ProTasker Collaboration Service is a serverless backend microservice responsible for managing team collaboration within projects.

It handles team invitations, role assignments, and membership control while enforcing secure access using Amazon Cognito JWT authorization.

This service operates fully serverless within the AWS Always Free Tier.

---

## Architecture

- AWS Lambda (Collaboration logic)
- Amazon API Gateway (REST endpoints)
- Amazon DynamoDB (Membership and role storage)
- Amazon Cognito (Authentication and JWT validation)
- IAM roles with least privilege access

---

## Responsibilities

- Invite users to projects
- Assign and update roles
- Manage project membership
- Validate permissions for collaborative actions
- Enforce user-scoped access control

---

## Security

- Cognito User Pool integration
- JWT-based authorization via API Gateway
- Role-based access control
- Membership validation
- IAM-based permission boundaries

---

## Deployment Model

Deployed as an independent microservice within a distributed serverless architecture.

All API requests require a valid Cognito access token in the Authorization header.

---

## Tech Stack

- Node.js
- AWS Lambda
- DynamoDB
- API Gateway
- Amazon Cognito

---

## Status

Initial architecture and collaboration service scaffolding.
