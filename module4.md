# Module 4: Core Prompt Patterns
## Professional Corporate Training Session

---

## 1. TOPIC OVERVIEW

### What is the Topic?

**Core Prompt Patterns** are proven, reusable blueprints for structuring prompts to solve specific types of problems. Think of them as design patterns in software engineering—standardized solutions to common challenges that you can adapt and apply across different situations. Each pattern provides a specific structure and approach for achieving a particular outcome, whether that's getting better reasoning, controlling output format, or making complex decisions.

**Real-World Analogy:** Imagine you're a master chef with a collection of recipe templates. You have a template for soups (base + liquid + seasoning), one for stir-fries (protein + vegetables + sauce), and one for baking (dry ingredients + wet ingredients + temperature). Each template provides a proven structure, but you customize the ingredients. Similarly, prompt patterns provide proven structures for getting specific results from AI—you just fill in the details.

### Why is it Necessary?

**The Problem It Solves:**
- Starting from scratch for every prompt is inefficient
- Without patterns, prompts are inconsistent and unpredictable
- Complex tasks require specialized approaches that aren't obvious
- Teams waste time reinventing the wheel

**Why Should Professionals Learn It:**
- **Efficiency:** Use proven patterns instead of guessing
- **Consistency:** Standardized approaches across teams
- **Quality:** Patterns are refined through extensive testing
- **Speed:** Faster prompt creation with templates
- **Versatility:** Handle any type of task with the right pattern

**Business Value:**
- 70% faster prompt creation using patterns
- 60% more consistent outputs across team members
- Reduced training time for new team members
- Standardized quality across all AI interactions
- Ability to handle 10x more use cases confidently

---

## 2. CONCEPT EXPLANATION

### Basic Understanding

Prompt patterns are structured frameworks that guide how you interact with AI. Each pattern is designed for a specific type of task or challenge. By learning these patterns, you can quickly select and apply the right approach for any situation.

### Foundation Patterns

#### 1. Persona Pattern
**What It Is:** Assigning a specific role, expertise level, and perspective to the AI.

**Structure:**
```
Act as [role] with [expertise/experience]. 
[Task with the persona's perspective].
```

**Example:**
```
Act as a Senior UX Designer with 8 years of experience in mobile apps.
Review this app interface and provide usability recommendations.
```

**Best For:** Tasks requiring specialized knowledge, specific tone, or expert perspective.

#### 2. Question Refinement Pattern
**What It Is:** Iteratively improving questions to get better answers.

**Structure:**
```
Ask a question → Evaluate the response → Identify what's missing → 
Refine the question → Get a better response.
```

**Example:**
```
Initial: "How can we improve customer satisfaction?"
Refined: "Based on customer feedback from Q3 showing a 15% drop in NPS 
for our mobile app, what specific UX improvements would most impact 
customer satisfaction for users aged 45+?"
```

**Best For:** When initial questions are too broad or miss the mark.

#### 3. Instruction Decomposition Pattern
**What It Is:** Breaking complex instructions into smaller, manageable components.

**Structure:**
```
Complex task → Break into steps → Order steps logically → 
Provide each as a clear instruction.
```

**Example:**
```
Instead of: "Create a marketing strategy"
Use: 
Step 1: Analyze our target audience demographics
Step 2: Research competitor marketing approaches
Step 3: Identify 5 unique positioning angles
Step 4: Choose 3 priority channels
Step 5: Create a 6-month execution timeline
```

**Best For:** Complex, multi-step tasks that need structure.

### Reasoning and Improvement Patterns

#### 4. Step-Back Prompting
**What It Is:** Asking the AI to take a broader perspective before diving into details.

**Structure:**
```
Step back and consider [broader context/principle].
Then apply this perspective to [specific problem].
```

**Example:**
```
Step back and consider: What are the fundamental principles 
of user-centered design for mobile banking apps?
Now apply these principles to evaluate our current app's 
onboarding flow.
```

**Best For:** Getting strategic perspectives, avoiding tunnel vision.

#### 5. ReAct Pattern (Reasoning + Acting)
**What It Is:** A pattern where the AI reasons about the problem, acts (generates output), observes the results, and reasons again.

**Structure:**
```
Reason: Think about the problem and approach
Act: Generate output based on reasoning
Observe: Evaluate the output
Reason again: Refine based on observation
Act again: Generate improved output
```

