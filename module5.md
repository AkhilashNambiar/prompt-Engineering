# Module 5: Prompt Engineering for Engineering Workflows
## Professional Corporate Training Session

---

## 1. TOPIC OVERVIEW

### What is the Topic?

**Prompt Engineering for Engineering Workflows** is the application of specialized prompting techniques to accelerate and enhance every stage of the software development lifecycle—from writing and debugging code, to testing, documentation, database management, and architectural decision-making. It's about using AI as your intelligent engineering partner across the entire development process.

**Real-World Analogy:** Imagine having a senior developer, a QA engineer, a technical writer, a database administrator, and a solutions architect—all available instantly, 24/7, and willing to help with any task. That's what prompt engineering enables. You're not replacing engineers; you're giving every engineer a team of AI assistants specialized for different aspects of their work.

### Why is it Necessary?

**The Problem It Solves:**
- Engineers spend 40-60% of their time on non-coding tasks (documentation, debugging, testing)
- Knowledge loss when senior engineers leave
- Inconsistent code quality across teams
- Slow onboarding for new developers
- Technical debt from poor documentation

**Why Professionals Should Learn It:**
- **Speed:** Generate code, tests, and documentation in seconds
- **Quality:** AI-assisted code review and optimization
- **Knowledge Preservation:** Document decisions and architecture
- **Onboarding:** AI can explain codebases to new team members
- **Consistency:** Standardized approaches across teams

**Business Value:**
- 40-60% reduction in development time for routine tasks
- 70% faster documentation creation
- 50% reduction in bug introduction through AI-assisted code review
- 3x faster onboarding for new engineers
- Significant reduction in technical debt through better documentation

---

## 2. CONCEPT EXPLANATION

### Basic Understanding

Engineering workflow prompt engineering applies specific patterns and techniques to development tasks. Each area of engineering—coding, testing, data, documentation, DevOps, and architecture—requires tailored prompting approaches.

### Software Development Prompts

#### 1. AI-Assisted Code Generation
**What It Is:** Using AI to generate code based on natural language descriptions.

**Key Principles:**
- Be specific about language, framework, and requirements
- Include inputs, outputs, and edge cases
- Specify performance and security requirements
- Request best practices and patterns

**Example Prompt:**
```
Generate a Python function using FastAPI that:
- Accepts user registration data (email, password, name)
- Validates email format and password strength
- Hashes password using bcrypt
- Stores user in PostgreSQL database
- Returns JWT token on success
- Handles duplicate email errors
```

#### 2. Code Explanation
**What It Is:** Having AI explain code in different contexts and levels of detail.

**Key Principles:**
- Specify the audience (junior dev, senior, non-technical)
- Request different levels of detail
- Ask for architectural context when relevant
- Request analogies for complex concepts

**Example:**
```
Explain this React component:
[Code]
Target audience: Junior developers with 6 months React experience.
Include: Purpose, prop flow, state management, lifecycle considerations.
```

#### 3. Code Optimization
**What It Is:** Identifying and fixing performance, readability, and maintainability issues.

**Key Principles:**
- Specify performance requirements (time, memory)
- Mention production environment constraints
- Request before/after comparison
- Ask for justification of changes

**Example:**
```
Optimize this Python function for an API endpoint that handles 
10,000 requests/minute. Priority: Speed > Memory > Readability.
Show before/after comparison and explain each optimization.
```

#### 4. Refactoring Prompts
**What It Is:** Restructuring code without changing functionality to improve quality.

**Key Principles:**
- Specify refactoring goals (readability, patterns, modularity)
- Maintain backward compatibility requirements
- Request design pattern recommendations
- Include test expectations

**Example:**
```
Refactor this monolithic class following SOLID principles.
Current code handles user authentication, data access, and logging.
Extract into separate classes with clear responsibilities.
Maintain all existing functionality.
```

### Debugging and Testing

#### 5. Debugging Prompts
**What It Is:** Using AI to identify and fix bugs in code.

**Key Principles:**
- Include full error messages and stack traces
- Describe expected vs actual behavior
- Include relevant code sections
- Mention environment details (language version, OS, dependencies)

**Example:**
```
Debug this Python code:

[Error message]
[Code snippet]
[Expected behavior vs actual]

Environment: Python 3.11, running on Ubuntu, using SQLAlchemy 2.0.
```

