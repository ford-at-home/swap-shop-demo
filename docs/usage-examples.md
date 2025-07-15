# 📖 Usage Examples

## Overview
This document provides real-world examples of how to use the swarm playbook for autonomous agent collaboration across different project types and scenarios.

---

## Example 1: User Authentication System

### Epic: "Build User Authentication System"

**Issues Generated**:
- `research: auth-best-practices`
- `spec: auth-requirements`
- `design: auth-ui-mockups`
- `architecture: auth-system-design`
- `feature: auth-frontend`
- `feature: auth-backend`
- `test: auth-test-suite`
- `security: auth-security-audit`
- `deployment: auth-production-release`

**Agent Team**:
- **User Research Specialist** → analyze authentication UX patterns
- **Product Requirements Analyst** → define auth requirements
- **UX/UI Designer** → create login/signup interfaces
- **System Architect** → design auth system architecture
- **Security Architect** → define security requirements
- **Frontend Developer** → implement auth UI
- **Backend Developer** → implement auth services
- **Test Automation Engineer** → create auth test suite
- **Security Auditor** → conduct security review
- **Release Manager** → coordinate deployment

**Execution Flow**:
1. **Research Phase**: User Research Specialist analyzes auth UX patterns
2. **Specification Phase**: Product Requirements Analyst creates auth PRD
3. **Design Phase**: UX/UI Designer creates interface mockups
4. **Architecture Phase**: System & Security Architects design secure auth system
5. **Implementation Phase**: Frontend & Backend Developers build auth features
6. **QA Phase**: Test Automation Engineer & Security Auditor validate implementation
7. **Release Phase**: Release Manager coordinates production deployment

---

## Example 2: E-commerce Platform

### Epic: "Build E-commerce Platform MVP"

**Phase Breakdown**:

#### Phase 1: Discovery & Validation (2 weeks)
- **Market Research Analyst**: E-commerce market analysis
- **User Research Specialist**: Customer journey mapping
- **Competitive Intelligence Analyst**: Competitor feature analysis
- **Validation Experiment Designer**: MVP validation experiments

#### Phase 2: Product Specification (3 weeks)
- **Product Requirements Analyst**: E-commerce platform PRD
- **User Story Writer**: Customer and admin user stories
- **UX/UI Designer**: Shopping experience wireframes
- **Feature Prioritization Analyst**: MVP feature prioritization

#### Phase 3: Architecture & Planning (2 weeks)
- **System Architect**: Microservices architecture design
- **API Designer**: Product, cart, and payment APIs
- **Database Architect**: Product catalog and order schema
- **Security Architect**: Payment security requirements

#### Phase 4: Implementation (8 weeks)
- **Frontend Developer**: Customer-facing web app
- **Backend Developer**: Product and order services
- **DevOps Engineer**: AWS infrastructure setup
- **Full-Stack Developer**: Admin dashboard

#### Phase 5: QA & Review (2 weeks)
- **Test Automation Engineer**: E2E shopping flow tests
- **Security Auditor**: Payment security audit
- **Performance Tester**: Load testing for traffic spikes
- **Code Reviewer**: Code quality and standards review

#### Phase 6: Release & Monitoring (1 week)
- **Release Manager**: Production deployment coordination
- **Site Reliability Engineer**: Monitoring and alerting setup
- **Documentation Specialist**: User guides and API docs

#### Phase 7: Feedback & Iteration (Ongoing)
- **Data Analyst**: Customer behavior analysis
- **User Feedback Analyst**: Support ticket analysis
- **Product Improvement Strategist**: Feature roadmap planning

---

## Example 3: Mobile App Development

### Epic: "Build Cross-Platform Mobile App"

**Specialized Roles**:
- **Mobile UX Designer**: Native mobile interface design
- **React Native Developer**: Cross-platform implementation
- **Mobile DevOps Engineer**: App store deployment
- **Mobile Test Engineer**: Device-specific testing
- **Performance Optimization Specialist**: Mobile performance tuning

**Execution Pattern**:
1. **Parallel Research**: Market + User + Competitive analysis
2. **Sequential Specification**: Requirements → Stories → Design
3. **Parallel Implementation**: iOS + Android + Backend
4. **Iterative Testing**: Device testing + Performance optimization
5. **Staged Release**: Beta testing → App store approval → Production

---

## Example 4: API-First SaaS Platform

### Epic: "Build API-First SaaS Platform"

**API-Centric Roles**:
- **API Product Manager**: API strategy and roadmap
- **API Designer**: RESTful API specification
- **API Developer**: Backend API implementation
- **API Documentation Specialist**: Developer documentation
- **API Security Engineer**: Authentication and authorization
- **API Performance Engineer**: Rate limiting and optimization