**Example:**
```
Step 1 - Reason: "I need to create a customer email. Let me 
think about the audience, tone, and key messages."

Step 2 - Act: [Generate initial email draft]

Step 3 - Observe: "The email is too formal for our millennial 
audience. It lacks personalization."

Step 4 - Reason Again: "I should use a more casual tone, 
include personalization variables, and add a clearer CTA."

Step 5 - Act Again: [Generate improved email]
```

**Best For:** Iterative refinement, complex creative tasks.

#### 6. Critic and Reviewer Pattern
**What It Is:** Having the AI first generate content, then review and critique its own work.

**Structure:**
```
Generate [content].
Then review it as a critic, identifying:
1. What works well
2. What needs improvement
3. Specific recommendations
Then produce a revised version.
```

**Example:**
```
Step 1: Generate a product description.
Step 2: Review this description critically:
- Does it match our brand voice?
- Are the key benefits clear?
- Is the call-to-action compelling?
Step 3: Create an improved version based on this review.
```

**Best For:** Quality control, polishing outputs, self-improvement.

#### 7. Self-Review Concepts
**What It Is:** The AI systematically evaluating its own outputs against specific criteria.

**Structure:**
```
Generate response → Apply review criteria → Score/rate response → 
Identify gaps → Generate improved version.
```

**Best For:** Ensuring quality, consistency, and completeness.

### Output Control Patterns

#### 8. Output Formatter Pattern
**What It Is:** Explicitly defining the exact structure and format of the output.

**Structure:**
```
Provide the response in this exact format:
[Structure specification with examples]
```

**Example:**
```
Provide your response as:
# [Main Title]
## Overview
[2-3 sentence summary]
## Key Findings
- Finding 1
- Finding 2
- Finding 3
## Recommendations
1. [Recommendation with justification]
2. [Recommendation with justification]
```

**Best For:** When you need consistent, machine-readable, or structured outputs.

#### 9. Summarization Pattern
**What It Is:** Extracting the most important information from larger text.

**Structure:**
```
Summarize [source] focusing on [specific aspects].
Length: [word/sentence limit]
Format: [bullets/paragraphs/sections]
Key points to include: [list]
```

**Example:**
```
Summarize this 50-page market research report focusing on:
- Key industry trends
- Competitive landscape
- Growth opportunities
Length: 300 words, 3 sections
```

**Best For:** Information overload, quick insights, executive briefings.

#### 10. Extraction Pattern
**What It Is:** Pulling specific data points, facts, or insights from text.

**Structure:**
```
From this text, extract:
[Specific elements to extract]
Output as [format: JSON/table/list].
```

**Example:**
```
From these customer reviews, extract:
- Product features mentioned
- Sentiment (positive/negative/neutral)
- Specific complaints
- Suggestions
Output as a table with columns: Review, Features, Sentiment, Issues.
```

**Best For:** Data processing, research analysis, competitive intelligence.

#### 11. Classification Pattern
**What It Is:** Categorizing or tagging content based on defined criteria.

**Structure:**
```
Classify [input] into one of these categories:
[Category 1]: [Definition]
[Category 2]: [Definition]
[Category 3]: [Definition]
Provide reasoning for your classification.
```

**Example:**
```
Classify this customer support ticket:
"My account was charged twice this month."

Categories:
- Billing Issue: Problems with charges, refunds, or invoices
- Technical Issue: Problems with app functionality
- Product Question: Questions about features or usage
- Other: Anything not covered

Reasoning: Provide why you chose this category.
```

**Best For:** Routing requests, organizing content, automated sorting.

### Decision and Workflow Patterns

#### 12. Decision-Making Pattern
**What It Is:** Structured evaluation of options to make a recommendation.

**Structure:**
```
Decision needed: [What's being decided]
Options: [List of options]
Criteria: [Factors to consider]
Analysis: [Evaluate each option against criteria]
Recommendation: [Best option with justification]
```

**Example:**
```
Decision: Which marketing channel to prioritize for Q4?
Options: Social Media, Email Marketing, Content Marketing
Criteria: ROI, Reach, Implementation Time, Cost
Analysis: [Detailed comparison]
Recommendation: [Best channel with justification]
```