#### 6. Unit Test Generation
**What It Is:** Automatically creating comprehensive unit tests.

**Key Principles:**
- Specify testing framework (pytest, JUnit, etc.)
- Include edge cases and error conditions
- Request test coverage analysis
- Mention mocking requirements

**Example:**
```
Generate unit tests for this function:
[Function code]
Testing framework: pytest
Include: Happy path, edge cases, error handling, boundary conditions.
Mock external dependencies.
```

### Data and Database Tasks

#### 7. SQL Query Generation
**What It Is:** Creating optimized SQL queries from natural language descriptions.

**Key Principles:**
- Describe the database schema
- Specify query purpose and requirements
- Include performance expectations
- Mention database type (PostgreSQL, MySQL, etc.)

**Example:**
```
Generate a PostgreSQL query that:
- Find top 10 customers by total purchase amount in Q3 2024
- Include customer name, email, total spent
- Join orders, customers, and order_items tables
- Optimize for 10M+ records
- Use indexes where appropriate
```

#### 8. Data Transformation Prompts
**What It Is:** Creating data pipelines and transformation logic.

**Key Principles:**
- Specify input and output formats
- Describe transformation rules
- Include data quality requirements
- Mention volume and frequency

**Example:**
```
Create a data transformation pipeline that:
- Input: CSV with 2M rows (customer_id, date, product, quantity, price)
- Clean: Remove negative quantities, valid date ranges
- Transform: Calculate total by customer/month, aggregate by product category
- Output: Parquet files partitioned by month
- Python with pandas, optimized for memory usage
```

### APIs and Technical Documentation

#### 9. API Documentation Generation
**What It Is:** Creating complete API documentation from code.

**Key Principles:**
- Request all documentation elements (endpoints, parameters, responses)
- Include examples for successful and error responses
- Specify format (OpenAPI, Markdown, etc.)
- Mention authentication requirements

**Example:**
```
Generate OpenAPI 3.0 documentation for:
[FastAPI/Flask/Express routes]
Include: All endpoints, request/response schemas, authentication,
        error responses, and example requests for each endpoint.
```

### DevOps and Architecture

#### 10. DevOps Automation Prompts
**What It Is:** Creating infrastructure and deployment automation.

**Key Principles:**
- Specify infrastructure requirements
- Include security and compliance needs
- Mention scaling and recovery requirements
- Request configuration examples

**Example:**
```
Create a Kubernetes deployment YAML for:
- A Node.js microservice with 3 replicas
- Auto-scaling based on CPU usage
- Health checks every 30s
- Secret management for environment variables
- Rolling update strategy with 25% max surge
```

### How AI Interprets Engineering Prompts

**What Makes Engineering Prompts Different:**
- **Precision matters:** Code must be syntactically correct
- **Context is crucial:** Need to understand the full system
- **Standards apply:** Best practices, patterns, and conventions
- **Safety is key:** Security, error handling, and edge cases

**Best Practices for Engineering Prompts:**

1. **Be Specific with Context:**
   - Language, version, and frameworks
   - Existing codebase structure
   - Performance requirements
   - Security constraints

2. **Request Justification:**
   - Why was this approach chosen?
   - What are the trade-offs?
   - How does it handle edge cases?

3. **Include Examples:**
   - Input/output examples
   - Error scenarios
   - Usage examples

4. **Set Quality Standards:**
   - Code style guidelines
   - Testing requirements
   - Documentation standards

5. **Request Multiple Approaches:**
   - Different implementations
   - Pros/cons of each
   - Recommendation with justification

### Common Mistakes to Avoid

| Mistake | Why It's a Problem | Better Approach |
|---------|-------------------|-----------------|
| Vague requirements | AI generates incorrect code | Be specific about inputs, outputs, and constraints |
| No error handling | Code fails in production | Request comprehensive error handling |
| Forgetting performance | Code scales poorly | Specify performance requirements |
| Missing security considerations | Vulnerable code | Request secure coding practices |
| No testing | Undetected bugs | Ask for tests with edge cases |
| Outdated dependencies | Compatibility issues | Specify version requirements |

---

## 3. PRACTICAL EXAMPLE

### Example 1: Simple Beginner Example

