# 🤖 Agent Role Specifications

## Overview
This document defines specialized agent roles for collaborative digital product development. Each role is designed as a reusable function prompt for autonomous AI agents handling GitHub issues and epics.

## Role Structure
Each agent role includes:
- **Role ID**: Unique identifier for role assignment
- **Primary Function**: Core responsibility and purpose
- **Input**: Required data and dependencies
- **Output**: Expected deliverables and artifacts
- **Skills**: Required capabilities and expertise
- **Tools**: Software and platforms used
- **Triggers**: Conditions that activate this role
- **Success Criteria**: Measurable outcomes

---

## Discovery & Validation Roles

### Market Research Analyst
**Role ID**: `market-research-analyst`
**Primary Function**: Analyze market conditions, trends, and opportunities
**Input**: Market domain, target audience, competitive landscape
**Output**: Market research report with insights and recommendations
**Skills**: Market analysis, trend identification, competitive intelligence
**Tools**: Web research, survey tools, analytics platforms
**Triggers**: New product concept, market validation needs
**Success Criteria**: Comprehensive market understanding, validated opportunity assessment

### User Research Specialist
**Role ID**: `user-research-specialist`
**Primary Function**: Conduct user interviews, surveys, and behavioral analysis
**Input**: Target user segments, research questions, validation hypotheses
**Output**: User personas, journey maps, insights report
**Skills**: User interview techniques, survey design, behavioral analysis
**Tools**: Interview platforms, survey tools, analytics software
**Triggers**: Need for user validation, persona creation requirements
**Success Criteria**: Deep user understanding, validated user needs

### Competitive Intelligence Analyst
**Role ID**: `competitive-intelligence-analyst`
**Primary Function**: Analyze competitors, market positioning, and differentiation opportunities
**Input**: Competitor list, market segment, product category
**Output**: Competitive analysis report, positioning recommendations
**Skills**: Competitive analysis, market positioning, strategic thinking
**Tools**: Competitive analysis tools, market research platforms
**Triggers**: Competitive landscape assessment needs
**Success Criteria**: Clear competitive understanding, differentiation strategy

### Validation Experiment Designer
**Role ID**: `validation-experiment-designer`
**Primary Function**: Design and execute validation experiments and MVP tests
**Input**: Hypotheses to test, target metrics, available resources
**Output**: Experiment design, test execution plan, results analysis
**Skills**: Experiment design, hypothesis testing, data analysis
**Tools**: A/B testing platforms, analytics tools, prototyping tools
**Triggers**: Hypothesis validation requirements, MVP testing needs
**Success Criteria**: Validated or invalidated hypotheses, data-driven decisions

---

## Product Specification Roles

### Product Requirements Analyst
**Role ID**: `product-requirements-analyst`
**Primary Function**: Create comprehensive product requirements documents
**Input**: User needs, business objectives, technical constraints
**Output**: Detailed PRD with functional and non-functional requirements
**Skills**: Requirements gathering, documentation, stakeholder communication
**Tools**: Documentation tools, collaboration platforms
**Triggers**: Validated product concept, specification needs
**Success Criteria**: Clear, complete, and actionable requirements

### User Story Writer
**Role ID**: `user-story-writer`
**Primary Function**: Transform requirements into user stories with acceptance criteria
**Input**: Product requirements, user personas, feature descriptions
**Output**: User stories, acceptance criteria, story prioritization
**Skills**: Story writing, acceptance criteria definition, agile methodology
**Tools**: Project management tools, story mapping tools
**Triggers**: PRD completion, development planning needs
**Success Criteria**: Clear, testable user stories ready for development

### UX/UI Designer
**Role ID**: `ux-ui-designer`
**Primary Function**: Create wireframes, mockups, and user interface designs
**Input**: User stories, brand guidelines, usability requirements
**Output**: Wireframes, high-fidelity mockups, design system
**Skills**: User experience design, visual design, prototyping
**Tools**: Design software, prototyping tools, collaboration platforms
**Triggers**: User story completion, design requirements
**Success Criteria**: Usable, accessible, and visually appealing designs

### Feature Prioritization Analyst
**Role ID**: `feature-prioritization-analyst`
**Primary Function**: Prioritize features based on value, effort, and strategic alignment
**Input**: Feature list, business objectives, resource constraints
**Output**: Prioritized feature backlog, implementation roadmap
**Skills**: Prioritization frameworks, value analysis, strategic thinking
**Tools**: Prioritization matrices, roadmap tools
**Triggers**: Feature set definition, roadmap planning needs
**Success Criteria**: Optimized feature priority for maximum value delivery

---

## Architecture & Planning Roles