**Best For:** Strategic decisions, resource allocation, investment choices.

#### 13. Multi-Step Workflow Pattern
**What It Is:** A sequence of steps that must be followed in order.

**Structure:**
```
Follow this workflow:
Step 1: [Action] → Output: [Expected outcome]
Step 2: [Action] → Output: [Expected outcome]
Step 3: [Action] → Output: [Expected outcome]
[Continue as needed]
```

**Example:**
```
Step 1: Analyze customer feedback → Output: Top 10 complaints
Step 2: Prioritize complaints by frequency and impact → Output: Priority list
Step 3: Recommend solutions for top 5 priorities → Output: Action plan
Step 4: Create timeline and assign ownership → Output: Project plan
```

**Best For:** Process automation, sequential tasks, project planning.

#### 14. Prompt Chaining
**What It Is:** Using the output of one prompt as input for the next.

**Structure:**
```
Prompt 1: [Generate intermediate output]
Prompt 2: [Use Prompt 1's output + additional instructions]
Prompt 3: [Use Prompt 2's output + additional instructions]
```

**Example:**
```
Prompt 1: Research top 5 customer pain points
Prompt 2: Based on these pain points, identify feature opportunities
Prompt 3: Based on these features, create a product roadmap
```

**Best For:** Complex, multi-stage tasks requiring refinement.

### How AI Interprets These Patterns

**Why Patterns Matter:**
- **Structure improves understanding:** AI parses structured inputs better
- **Clear expectations:** Patterns tell the AI what you want and how
- **Consistent quality:** Patterns produce predictable results
- **Efficiency:** Less ambiguity = fewer iterations

**AI's Process with Each Pattern:**
1. **Persona:** "I should adopt this role's perspective"
2. **Question Refinement:** "Let me focus on what's being asked more precisely"
3. **Instruction Decomposition:** "I'll process these steps in order"
4. **Step-Back:** "Let me consider the bigger picture first"
5. **ReAct:** "I'll reason, act, observe, and improve"
6. **Critic/Reviewer:** "Let me evaluate my own work critically"
7. **Output Formatter:** "I need to structure my response exactly"
8. **Classification:** "I need to categorize based on these rules"

### Best Practices

1. **Select the pattern that matches your goal**—don't force a pattern
2. **Combine patterns strategically** when needed
3. **Start simple, add complexity only when necessary**
4. **Test different patterns** to find what works best
5. **Document pattern effectiveness** for your specific use cases
6. **Train your team** on pattern selection and application

### Common Mistakes to Avoid

| Mistake | Why It's a Problem | Better Approach |
|---------|-------------------|-----------------|
| Using the wrong pattern | Poor results, wasted time | Match pattern to task |
| Overcomplicating | Confuses the AI | Start with simple patterns |
| Forgetting to customize | Generic, shallow outputs | Add specific context |
| Not iterating | Missed opportunities for improvement | Test and refine patterns |
| Ignoring pattern combinations | Missing synergy | Combine complementary patterns |

### Advanced Considerations

**Combining Patterns:**
- **Persona + Question Refinement:** Expert perspective on refined questions
- **Step-Back + Decision-Making:** Strategic perspective before decisions
- **ReAct + Critic:** Iterative generation and self-improvement
- **Extraction + Classification:** Both pull data and categorize it

**Pattern Selection Decision Tree:**

```
Task Type → Choose Pattern
├── Need specialized knowledge → Persona Pattern
├── Question too broad → Question Refinement Pattern
├── Complex task with many steps → Instruction Decomposition Pattern
├── Need strategic perspective → Step-Back Prompting
├── Need iterative improvement → ReAct or Critic Pattern
├── Need specific format → Output Formatter Pattern
├── Need to distill information → Summarization Pattern
├── Need specific data points → Extraction Pattern
├── Need to sort/organize → Classification Pattern
├── Need to choose between options → Decision-Making Pattern
├── Need sequential process → Multi-Step Workflow Pattern
└── Need multi-stage project → Prompt Chaining
```

---

## 3. PRACTICAL EXAMPLE

### Example 1: Simple Beginner Example

**Scenario:** A junior marketer needs to write social media captions.

**Technique:** Persona Pattern + Output Formatter Pattern

**Input (Basic - No Pattern):**
```
Write social media posts for our new coffee product.
```