**Scenario:** A junior developer needs help writing a simple function.

**Input:**
```
Write a Python function that:
- Takes a list of numbers
- Returns the average
- Handles empty lists gracefully
- Includes type hints and docstring
- Has error handling for non-numeric values
```

**Process:**
1. AI identifies Python as the language
2. Understands the requirements (average, empty list, type hints, etc.)
3. Generates code with best practices
4. Includes documentation and error handling

**Expected Output:**
```python
from typing import List, Union

def calculate_average(numbers: List[Union[int, float]]) -> Union[float, None]:
    """
    Calculate the average of a list of numbers.
    
    Args:
        numbers: A list of integers or floats
        
    Returns:
        The average as a float, or None if the list is empty
        
    Raises:
        TypeError: If any element is not a number
        
    Examples:
        >>> calculate_average([1, 2, 3, 4, 5])
        3.0
        >>> calculate_average([])
        None
    """
    if not numbers:
        return None
    
    for num in numbers:
        if not isinstance(num, (int, float)):
            raise TypeError(f"Expected number, got {type(num).__name__}")
    
    return sum(numbers) / len(numbers)

# Usage example
if __name__ == "__main__":
    result = calculate_average([1, 2, 3, 4, 5])
    print(f"Average: {result}")
```

---

### Example 2: Business Example

**Scenario:** An engineering team needs to refactor a legacy payment processing system.

**Input:**
```
ROLE:
Act as a Senior Software Architect with expertise in payment systems 
and microservices architecture.

CONTEXT:
We have a legacy monolithic payment processing system in Python/Django.
- 50,000+ transactions/day
- 15+ years old codebase
- High technical debt
- Frequently goes down during peak hours
- Team of 12 engineers maintaining it
- Currently running on AWS EC2

TASK:
Design a migration strategy from the legacy monolith to a modern 
microservices architecture for our payment processing system.

INSTRUCTIONS:
1. Analyze the challenges of the current system
2. Recommend a microservices breakdown (with service boundaries)
3. Provide a phased migration approach (0-18 months)
4. Address data migration and consistency challenges
5. Include technology recommendations
6. Identify potential risks and mitigation strategies
7. Estimate team size and skill requirements

CONSTRAINTS:
- Must be production-safe (no downtime)
- Must handle 100K+ transactions/day after migration
- Must comply with PCI-DSS
- Budget: $2M over 18 months
- Team cannot exceed 12 people
- Must use cloud-native technologies

OUTPUT FORMAT:
Provide a migration strategy document with:
1. Executive Summary
2. Current State Analysis
3. Proposed Architecture
4. Migration Phases
5. Technology Stack
6. Risk Assessment
7. Resource Plan
8. Timeline
9. Success Metrics
```

**Process:**
1. Senior Architect role sets expertise expectations
2. Comprehensive context about the legacy system
3. Detailed instructions guide the architecture design
4. Constraints ensure practical, feasible recommendations
5. Structured output format for clear documentation