**Execution Pattern**:
1. **API-First Design**: Design APIs before implementation
2. **Contract Testing**: Mock APIs for frontend development
3. **Parallel Development**: Backend + Frontend + Documentation
4. **API Versioning**: Backward compatibility management
5. **Developer Experience**: SDK creation and sample apps

---

## Example 5: Data-Driven Product

### Epic: "Build Analytics Dashboard"

**Data-Focused Roles**:
- **Data Architect**: Data pipeline design
- **Data Engineer**: ETL pipeline implementation
- **Frontend Data Visualization Developer**: Dashboard implementation
- **Data Analyst**: Metrics definition and analysis
- **Data Security Engineer**: Data privacy and compliance

**Execution Pattern**:
1. **Data Discovery**: Data source identification and analysis
2. **Pipeline Design**: ETL architecture and data flow
3. **Parallel Implementation**: Data pipeline + Dashboard UI
4. **Data Quality**: Testing and validation
5. **Analytics Setup**: Monitoring and alerting

---

## Team Composition Patterns

### Small Project (1-3 Agents)
- **Full-Stack Developer**: Implementation across all layers
- **DevOps Engineer**: Infrastructure and deployment
- **UX/UI Designer**: User experience and interface

### Medium Project (4-8 Agents)
- **Product Requirements Analyst**: Requirements and planning
- **Frontend Developer**: User interface implementation
- **Backend Developer**: Server-side logic and APIs
- **Database Architect**: Data modeling and optimization
- **Test Automation Engineer**: Quality assurance
- **DevOps Engineer**: Infrastructure and deployment
- **Security Architect**: Security requirements
- **Release Manager**: Deployment coordination

### Large Project (8+ Agents)
- **Complete Phase Teams**: Dedicated agents for each phase
- **Specialized Roles**: Domain-specific expertise
- **Cross-Functional Coordination**: Integration specialists
- **Quality Assurance**: Multiple testing specialists
- **Release Coordination**: Multiple deployment managers

---

## Execution Patterns

### Sequential Execution
Best for projects with strong dependencies and clear handoffs:
```
Discovery → Specification → Architecture → Implementation → QA → Release
```

### Parallel Execution
Best for projects with independent workstreams:
```
Discovery + Specification (parallel)
↓
Architecture (depends on both)
↓
Frontend + Backend + DevOps (parallel)
↓
Testing + Documentation (parallel)
```

### Iterative Execution
Best for projects requiring multiple cycles:
```
MVP Phase:
Discovery → Specification → Implementation → Release
↓
Enhancement Phase:
Feedback → Specification → Implementation → Release
↓
Scale Phase:
Analysis → Architecture → Implementation → Release
```

### Hybrid Execution
Best for complex projects with mixed dependencies:
```
Phase 1: Discovery + Competitive Analysis (parallel)
Phase 2: Specification (sequential)
Phase 3: Architecture + Security (parallel)
Phase 4: Frontend + Backend + DevOps (parallel)
Phase 5: Testing + Documentation (parallel)
Phase 6: Release (sequential)
Phase 7: Feedback + Analytics (parallel)
```

---

## Best Practices

### 1. Role Assignment
- Match agent capabilities to role requirements
- Consider workload distribution across agents
- Plan for role dependencies and handoffs
- Have backup agents for critical roles

### 2. Communication Protocols
- Use GitHub issues for all work coordination
- Establish clear handoff criteria between roles
- Document decisions and rationale
- Regular status updates and progress reporting

### 3. Quality Gates
- Define clear acceptance criteria for each role
- Implement automated testing and validation
- Regular code reviews and quality checks
- Continuous monitoring and feedback loops

### 4. Risk Management
- Identify critical path dependencies
- Plan for agent failures and replacements
- Have escalation procedures for blockers
- Regular risk assessment and mitigation

### 5. Continuous Improvement
- Collect metrics on agent performance
- Analyze workflow efficiency and bottlenecks
- Iterate on role definitions and processes
- Share learnings across projects

---

## Troubleshooting Common Issues

### Issue: Agent Role Conflicts
**Symptoms**: Multiple agents working on overlapping tasks
**Solution**: Clarify role boundaries and dependencies
**Prevention**: Better issue scoping and role assignment

### Issue: Blocking Dependencies
**Symptoms**: Agents waiting for inputs from other agents
**Solution**: Implement parallel work streams where possible
**Prevention**: Better dependency mapping and scheduling

### Issue: Quality Issues
**Symptoms**: Bugs, security vulnerabilities, performance problems
**Solution**: Strengthen quality gates and testing
**Prevention**: Better role specialization and review processes

### Issue: Communication Gaps
**Symptoms**: Missing requirements, unclear specifications
**Solution**: Improve handoff documentation and validation
**Prevention**: Better communication protocols and templates

---

*This document is part of the [Swarm Playbook](../CLAUDE.md) for autonomous agent collaboration.*
