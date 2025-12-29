# ADR-001: Choice of Modular Monolith Architecture

## Status
Accepted

## Context
The Complaint Management System must support multiple user roles,
multi-tenancy, scalability, and security while remaining feasible
to implement as a proof of concept for academic assessment.

## Decision
A modular monolith architecture using Node.js and Express was selected.
The system is deployed as a single application but internally organised
into clearly defined modules such as complaints, users, tenants,
notifications, and reporting.

## Alternatives Considered
- Microservices architecture
- Service-oriented architecture (SOA)
- Traditional layered monolith

## Consequences
- Easier development and deployment
- Clear internal boundaries between modules
- Reduced operational complexity for a proof of concept
- Architecture can evolve into microservices in the future if required