**Expected Output:**
```markdown
# Payment Processing System Migration Strategy

## 1. Executive Summary
Migrate the 15-year-old monolithic payment system to a cloud-native microservices architecture over 18 months, eliminating single points of failure, scaling to 100K+ daily transactions, and enabling independent team velocity.

## 2. Current State Analysis

### Challenges
- **Monolithic Architecture**: Single deployment, any change risks entire system
- **Fragile Database**: Single PostgreSQL DB with replication issues
- **Technical Debt**: 15+ years of accumulated complexity, 40% code coverage
- **Performance Bottlenecks**: Payment processing times >30s during peak
- **Team Velocity**: Only 2-3 features per sprint, 40% time on maintenance
- **Outdated Infrastructure**: EC2 instances without auto-scaling

### Key Metrics
- **Transactions/Day**: 50,000 (peak 5,000/hr)
- **Uptime**: 98.7% (target 99.99%)
- **Processing Time**: 30s avg (target <5s)
- **Response Time**: 2.3s avg (target <200ms)
- **Codebase**: 500,000+ lines across 45 Django apps

## 3. Proposed Architecture

### Service Breakdown

```
┌─────────────────────────────────────────────────────────────┐
│                    API Gateway (Kong)                       │
└─────────────────────────────────────────────────────────────┘
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
┌───────▼────────┐ ┌──────▼───────┐ ┌──────▼────────┐
│ Payment Core    │ │ Customer     │ │ Notification  │
│ Service        │ │ Service      │ │ Service       │
├────────────────┤ ├──────────────┤ ├───────────────┤
│ - Process      │ │ - Profile    │ │ - Email       │
│ - Validation   │ │ - Verification│ │ - SMS         │
│ - Routing      │ │ - History    │ │ - Webhook     │
│ - Settlement   │ │              │ │               │
└───────┬────────┘ └──────┬───────┘ └──────┬────────┘
        │                 │                │
        └─────────────────┼────────────────┘
                          │
        ┌─────────────────▼─────────────────┐
        │         Event Bus (Kafka)         │
        └───────────────────────────────────┘
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
┌───────▼────────┐ ┌──────▼───────┐ ┌──────▼────────┐
│ Analytics       │ │ Fraud        │ │ Reporting     │
│ Service        │ │ Detection     │ │ Service       │
├────────────────┤ ├──────────────┤ ├───────────────┤
│ - Metrics      │ │ - Real-time  │ │ - Daily       │
│ - Forecasting  │ │ - Pattern    │ │ - Monthly     │
│ - Anomalies    │ │ - Rules      │ │ - Real-time   │
└────────────────┘ └──────────────┘ └───────────────┘
```

### Technology Stack
- **Languages**: Go (core services), Python (ML services)
- **Frameworks**: GoFiber, FastAPI
- **Database**: PostgreSQL (partitioned), Redis (caching), DynamoDB (session)
- **Messaging**: Apache Kafka
- **Container**: Docker + Kubernetes (EKS)
- **CI/CD**: GitHub Actions + ArgoCD
- **Monitoring**: Prometheus + Grafana + Datadog
- **API Gateway**: Kong
- **Service Mesh**: Istio

## 4. Migration Phases

### Phase 1: Foundation (Months 0-6)
- **Goal**: Establish modern infrastructure and DevOps practices
- **Actions**:
  1. Set up Kubernetes cluster with Istio service mesh
  2. Implement CI/CD pipeline (GitHub Actions → EKS)
  3. Create shared libraries for common patterns
  4. Set up monitoring, logging, and alerting
  5. Migrate read-only data to new databases
- **Risk**: New infrastructure complexity
- **Mitigation**: Start with non-critical services first
- **Team**: 4 engineers (DevOps + Backend)

### Phase 2: Strangler Pattern (Months 6-12)
- **Goal**: Extract services one by one with API Gateway routing
- **Actions**:
  1. Implement Customer Service (7 weeks)
  2. Implement Notification Service (4 weeks)
  3. Implement Payment Core Service (12 weeks)
  4. Route 20% of traffic to new services
  5. Monitor and fix issues
- **Risk**: Data consistency during split
- **Mitigation**: Event sourcing with Kafka for eventual consistency
- **Team**: 8 engineers (2 per service + 2 platform)

### Phase 3: Complete Migration (Months 12-15)
- **Goal**: Move all traffic to new system
- **Actions**:
  1. Route 100% traffic to new services
  2. Decommission legacy payment service
  3. Migrate remaining reports and analytics
  4. Train team on new architecture
- **Risk**: Undiscovered edge cases
- **Mitigation**: Gradual traffic increase + canary deployments
- **Team**: 10 engineers

### Phase 4: Optimization (Months 15-18)
- **Goal**: Performance tuning and optimization
- **Actions**:
  1. Performance testing and tuning
  2. Implement auto-scaling policies
  3. Add ML-based fraud detection
  4. Optimize database queries and indexes
  5. Implement disaster recovery
- **Risk**: Performance bottlenecks in new architecture
- **Mitigation**: Load testing, proper monitoring, auto-scaling
- **Team**: 12 engineers

## 5. Risk Assessment

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| Data migration issues | High | Critical | Dual-write strategy + verification steps |
| Performance degradation | Medium | High | Load testing, monitoring, performance benchmarks |
| Security compliance | Medium | Critical | PCI-DSS audit, security review, encryption at rest |
| Team skill gaps | High | Medium | Training program, cloud certification budget |
| Integration failures | Medium | Medium | Comprehensive integration tests, feature flags |
| Legacy system coupling | High | High | API-first approach, adapter pattern |

## 6. Resource Plan

### Team Structure
- **Platform Team** (2 engineers): Kubernetes, CI/CD, Monitoring
- **Payment Core** (2 engineers): Go, transactions
- **Customer Service** (2 engineers): Python, user data
- **Notification Service** (1 engineer): Email/SMS integration
- **Analytics Service** (2 engineers): Data pipelines, reporting
- **QA/Test** (1 engineer): Integration testing, performance
- **Architect** (1 engineer): Oversee all technical decisions
- **PM** (1 engineer): Timeline, coordination

### Budget Breakdown
- **Infrastructure**: $500K (EKS, databases, monitoring)
- **Tools**: $100K (Datadog, CI/CD, security tools)
- **Team**: $1.2M (12 engineers × 18 months)
- **Training**: $50K (Kubernetes, Go, Kafka certifications)
- **Contingency**: $150K (unexpected costs)
- **Total**: $2M

## 7. Success Metrics

### Performance KPIs
- **Transaction Processing**: <5s (from 30s)
- **API Response Time**: <200ms (from 2.3s)
- **Uptime**: 99.99% (from 98.7%)
- **Transactions/Day**: 100,000+ (from 50,000)

### Business KPIs
- **Team Velocity**: 5x increase in features/sprint
- **Onboarding**: New devs productive in 2 weeks (from 3 months)
- **Deployment Frequency**: Daily (from quarterly)
- **MTTR**: <30 minutes (from 3+ hours)

### Quality Metrics
- **Code Coverage**: 80%+ (from 40%)
- **Testing**: Automated regression suite
- **Documentation**: Up-to-date service documentation
- **Security**: PCI-DSS compliance validated

## 8. Recommendation
Proceed with the phased migration approach. The architecture provides the necessary scalability, maintainability, and reliability while managing risk through incremental deployment and comprehensive monitoring.
```