**Input (With Pattern):**
```
PERSONA PATTERN:
Act as a Senior Social Media Manager at a trendy coffee brand. 
You have 5 years of experience creating viral content and understand 
Gen Z and millennial audiences perfectly.

OUTPUT FORMATTER PATTERN:
Create 3 Instagram caption options in this exact structure:

Caption Option 1:
[Headline - short, catchy, emoji]
[Body - informative, engaging, 2-3 sentences]
[Call to action - with emoji]
[Hashtags - 5 relevant hashtags, including #OurBrand]

Caption Option 2:
[same structure]

Caption Option 3:
[same structure]

TASK:
Create captions for our new "Midnight Roast" - a dark, bold coffee 
with hints of dark chocolate and a smooth finish. Launching next week.
```

**Process:**
1. Persona sets the expertise and creativity level
2. Output Formatter ensures consistent, usable posts
3. The AI adopts the Social Media Manager role
4. Creates professional captions with the right tone

**Expected Output:**
```
Caption Option 1:
☕️ Your 3 PM just got an upgrade!

Meet Midnight Roast—our boldest blend yet. Dark, smooth, with hints of 
dark chocolate and a finish so flawless, you'll forget it's just coffee. 
Available next week—mark your calendars! 🗓️

Shop the drop before it's gone! 👆
#MidnightRoast #CoffeeLovers #NewBlend #DarkRoast #OurBrand

Caption Option 2:
🌙 Dark roast, dark vibes.

Introducing Midnight Roast—for those who like their coffee as bold as 
their ambitions. Hints of chocolate, zero regrets. Ready to conquer? 
We thought so. 💪

Pre-order now and be the first to taste! Link in bio! 🔗
#BoldCoffee #DarkRoast #NewLaunch #CoffeeTime #OurBrand

Caption Option 3:
Chocolate. Coffee. Perfection.

We've created the ultimate winter warmer—Midnight Roast. Smooth, bold, 
and dangerously delicious. It's dark chocolate meets coffee in the 
best way possible. 🍫☕️

Wake up and smell the chocolate. Order now! 🛒
#NewCoffee #DarkChocolate #WinterWarmers #CoffeeAddict #OurBrand
```

---

### Example 2: Business Example

**Scenario:** A product manager needs to prioritize features for next quarter.

**Technique:** Decision-Making Pattern + Instruction Decomposition Pattern

**Input:**
```
DECISION-MAKING PATTERN:
Decision Needed: Which 3 features should our product team build next quarter?

Options:
A) AI-Powered Chatbot - 8 weeks, complex
B) Mobile App Redesign - 10 weeks, very complex
C) Reporting Dashboard - 4 weeks, simple
D) API Integration Hub - 6 weeks, medium
E) User Onboarding Flow - 3 weeks, simple
F) Customization Platform - 9 weeks, complex

Criteria to evaluate:
1. ROI potential (1-10)
2. User demand (1-10)
3. Development effort (weeks)
4. Strategic importance (1-10)
5. Competitive differentiation (1-10)

INSTRUCTION DECOMPOSITION PATTERN:
Step 1: Score each option against all 5 criteria
Step 2: Calculate weighted scores (weights: ROI 25%, Demand 25%, 
        Effort 20%, Strategy 20%, Differentiation 10%)
Step 3: Rank options by total score
Step 4: Recommend top 3 with justification
Step 5: Provide a timeline for implementing the top 3 in sequence

Constraints:
- Team capacity: 6 developers, 12 weeks
- Must include at least one high-impact feature
- Must consider both user satisfaction and revenue

OUTPUT FORMAT:
Provide as a decision report with:
1. Scoring Matrix (table)
2. Rankings
3. Recommendations (top 3)
4. Timeline
5. Risk Assessment
6. Rationale
```

**Process:**
1. Decision-Making Pattern structures the evaluation
2. Instruction Decomposition breaks it into logical steps
3. The AI scores, weighs, and analyzes options systematically
4. Delivers a data-driven recommendation