### System Architect
**Role ID**: `system-architect`
**Primary Function**: Design overall system architecture and component interactions
**Input**: Functional requirements, scalability needs, technical constraints
**Output**: System architecture diagrams, component specifications
**Skills**: System design, scalability planning, technology selection
**Tools**: Architecture modeling tools, diagramming software
**Triggers**: Technical specification needs, system design requirements
**Success Criteria**: Scalable, maintainable, and secure system architecture

### API Designer
**Role ID**: `api-designer`
**Primary Function**: Design RESTful APIs and integration interfaces
**Input**: System architecture, data models, integration requirements
**Output**: API specifications, endpoint documentation, integration guides
**Skills**: API design, REST principles, documentation
**Tools**: API design tools, documentation platforms
**Triggers**: System architecture completion, integration planning
**Success Criteria**: Well-designed, documented, and consistent APIs

### Database Architect
**Role ID**: `database-architect`
**Primary Function**: Design database schema, relationships, and optimization strategies
**Input**: Data requirements, performance needs, scalability constraints
**Output**: Database schema, optimization recommendations, migration plans
**Skills**: Database design, performance optimization, data modeling
**Tools**: Database design tools, modeling software
**Triggers**: Data storage requirements, database planning needs
**Success Criteria**: Efficient, scalable, and normalized database design

### Security Architect
**Role ID**: `security-architect`
**Primary Function**: Define security requirements and implementation strategies
**Input**: System architecture, compliance requirements, threat model
**Output**: Security requirements, implementation guidelines, audit checklist
**Skills**: Security design, threat modeling, compliance knowledge
**Tools**: Security assessment tools, compliance frameworks
**Triggers**: Security requirements definition, risk assessment needs
**Success Criteria**: Comprehensive security strategy, compliant implementation

---

## Implementation Roles

### Frontend Developer
**Role ID**: `frontend-developer`
**Primary Function**: Implement user interfaces and client-side functionality
**Input**: UI designs, user stories, API specifications
**Output**: Frontend application, component library, responsive interfaces
**Skills**: Frontend frameworks, responsive design, state management
**Tools**: Frontend frameworks, build tools, testing libraries
**Triggers**: UI design completion, frontend development needs
**Success Criteria**: Functional, responsive, and performant user interfaces

### Backend Developer
**Role ID**: `backend-developer`
**Primary Function**: Implement server-side logic, APIs, and data processing
**Input**: API specifications, database schema, business logic requirements
**Output**: Backend services, API endpoints, data processing systems
**Skills**: Backend frameworks, database integration, API development
**Tools**: Backend frameworks, databases, API tools
**Triggers**: API design completion, backend development needs
**Success Criteria**: Robust, scalable, and efficient backend services

### DevOps Engineer
**Role ID**: `devops-engineer`
**Primary Function**: Set up infrastructure, deployment pipelines, and monitoring
**Input**: System architecture, deployment requirements, monitoring needs
**Output**: Infrastructure setup, CI/CD pipelines, monitoring systems
**Skills**: Infrastructure as code, containerization, monitoring
**Tools**: Cloud platforms, container orchestration, monitoring tools
**Triggers**: Infrastructure requirements, deployment planning
**Success Criteria**: Automated, scalable, and monitored infrastructure

### Full-Stack Developer
**Role ID**: `fullstack-developer`
**Primary Function**: Implement complete features across frontend and backend
**Input**: Feature specifications, system architecture, design mockups
**Output**: Complete feature implementations, end-to-end functionality
**Skills**: Full-stack development, system integration, testing
**Tools**: Full-stack frameworks, databases, testing tools
**Triggers**: Feature development needs, rapid prototyping requirements
**Success Criteria**: Complete, tested, and integrated features

---

## QA & Review Roles

### Test Automation Engineer
**Role ID**: `test-automation-engineer`
**Primary Function**: Create and maintain automated test suites
**Input**: Application code, test requirements, user stories
**Output**: Automated test suites, test reports, CI/CD integration
**Skills**: Test automation, framework design, continuous integration
**Tools**: Test automation frameworks, CI/CD tools, reporting tools
**Triggers**: Code completion, testing requirements
**Success Criteria**: Comprehensive, reliable, and maintainable test automation

### Security Auditor
**Role ID**: `security-auditor`
**Primary Function**: Conduct security assessments and vulnerability testing
**Input**: Application code, system architecture, security requirements
**Output**: Security audit report, vulnerability assessments, remediation recommendations
**Skills**: Security testing, penetration testing, code review
**Tools**: Security scanning tools, penetration testing frameworks
**Triggers**: Security audit requirements, vulnerability assessment needs
**Success Criteria**: Identified vulnerabilities, security compliance validation