---

### Example 3: Technical Example

**Scenario:** A DevOps engineer needs to debug a production issue.

**Input:**
```
ROLE:
Act as a Senior DevOps Engineer specializing in Kubernetes and 
microservices troubleshooting.

TASK:
Debug the following production issue:

ISSUE DESCRIPTION:
Our payment service microservice is failing health checks periodically. 
The service runs in Kubernetes (EKS) with 3 replicas.

ERROR LOGS:
```
2024-01-15 14:32:15 ERROR: Connection pool exhausted for database connection
2024-01-15 14:32:16 WARNING: Health check failed for pod payment-7d8f9c-abcde
2024-01-15 14:32:18 ERROR: connection timeout after 5000ms
2024-01-15 14:32:20 ERROR: Database connection failed: TimeoutError
```

ENVIRONMENT DETAILS:
- Kubernetes version: 1.27
- Service language: Python (FastAPI)
- Database: PostgreSQL 14 (RDS)
- Connection pool: SQLAlchemy pool_size=5, max_overflow=10
- Requests per replica: ~100/min
- Database connections: 40 total available
- CPU limit: 2 cores, Memory: 4GB

RECENT CHANGES:
- Deployed new feature 2 days ago (bulk order processing)
- Increased replica count from 2 to 3 yesterday
- No database configuration changes

INSTRUCTIONS:
1. Analyze the root cause of the health check failures
2. Provide immediate remediation steps
3. Recommend long-term solutions
4. Create a Kubernetes manifest to implement the solution
5. Add monitoring/alerting recommendations

CONSTRAINTS:
- Must be a quick fix (production issue)
- Zero downtime required
- Must be within existing budget
- Need to implement within 4 hours

OUTPUT FORMAT:
Provide a troubleshooting report with:
1. Root Cause Analysis
2. Immediate Actions
3. Long-term Recommendations
4. Implementation Code
5. Monitoring Plan
```

**Process:**
1. DevOps Engineer role sets expert troubleshooting context
2. Detailed error logs and environment details provided
3. Step-by-step instructions guide systematic analysis
4. Production constraints ensure practical solutions