**Expected Output:**
```markdown
# Q4 Feature Prioritization Decision Report

## Scoring Matrix

| Feature | ROI (25%) | Demand (25%) | Effort (20%) | Strategy (20%) | Diff (10%) | Total |
|---------|-----------|--------------|--------------|----------------|------------|-------|
| A - AI Chatbot | 9 | 8 | 8 weeks | 9 | 9 | 8.5 |
| B - Mobile Redesign | 7 | 7 | 10 weeks | 8 | 7 | 7.0 |
| C - Reporting | 6 | 9 | 4 weeks | 6 | 5 | 6.8 |
| D - API Hub | 8 | 6 | 6 weeks | 9 | 8 | 7.9 |
| E - Onboarding | 5 | 8 | 3 weeks | 5 | 4 | 5.9 |
| F - Customization | 7 | 7 | 9 weeks | 8 | 9 | 7.6 |

## Rankings

1. **AI-Powered Chatbot** - 8.5
2. **API Integration Hub** - 7.9
3. **Customization Platform** - 7.6

## Recommendations (Top 3)

### #1: AI-Powered Chatbot (Priority)
**Justification:** Highest ROI potential (9) and strategic importance (9). 
This feature directly addresses customer service costs and improves 
user experience. Differentiates us from competitors.

**Effort:** 8 weeks, high complexity
**Expected Impact:** 35% reduction in support tickets, 15% increase in user engagement

### #2: API Integration Hub (Priority)
**Justification:** Strong strategic value (9) enabling ecosystem growth. 
While user demand is moderate (6), this opens partnership opportunities 
and long-term revenue streams.

**Effort:** 6 weeks, medium complexity
**Expected Impact:** 20+ new integrations, 10% increase in enterprise sales

### #3: Customization Platform (Priority)
**Justification:** High differentiation potential (9). Users have been 
requesting customization for 18+ months. While complex (9 weeks), 
it's essential for user retention.

**Effort:** 9 weeks, high complexity
**Expected Impact:** 25% improvement in NPS, 12% retention increase

## Implementation Timeline

| Phase | Feature | Duration | Timeline |
|-------|---------|----------|----------|
| Phase 1 | AI Chatbot (MVP) | Weeks 1-8 | Start Q4 |
| Phase 2 | API Hub | Weeks 6-11 | Mid Q4 |
| Phase 3 | Customization | Weeks 7-12 | Late Q4 |

**Parallel Work:** API Hub and Customization can overlap with Chatbot after 
initial Chatbot architecture is completed (Week 6+).

## Risk Assessment

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| Chatbot accuracy issues | Medium | High | Start with limited scope, expand based on feedback |
| API integration delays | Low | Medium | Build with well-documented APIs |
| Customization overload | Medium | High | Implement with feature flags, gradual rollout |

## Final Rationale

The recommended approach delivers:
- **Immediate value** (Chatbot reduces costs)
- **Long-term strategic advantage** (API Hub and Customization)
- **Balanced investment** across user demand, ROI, and strategy
- **Manageable workload** that fits team capacity (max 8-week overlap)

**Decision:** Proceed with AI Chatbot as Phase 1 priority, with planning for 
API Hub and Customization to begin in parallel after Week 6.
```

---

### Example 3: Technical Example

**Scenario:** A developer needs to refactor and optimize code with quality assurance.

**Technique:** ReAct Pattern + Critic and Reviewer Pattern

**Input:**
```
CONTEXT:
We have a critical function in our e-commerce platform that processes 
orders. It's showing performance issues and error rates are increasing.

CURRENT CODE:
```python
def process_order(order_data):
    # Process order with poor error handling
    try:
        user = User.objects.get(id=order_data['user_id'])
        cart = Cart.objects.get(user=user, active=True)
        
        # Calculate total
        total = 0
        for item in cart.items.all():
            product = Product.objects.get(id=item.product_id)
            total += product.price * item.quantity
        
        # Create order
        order = Order.objects.create(user=user, total=total)
        
        # Process payment
        payment = Payment.objects.create(order=order, amount=total)
        payment.process()
        
        # Update inventory
        for item in cart.items.all():
            product = Product.objects.get(id=item.product_id)
            product.stock -= item.quantity
            product.save()
        
        # Clear cart
        cart.active = False
        cart.save()
        
        return order
    except Exception as e:
        logger.error(f"Order failed: {e}")
        return None