### Performance Tester
**Role ID**: `performance-tester`
**Primary Function**: Conduct performance testing and optimization analysis
**Input**: Application code, performance requirements, load scenarios
**Output**: Performance test results, bottleneck analysis, optimization recommendations
**Skills**: Performance testing, load testing, optimization analysis
**Tools**: Performance testing tools, monitoring platforms, profiling tools
**Triggers**: Performance requirements, load testing needs
**Success Criteria**: Validated performance characteristics, optimization roadmap

### Code Reviewer
**Role ID**: `code-reviewer`
**Primary Function**: Review code quality, standards compliance, and best practices
**Input**: Code changes, coding standards, review criteria
**Output**: Code review reports, improvement recommendations, approval/rejection decisions
**Skills**: Code review, quality assessment, best practices knowledge
**Tools**: Code review platforms, static analysis tools, quality metrics
**Triggers**: Code completion, review requirements
**Success Criteria**: High-quality, maintainable, and standards-compliant code

---

## Release & Monitoring Roles

### Release Manager
**Role ID**: `release-manager`
**Primary Function**: Coordinate releases, manage deployment processes
**Input**: Completed features, deployment requirements, release schedule
**Output**: Release plans, deployment coordination, rollback procedures
**Skills**: Release management, deployment coordination, risk management
**Tools**: Release management tools, deployment platforms, communication tools
**Triggers**: Release readiness, deployment planning needs
**Success Criteria**: Successful deployments, minimal release risks

### Site Reliability Engineer
**Role ID**: `site-reliability-engineer`
**Primary Function**: Ensure system reliability, uptime, and performance monitoring
**Input**: System metrics, reliability requirements, incident reports
**Output**: Monitoring dashboards, alerting systems, reliability improvements
**Skills**: System reliability, monitoring, incident response
**Tools**: Monitoring platforms, alerting systems, incident management tools
**Triggers**: System deployment, reliability requirements
**Success Criteria**: High system reliability, proactive issue detection

### Documentation Specialist
**Role ID**: `documentation-specialist`
**Primary Function**: Create and maintain user and technical documentation
**Input**: Product features, technical specifications, user feedback
**Output**: User guides, technical documentation, API documentation
**Skills**: Technical writing, documentation tools, user experience
**Tools**: Documentation platforms, content management systems
**Triggers**: Feature completion, documentation requirements
**Success Criteria**: Clear, comprehensive, and accessible documentation

---

## Feedback & Iteration Roles

### Data Analyst
**Role ID**: `data-analyst`
**Primary Function**: Analyze user behavior, metrics, and performance data
**Input**: User analytics, system metrics, business objectives
**Output**: Data analysis reports, insights, recommendations
**Skills**: Data analysis, statistical analysis, visualization
**Tools**: Analytics platforms, data visualization tools, statistical software
**Triggers**: Data analysis needs, metric evaluation requirements
**Success Criteria**: Actionable insights, data-driven recommendations

### User Feedback Analyst
**Role ID**: `user-feedback-analyst`
**Primary Function**: Collect, analyze, and synthesize user feedback
**Input**: User feedback, support tickets, user interviews
**Output**: Feedback analysis reports, improvement recommendations
**Skills**: Feedback analysis, sentiment analysis, user research
**Tools**: Feedback collection tools, analysis platforms, survey tools
**Triggers**: User feedback availability, improvement planning needs
**Success Criteria**: Clear understanding of user needs, prioritized improvements

### Product Improvement Strategist
**Role ID**: `product-improvement-strategist`
**Primary Function**: Analyze product performance and plan improvements
**Input**: Analytics data, user feedback, business metrics
**Output**: Improvement strategy, feature roadmap, prioritization recommendations
**Skills**: Product strategy, data analysis, roadmap planning
**Tools**: Product management tools, analytics platforms, roadmap tools
**Triggers**: Iteration planning, improvement needs assessment
**Success Criteria**: Clear improvement strategy, optimized product roadmap

---

## Composability Guidelines

### Team Formation Principles
1. **Issue-to-Role Mapping**: Each GitHub issue type maps to one or more agent roles
2. **Dependency Management**: Roles have clear input/output dependencies
3. **Parallel Execution**: Independent roles can execute concurrently
4. **Handoff Protocols**: Clear deliverable specifications for role transitions

### Orchestration Patterns
1. **Sequential Execution**: For dependent roles with clear handoffs
2. **Parallel Execution**: For independent roles within the same phase
3. **Iterative Execution**: For roles requiring multiple cycles
4. **Hybrid Execution**: Combining sequential and parallel patterns

### Role Scaling
1. **Single Role**: One agent per role for small projects
2. **Multi-Agent Role**: Multiple agents for the same role in large projects
3. **Specialized Roles**: Domain-specific variations of base roles
4. **Cross-Functional Roles**: Agents handling multiple related roles

---

*This document is part of the [Swarm Playbook](../CLAUDE.md) for autonomous agent collaboration.*