**Expected Output:**
```markdown
# Payment Service Health Check Failure Analysis

## 1. Root Cause Analysis

### Primary Issue: Connection Pool Exhaustion

**What's Happening:**
The bulk order processing feature introduced in the last deployment is creating significantly more database connections than before. The service is hitting `max_overflow=10` and `pool_size=5` limits, causing new requests to time out waiting for connections.

**Detailed Chain of Events:**
1. Bulk order processing creates multiple database transactions per order
2. Each transaction holds a connection for 2-5 seconds
3. With 100 requests/min × 3 replicas = 300 requests/min
4. Connection pool: 5 connections + 10 overflow = 15 max per replica
5. 15 connections × 3 replicas = 45 connections (exceeding the 40 available database connections)
6. When connections exceed available, requests start timing out
7. Kubernetes health checks time out, pods are marked unhealthy

### Contributing Factors:
- **Connection leak**: Some connections not properly released after transactions
- **Aggressive scaling**: Adding third replica without database connection planning
- **Long-running queries**: Bulk operations are not optimized
- **No connection timeout**: Default timeout (30s) is too long when pool is exhausted

## 2. Immediate Actions (Next 4 Hours)

### A. Increase Connection Pool Limits (Immediate)

**Database Side:**
```sql
-- Increase max connections on PostgreSQL (RDS)
ALTER SYSTEM SET max_connections = 100;
-- Restart database (requires maintenance window)
-- OR use RDS parameter group to modify and apply immediately
```

### B. Increase Application Pool Size

**Update Kubernetes ConfigMap / Environment Variables:**
```yaml
# application-config.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: payment-service-config
data:
  DATABASE_POOL_SIZE: "10"      # Increased from 5
  DATABASE_MAX_OVERFLOW: "20"   # Increased from 10
  DATABASE_POOL_TIMEOUT: "5"    # Reduced from 30
  DATABASE_POOL_RECYCLE: "1800" # Recycle connections after 30 minutes
```

### C. Deploy with Connection Pool Changes

```bash
# Apply the configuration
kubectl apply -f application-config.yaml

# Restart deployment with new env vars
kubectl rollout restart deployment/payment-service

# Monitor rollout status
kubectl rollout status deployment/payment-service
```

### D. Temporary Query Optimization (Quick Fix)

```python
# Add bulk processing optimization
def process_bulk_orders(orders_data):
    """Process bulk orders with optimized connection usage."""
    # Use single transaction for all updates
    with db.transaction():
        # Use batch operations instead of per-item
        connection.execute(
            bulk_insert(OrderItem, orders_data)
        )
```

## 3. Long-term Recommendations

### 1. Implement Connection Pooling Strategy

**AWS RDS Proxy Implementation:**
```yaml
# RDS Proxy configuration
apiVersion: rds.aws.com/v1alpha1
kind: DBProxy
metadata:
  name: payment-db-proxy
spec:
  engineFamily: POSTGRESQL
  dbProxyName: payment-proxy
  roleArn: arn:aws:iam::123456789:role/rds-proxy-role
  vpcSubnetIds:
    - subnet-1
    - subnet-2
  auth:
    - authScheme: SECRETS
      secretArn: arn:aws:secretsmanager:...
  requireTLS: true
```

**Benefits:**
- Connection pooling at infrastructure level
- Automatic connection management
- Reduces database CPU and memory pressure
- Enables connection sharing across replicas

### 2. Optimize Queries for Bulk Operations

```python
# Before: Multiple individual queries
def create_orders_bad(orders):
    for order in orders:
        db.execute("INSERT INTO orders ...", order)
        db.execute("INSERT INTO order_items ...", order.items)

# After: Bulk operations with prepared statements
def create_orders_good(orders):
    # Prepare statements once
    order_stmt = db.prepare("INSERT INTO orders ...")
    item_stmt = db.prepare("INSERT INTO order_items ...")
    
    # Bulk insert using executemany
    db.executemany(order_stmt, orders_data)
    db.executemany(item_stmt, items_data)
    
    # Single commit
    db.commit()
```

### 3. Implement Circuit Breaker Pattern

```python
from circuitbreaker import circuit

@circuit(failure_threshold=5, recovery_timeout=60)
def process_order_with_circuit_breaker(order_data):
    """Execute with circuit breaker to prevent cascading failures."""
    return db.execute("INSERT INTO orders ...", order_data)
```

### 4. Add HPA Based on Connection Usage

```yaml
# HorizontalPodAutoscaler.yaml
apiVersion: autoscaling/v2
kind: HorizontalPodAutoscaler
metadata:
  name: payment-service-hpa