```

TASK - REACT PATTERN:
Step 1 (Reason): Analyze the current code. Identify performance issues, 
security vulnerabilities, error handling problems, and best practice violations.

Step 2 (Act): Generate a refactored version that addresses all issues.

Step 3 (Observe): Evaluate your refactored code against production standards.

Step 4 (Reason Again): Identify remaining improvement opportunities.

Step 5 (Act Again): Generate an optimized, production-ready version.

CRITIC AND REVIEWER PATTERN:
After generating each version, review it against:
1. Performance (n+1 queries, database efficiency)
2. Error handling (robustness, rollback, logging)
3. Security (SQL injection, data validation)
4. Maintainability (readability, comments, structure)
5. Transaction integrity (ACID compliance)

OUTPUT FORMAT:
Provide:
1. Code Analysis (issues identified)
2. Version 1: Refactored Code
3. Critic's Review of Version 1
4. Version 2: Optimized Code
5. Performance Comparison
6. Recommendations for Testing
```

**Process:**
1. ReAct Pattern guides iterative improvement
2. Critic Pattern ensures quality through self-review
3. The AI analyzes, refactors, reviews, and improves
4. Delivers production-ready optimized code

**Expected Output:**
```python
"""
CODE ANALYSIS - Issues Identified:

1. **N+1 Query Problem**: Iterating over cart.items.all() without 
   prefetching; each iteration queries Product separately
2. **No Transaction Management**: If any step fails, database is left 
   in inconsistent state
3. **No Input Validation**: order_data is assumed to contain user_id; 
   no validation for missing keys
4. **No Inventory Race Condition Handling**: No locking mechanism
5. **Generic Exception Handler**: Catching all exceptions hides the root cause
6. **Poor Performance**: Multiple round trips to database
7. **Insufficient Logging**: No structured logging with request IDs
8. **No Retry Logic**: Payment failure leads to customer frustration
9. **Hardcoded Values**: No handling for edge cases (negative quantities)
10. **Missing Return**: No order confirmation or ID returned
"""

# ================================================================
# VERSION 1 - REFACTORED CODE
# ================================================================

from django.db import transaction
from django.core.exceptions import ValidationError
import logging
import json
from typing import Optional, Dict, Any

logger = logging.getLogger(__name__)

class OrderProcessingError(Exception):
    """Custom exception for order processing errors."""
    pass

class PaymentFailedError(Exception):
    """Payment processing failed."""
    pass

class InventoryInsufficientError(Exception):
    """Insufficient stock for order."""
    pass

def process_order_refactored(order_data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
    """
    Process an order with proper error handling, transaction management,
    and performance optimizations.
    
    Args:
        order_data: Dict containing 'user_id' and optionally 'shipping_id'
        
    Returns:
        Dict with order details or None if processing fails
        
    Raises:
        OrderProcessingError: For fatal processing errors
    """
    
    # 1. Input validation
    user_id = order_data.get('user_id')
    if not user_id:
        raise ValidationError("user_id is required")
    
    # 2. Use select_related/prefetch_related for performance
    from django.db import models
    
    try:
        with transaction.atomic():
            # Get user with cart and items efficiently
            user = User.objects.select_for_update().get(id=user_id)
            
            cart = Cart.objects.select_for_update().filter(
                user=user, 
                active=True
            ).prefetch_related(
                models.Prefetch('items', queryset=CartItem.objects.select_related('product'))
            ).first()
            
            if not cart:
                logger.warning(f"No active cart found for user {user_id}")
                return None
            
            # 3. Efficiently calculate total with single query
            total = cart.items.aggregate(
                total=models.Sum(models.F('product__price') * models.F('quantity'))
            )['total'] or 0
            
            if total <= 0:
                raise ValidationError("Order total must be greater than 0")
            
            # 4. Check inventory with lock to prevent race conditions
            inventory_items = []
            for item in cart.items.all():
                product = Product.objects.select_for_update().get(id=item.product_id)
                if product.stock < item.quantity:
                    raise InventoryInsufficientError(
                        f"Insufficient stock for product {product.id}: {product.stock} available, {item.quantity} requested"
                    )
                inventory_items.append((product, item))
            
            # 5. Create order
            order = Order.objects.create(
                user=user, 
                total=total,
                status='pending'
            )
            
            # 6. Process payment with retry logic
            try:
                payment = Payment.objects.create(order=order, amount=total)
                payment.process(max_retries=3)
            except Exception as e:
                logger.error(f"Payment failed for order {order.id}: {str(e)}")
                raise PaymentFailedError(f"Payment processing failed: {str(e)}")
            
            # 7. Update inventory and order items
            for product, item in inventory_items:
                product.stock -= item.quantity
                product.save()
                # Create order items for reference
                OrderItem.objects.create(
                    order=order,
                    product=product,
                    quantity=item.quantity,
                    price_at_time=product.price
                )
            
            # 8. Clear cart
            cart.active = False
            cart.save()
            
            # 9. Log success
            logger.info(
                f"Order {order.id} processed successfully",
                extra={
                    'user_id': user_id,
                    'order_total': total,
                    'items_count': len(inventory_items)
                }
            )
            
            return {
                'order_id': order.id,
                'total': total,
                'status': order.status,
                'items': len(inventory_items)
            }
            
    except (ValidationError, PaymentFailedError, InventoryInsufficientError) as e:
        # These are expected business errors
        logger.error(f"Business error processing order for user {user_id}: {str(e)}")
        raise
    except Exception as e:
        # Unexpected errors
        logger.error(
            f"Unexpected error processing order for user {user_id}: {str(e)}",
            exc_info=True
        )
        raise OrderProcessingError(f"Unexpected error: {str(e)}")

# ================================================================
# CRITIC'S REVIEW OF VERSION 1
# ================================================================

# Performance Review:
# ✅ Fixed N+1 query with prefetch_related
# ✅ Used select_for_update for row-level locking
# ✅ Single query for total calculation using aggregate
# ⚠️ Could add caching for frequently used products
# ⚠️ Consider bulk_create for order items

# Error Handling Review:
# ✅ Transaction atomic ensures rollback on any failure
# ✅ Specific exceptions for different error types
# ✅ Structured logging with extra context
# ⚠️ Consider adding more validation for edge cases (negative quantities)

# Security Review:
# ✅ No SQL injection vulnerability
# ✅ Input validation implemented
# ✅ Transaction isolation prevents race conditions

# Maintainability Review:
# ✅ Clear function with docstring
# ✅ Type hints for better readability
# ✅ Logging for monitoring and debugging

# Additional Optimization Opportunities:
# 1. Batch inventory updates using bulk_update
# 2. Add distributed locking for microservices architecture
# 3. Implement circuit breaker for payment gateway
# 4. Add metrics collection for monitoring

# ================================================================
# VERSION 2 - OPTIMIZED PRODUCTION CODE
# ================================================================

from django.db import transaction, models
from django.core.exceptions import ValidationError
from django.conf import settings
import logging
import json
import time
from typing import Optional, Dict, Any, List, Tuple
from dataclasses import dataclass
from contextlib import contextmanager
from prometheus_client import Counter, Histogram

# Prometheus metrics
order_processing_time = Histogram('order_processing_seconds', 'Time to process order')
order_processed_counter = Counter('order_processed_total', 'Total orders processed')
order_failure_counter = Counter('order_failure_total', 'Total order failures', ['error_type'])

logger = logging.getLogger(__name__)

class OrderProcessingError(Exception):
    """Custom exception for order processing errors."""
    pass

class PaymentFailedError(Exception):
    """Payment processing failed."""
    pass

class InventoryInsufficientError(Exception):
    """Insufficient stock for order."""
    pass

@dataclass
class OrderResult:
    """Immutable result of order processing."""
    order_id: int
    total: float
    status: str
    items_count: int
    processing_time_ms: float

@contextmanager
def measure_performance(metric_name):
    """Context manager for performance measurement."""
    start = time.perf_counter()
    try:
        yield
    finally:
        duration = (time.perf_counter() - start) * 1000
        order_processing_time.observe(duration / 1000)  # Convert to seconds

def process_order_production(order_data: Dict[str, Any]) -> Optional[OrderResult]:
    """
    Production-ready order processing with comprehensive error handling,
    performance optimizations, and monitoring.
    
    Args:
        order_data: Dict containing 'user_id' and 'payment_method'
        
    Returns:
        OrderResult with order details or None
        
    Raises:
        OrderProcessingError: For fatal processing errors
    """
    
    with measure_performance('process_order'):
        # 1. Input validation
        user_id = order_data.get('user_id')
        payment_method = order_data.get('payment_method', 'default')
        
        if not user_id or not isinstance(user_id, int):
            raise ValidationError("Valid user_id is required")
        
        # 2. Get database connection with optimized settings
        from django.db import connection, transaction
        
        try:
            with transaction.atomic():
                # Use select_for_update to lock user row
                user = User.objects.select_for_update(skip_locked=True).get(id=user_id)
                if not user:
                    order_failure_counter.labels(error_type='user_not_found').inc()
                    return None
                
                # Optimized cart query with all necessary data
                cart = (Cart.objects
                       .select_for_update(skip_locked=True)
                       .filter(user=user, active=True)
                       .prefetch_related(
                           models.Prefetch(
                               'items',
                               queryset=CartItem.objects.select_related('product')
                           )
                       )
                       .first())
                
                if not cart or not cart.items.exists():
                    order_failure_counter.labels(error_type='empty_cart').inc()
                    logger.warning(f"No active cart found for user {user_id}")
                    return None
                
                # 3. Calculate total efficiently
                total = cart.items.aggregate(
                    total=models.Sum(models.F('product__price') * models.F('quantity'))
                )['total'] or 0
                
                if total <= 0:
                    raise ValidationError("Order total must be greater than 0")
                
                # 4. Batch inventory check and update
                cart_items = list(cart.items.all())
                products = Product.objects.filter(
                    id__in=[item.product_id for item in cart_items]
                ).select_for_update(skip_locked=True)
                
                product_map = {p.id: p for p in products}
                inventory_updates = []
                
                for item in cart_items:
                    product = product_map.get(item.product_id)
                    if not product:
                        raise InventoryInsufficientError(
                            f"Product {item.product_id} not found"
                        )
                    if product.stock < item.quantity:
                        raise InventoryInsufficientError(
                            f"Insufficient stock for product {product.id}"
                        )
                    product.stock -= item.quantity
                    inventory_updates.append(product)
                
                # 5. Bulk update inventory (single query)
                Product.objects.bulk_update(inventory_updates, ['stock'])
                
                # 6. Create order
                order = Order.objects.create(
                    user=user, 
                    total=total,
                    status='pending_payment'
                )
                
                # 7. Create order items in bulk
                order_items = [
                    OrderItem(
                        order=order,
                        product=item.product,
                        quantity=item.quantity,
                        price_at_time=item.product.price
                    )
                    for item in cart_items
                ]
                OrderItem.objects.bulk_create(order_items)
                
                # 8. Process payment (async or queue)
                try:
                    from payments.services import PaymentProcessor
                    processor = PaymentProcessor()
                    payment_result = processor.process_payment(
                        order_id=order.id,
                        amount=total,
                        method=payment_method,
                        user_id=user_id
                    )
                    
                    if not payment_result.success:
                        raise PaymentFailedError(
                            f"Payment failed: {payment_result.error}"
                        )
                    
                except Exception as e:
                    logger.error(
                        f"Payment failed for order {order.id}",
                        extra={'user_id': user_id, 'error': str(e)}
                    )
                    raise PaymentFailedError(f"Payment processing failed: {str(e)}")
                
                # 9. Update order status
                order.status = 'completed'
                order.payment_processed_at = timezone.now()
                order.save()
                
                # 10. Clear cart
                cart.active = False
                cart.save()
                
                # 11. Send confirmation (async)
                from tasks import send_order_confirmation
                send_order_confirmation.delay(order.id)
                
                # 12. Log and metrics
                logger.info(
                    f"Order {order.id} processed successfully",
                    extra={
                        'user_id': user_id,
                        'order_total': total,
                        'items_count': len(cart_items),
                        'payment_method': payment_method
                    }
                )
                
                order_processed_counter.inc()
                
                return OrderResult(
                    order_id=order.id,
                    total=total,
                    status=order.status,
                    items_count=len(cart_items),
                    processing_time_ms=0  # Updated by context manager
                )
                
        except (ValidationError, PaymentFailedError, InventoryInsufficientError) as e:
            order_failure_counter.labels(error_type=type(e).__name__).inc()
            logger.error(f"Business error for user {user_id}: {str(e)}")
            raise
        except Exception as e:
            order_failure_counter.labels(error_type='unexpected').inc()
            logger.error(
                f"Unexpected error for user {user_id