spec:
  scaleTargetRef:
    apiVersion: apps/v1
    kind: Deployment
    name: payment-service
  minReplicas: 3
  maxReplicas: 10
  metrics:
  - type: Pods
    pods:
      metric:
        name: database_connections_used
      target:
        type: AverageValue
        averageValue: "8"  # Scale when >80% of pool
```

## 4. Implementation Code

### Complete Kubernetes Deployment with Fixes

```yaml
# deployment.yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: payment-service
  namespace: production
  labels:
    app: payment-service
    version: v2.1.0
spec:
  replicas: 3
  strategy:
    type: RollingUpdate
    rollingUpdate:
      maxSurge: 1
      maxUnavailable: 0  # Zero downtime
  selector:
    matchLabels:
      app: payment-service
  template:
    metadata:
      labels:
        app: payment-service
      annotations:
        prometheus.io/scrape: "true"
        prometheus.io/port: "8000"
    spec:
      containers:
      - name: payment-service
        image: payment-service:latest
        imagePullPolicy: Always
        ports:
        - containerPort: 8000
          name: http
          protocol: TCP
        env:
        - name: DATABASE_URL
          valueFrom:
            secretKeyRef:
              name: db-secret
              key: url
        - name: DATABASE_POOL_SIZE
          value: "10"
        - name: DATABASE_MAX_OVERFLOW
          value: "20"
        - name: DATABASE_POOL_TIMEOUT
          value: "5"
        - name: DATABASE_POOL_RECYCLE
          value: "1800"
        - name: CONNECTION_POOL_MAX_AGE
          value: "300"
        - name: OPTIMIZE_BULK_OPERATIONS
          value: "true"
        resources:
          requests:
            memory: "512Mi"
            cpu: "250m"
          limits:
            memory: "2Gi"
            cpu: "1"
        livenessProbe:
          httpGet:
            path: /healthz
            port: 8000
          initialDelaySeconds: 30
          periodSeconds: 10
          timeoutSeconds: 3
          failureThreshold: 3
        readinessProbe:
          httpGet:
            path: /ready
            port: 8000
          initialDelaySeconds: 15
          periodSeconds: 5
          timeoutSeconds: 2
          failureThreshold: 2
        lifecycle:
          preStop:
            exec:
              command: ["sh", "-c", "sleep 15 && /app/graceful-shutdown"]
```

### Connection Pool Monitoring Script

```python
# monitor_connections.py - Deploy as sidecar
import psycopg2
import time
from prometheus_client import Gauge, start_http_server

active_connections = Gauge('db_active_connections', 'Active DB connections')
idle_connections = Gauge('db_idle_connections', 'Idle DB connections')
waiting_connections = Gauge('db_waiting_connections', 'Waiting DB connections')

def collect_metrics(db_url):
    conn = psycopg2.connect(db_url)
    cursor = conn.cursor()
    
    while True:
        # Query pg_stat_activity
        cursor.execute("""
            SELECT 
                COUNT(*) FILTER (WHERE state = 'active') as active,
                COUNT(*) FILTER (WHERE state = 'idle') as idle,
                COUNT(*) FILTER (WHERE wait_event IS NOT NULL) as waiting
            FROM pg_stat_activity
        """)
        
        active, idle, waiting = cursor.fetchone()
        active_connections.set(active)
        idle_connections.set(idle)
        waiting_connections.set(waiting)
        
        time.sleep(15)

if __name__ == "__main__":
    start_http_server(9090)
    collect_metrics("postgresql://...")
```

## 5. Monitoring Plan

### Key Metrics to Monitor

```yaml
# prometheus-rules.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: payment-service-alerts
data:
  alerts.yaml: |
    groups:
      - name: database_alerts
        rules:
        - alert: DBConnectionsExhausted
          expr: increase(db_connection_wait_seconds[5m]) > 10
          annotations:
            severity: critical
            summary: "Database connection pool exhausted"
            
        - alert: DBConnectionPoolHigh
          expr: db_pool_current_connections / db_pool_max_connections > 0.85
          for: 2m
          annotations:
            severity: warning
            summary: "Connection pool above 85% usage"
            
        - alert: SlowQueries
          expr: increase(db_query_duration_seconds_bucket[5m]) > 10
          annotations:
            severity: warning
            summary: "Slow queries detected"
```

### Dashboard Recommendations

**Grafana Dashboard Components:**
1. **Connection Pool Usage**: Current connections vs. max
2. **Query Performance**: P95, P99 query duration
3. **Active Connections**: By service and pod
4. **Transaction Rates**: Per second
5. **Error Rates**: Connection timeouts, query errors
6. **Resource Usage**: CPU/Memory of database and application pods

## Summary of Immediate Actions

| Priority | Action | Owner | Timeline |
|----------|--------|-------|----------|
| Critical | Increase database max_connections | DBA | 1 hour |
| High | Update application pool settings | DevOps | 30 min |
| High | Deploy with new config | DevOps | 30 min |
| High | Monitor connection usage | All | Ongoing |
| Medium | Implement RDS Proxy | DevOps | 1 week |
| Medium | Optimize bulk queries | Developer | 2 weeks |
| Low | Implement circuit breaker | Developer | 1 month |
| Low | Add HPA based on DB metrics | DevOps | 1 month |

**Rollback Plan:** If issues persist, revert to the previous deployment without the bulk order optimization and roll back replica count to 2.
```

---

## 4. SUGGESTED PROMPT TEMPLATE

### Engineering Prompt Template

```
[ROLE]
Act as a [Senior/Lead] [Software Engineer/DevOps Engineer/Data Engineer/Architect] 
with [X] years of experience in [specific domain/technology].

[CONTEXT]
Project: [Project name and brief description]
Technology Stack: [Languages, frameworks, databases, cloud services]
Team: [Team size, experience level]
Current Status: [What's working, what's not]
Constraints: [Budget, timeline, performance requirements]

[TASK]
Specific engineering task:
[What you need: code, debugging, documentation, architecture design, etc.]

[INSTRUCTIONS]
1. [Step 1 - e.g., Analyze requirements]
2. [Step 2 - e.g., Design approach]
3. [Step 3 - e.g., Implementation]
4. [Step 4 - e.g., Testing/Validation]
5. [Step 5 - e.g., Documentation]

[CONSTRAINTS]
- Language/Version: [e.g., Python 3.11, React 18]
- Performance: [e.g., <200ms response, handle 10K req/sec]
- Security: [e.g., OAuth2, encryption requirements]
- Testing: [e.g., 90% code coverage]
- Documentation: [e.g., Inline comments, README]
- Deployment: [e.g., Kubernetes, Docker]

[EXAMPLES] (Optional)
Example of desired outcome:
[Provide input/output example]

[OUTPUT FORMAT]
Provide your response with:
1. [Section 1 - e.g., Approach]
2. [Section 2 - e.g., Implementation]
3. [Section 3 - e.g., Tests]
4. [Section 4 - e.g., Documentation]
```

---

## 5. COMPLETE SAMPLE PROMPT

### Production-Ready Prompt: API Integration

```
ROLE:
Act as a Senior Backend Engineer with 7 years of experience in Python, FastAPI, 
and microservices architecture. You specialize in building robust, 
production-grade APIs with comprehensive error handling and monitoring.

CONTEXT:
Project: Order Management System (OMS) - Phase 2
Technology Stack: Python 3.11, FastAPI, PostgreSQL 14, Redis 7, Docker, Kubernetes
Team: 5 backend engineers, 3 frontend, 2 QA
Current Status: We have a working monolith in Django, migrating to microservices
Constraints: Must maintain 99.99% uptime, handle 500 concurrent requests/second

TASK:
Build a RESTful API service for order creation and management. This is the 
core service in our microservices architecture.

INSTRUCTIONS:
1. Design the API endpoints (POST /orders, GET /orders/{id}, PUT /orders/{id}/status)
2. Implement input validation using Pydantic models
3. Create database models with SQLAlchemy ORM
4. Implement business logic with proper transaction management
5. Add comprehensive error handling (400, 404, 500 responses)
6. Implement idempotency key handling (prevent duplicate orders)
7. Add structured logging and request tracing
8. Create unit tests with pytest (80%+ coverage)
9. Add performance optimization (caching, connection pooling)
10. Document the API using OpenAPI/Swagger

CONSTRAINTS:
- Must use FastAPI
