# Module 3: Practical Prompt Design Techniques
## Professional Corporate Training Session

---

## 1. TOPIC OVERVIEW

### What is the Topic?

**Practical Prompt Design Techniques** are the specific strategies, methods, and frameworks you use to craft prompts that elicit the best possible responses from AI models. These techniques range from simple approaches (like zero-shot prompting) to sophisticated methods (like prompt chaining and step-by-step reasoning).

Think of it like a chef's toolkit—you have different knives for different purposes. A paring knife (zero-shot) works for simple tasks, while a chef's knife (few-shot) handles more complex preparations, and a full kitchen setup (prompt chaining) tackles elaborate multi-course meals.

**Real-World Analogy:** Imagine you're training a new employee. If you give them a task with no examples (zero-shot), they might struggle. If you show them one example (one-shot), they'll have a better idea. If you provide multiple examples (few-shot), they'll understand the pattern. If you make them role-play as a senior manager (persona-based), they'll adopt that perspective. And if you break a complex project into daily tasks (prompt chaining), they'll manage it step by step.

### Why is it Necessary?

**The Problem It Solves:**
- One prompt approach doesn't work for all scenarios
- Different tasks require different prompting strategies
- AI models respond differently to various techniques
- Without technique knowledge, you're limited to basic prompts

**Why Should Professionals Learn It:**
- **Versatility:** Apply the right technique to the right situation
- **Efficiency:** Get better results with fewer iterations
- **Precision:** Handle complex, multi-step tasks effectively
- **Control:** Guide AI reasoning and response quality
- **Innovation:** Unlock advanced AI capabilities

**Business Value:**
- 50-80% improvement in output quality with the right technique
- Ability to handle 10x more complex tasks
- Reduced dependency on technical AI knowledge
- Standardized methodology across teams
- Faster AI adoption and ROI realization

---

## 2. CONCEPT EXPLANATION

### Basic Understanding

Prompt design techniques are the practical methods you apply to structure your prompts for optimal results. Each technique serves a specific purpose and works best for particular types of tasks.

### Key Techniques Explained

#### 1. Zero-Shot Prompting
**Definition:** Asking the AI to perform a task without providing any examples. The model relies entirely on its training data.

**When to Use:** Simple, common tasks the AI likely understands well.

**Example:**
```
Translate the following text to Spanish:
"Hello, how are you today?"
```

#### 2. One-Shot Prompting
**Definition:** Providing exactly one example of the desired input-output pair before giving the actual task.

**When to Use:** When you need to demonstrate a specific format or pattern.

**Example:**
```
Example: Question: "What is the capital of France?" → Answer: "Paris"

Now answer: Question: "What is the capital of Japan?" → Answer:
```

#### 3. Few-Shot Prompting
**Definition:** Providing multiple examples (typically 2-5) to demonstrate the pattern, format, and quality expected.

**When to Use:** Complex tasks, specific formats, when quality consistency matters.

**Example:**
```
Examples of product descriptions:
Product: Bamboo Water Bottle → "Eco-friendly, lightweight, perfect for on-the-go..."
Product: Wireless Earbuds → "Crystal clear sound, noise-canceling, 8-hour battery..."

Now describe: Product: Smart Fitness Watch →
```

#### 4. Instruction-Based Prompting
**Definition:** Explicitly telling the AI what to do and often how to do it using clear, step-by-step instructions.

**When to Use:** Most business applications, when you need specific structure or approach.

**Example:**
```
Task: Create a business email
Instructions:
1. Start with a professional greeting
2. State the purpose clearly in the first sentence
3. Provide key details in bullet points
4. End with a call-to-action and sign-off
```

#### 5. Persona-Based Prompting
**Definition:** Assigning a specific role, personality, or perspective to the AI to shape its responses.

**When to Use:** When tone, expertise, or perspective matters significantly.

**Example:**
```
Act as a Senior Financial Advisor with 15 years of experience.
Provide investment advice to a 35-year-old professional...
```

#### 6. Comparative Prompting
**Definition:** Asking the AI to compare, contrast, or evaluate multiple options, perspectives, or scenarios.

**When to Use:** Decision-making, analysis, evaluation tasks.

**Example:**
```
Compare the following three marketing strategies:
Strategy A, Strategy B, Strategy C
Analyze pros, cons, and recommend one with justification.
```

#### 7. Delimiters
**Definition:** Using special characters or formatting (---, ###, quotes, brackets) to separate different parts of the prompt.

**When to Use:** Complex prompts with multiple sections, when you need to clearly distinguish content.

**Example:**
```
### Context ###
We are a B2B SaaS company...
### Task ###
Please analyze...
### Example ###
...
```

#### 8. Context Injection
**Definition:** Strategically placing contextual information at specific points in the prompt to maximize relevance.

**When to Use:** When the AI needs background information to generate appropriate responses.

**Example:**
```
Before answering the question below, know that...
[Context information]
Now, given this context, respond to:
[Question or task]
```

#### 9. Multi-Step Prompting
**Definition:** Breaking a complex task into multiple, sequential prompts or instructions within a single prompt.

**When to Use:** Complex analysis, problem-solving, or creation tasks.

**Example:**
```
Step 1: Analyze the following customer feedback data
Step 2: Identify top 3 complaints
Step 3: Recommend solutions for each
Step 4: Create an action plan
```

#### 10. Step-by-Step Reasoning (Chain of Thought)
**Definition:** Asking the AI to show its reasoning process step by step before providing the final answer.

**When to Use:** Complex reasoning, math, logic, analysis tasks.

**Example:**
```
Please solve this problem step by step:
[Problem]
Show your reasoning at each step before providing the final answer.
```

#### 11. Prompt Chaining
**Definition:** Using the output of one prompt as the input for another prompt in a sequence, building towards a final result.

**When to Use:** Very complex, multi-stage tasks that benefit from intermediate results.

**Example:**
```
Prompt 1: Research top market trends
Prompt 2: Based on these trends, identify opportunities
Prompt 3: Based on opportunities, create a strategy
```

### How AI Interprets These Techniques

**Why Technique Choice Matters:**
- **Zero-shot:** AI relies on general training; may make assumptions
- **Few-shot:** AI learns pattern from examples; more accurate
- **Persona:** AI adopts language, tone, and perspective
- **Step-by-step:** AI engages in more deliberate, accurate reasoning
- **Chaining:** AI builds on previous outputs, cumulative quality

**AI's Process with Different Techniques:**
1. **Zero-shot:** "I know what to do from my training"
2. **Few-shot:** "I see the pattern, let me follow it"
3. **Persona:** "I am this person, let me speak as them"
4. **Chain of thought:** "Let me think through this logically"
5. **Chaining:** "This previous output guides what I do next"

### Best Practices

1. **Start with zero-shot** for simple tasks; add examples if needed
2. **Use 2-4 examples** in few-shot prompting—more can confuse
3. **Be specific with personas** (Senior, years of experience, domain)
4. **Use delimiters** for clarity in complex prompts
5. **Chain reasoning** for complex analytical tasks
6. **Inject context** at the right point for relevance
7. **Break complex tasks** into manageable steps
8. **Test different techniques** to find what works best

### Common Mistakes to Avoid

| Mistake | Why It's a Problem | Better Approach |
|---------|-------------------|-----------------|
| Using zero-shot for complex tasks | AI lacks guidance for nuanced requirements | Use few-shot or multi-step |
| Too many examples in few-shot | Confuses the AI, reduces quality | Use 2-4 high-quality examples |
| Generic personas | AI doesn't adopt a useful perspective | Specific role + expertise + experience |
| No reasoning steps | AI jumps to conclusions | Ask for step-by-step reasoning |
| Not chaining complex tasks | AI can't handle complexity in one pass | Break into multiple prompts |

### Advanced Considerations

**When to Combine Techniques:**
- **Persona + Few-shot:** For expert-level outputs with examples
- **Chain of thought + Context injection:** For reasoning with background
- **Multi-step + Delimiters:** For complex structured tasks
- **Prompt chaining + Persona:** For maintaining consistency across chain

**Choosing the Right Technique:**

| Task Type | Recommended Technique |
|-----------|----------------------|
| Simple Q&A | Zero-shot |
| Format-specific tasks | Few-shot (2-3 examples) |
| Expert analysis | Persona + Chain of thought |
| Complex creation | Multi-step + Context injection |
| Multi-stage projects | Prompt chaining |
| Decision-making | Comparative + Chain of thought |

---

## 3. PRACTICAL EXAMPLE

### Example 1: Simple Beginner Example

**Scenario:** A content writer needs to generate social media posts about sustainable fashion.

**Technique:** Zero-shot vs Few-shot comparison

**Input (Zero-Shot):**
```
Write an Instagram caption for a sustainable fashion brand.
```

**Process:**
- AI relies on general knowledge about sustainable fashion
- Generates a generic caption without specific brand voice
- May be too general or miss specific brand elements

**Expected Output (Zero-Shot):**
```
🌿 Sustainable fashion is more than a trend—it's a movement! 
Choose eco-friendly materials that love our planet as much as you do. 
Made with care, designed to last. #SustainableFashion #EcoStyle
```

---

**Input (Few-Shot - Refined):**
```
Write an Instagram caption for our sustainable fashion brand "EcoChic".

Examples of our successful posts:
Post 1: "♻️ Every thread tells a story of change. Our new collection uses 100% organic cotton—saving 2,700 liters of water per t-shirt. Wear the change. #EcoChic #SustainableFashion"

Post 2: "🌍 Fast fashion is out. Thoughtful style is in. Our fall collection is crafted from recycled ocean plastics, transforming waste into wardrobe essentials. 💙 #EcoChic #CircularFashion"

Post 3: "👗 Did you know? Each EcoChic dress saves 5kg of textile waste from landfills. This is fashion that gives back. Join the revolution. 🌿 #EcoChic #ZeroWaste"

Now write a new caption about our new bamboo fiber collection launching next week.
Use our brand voice: inspiring, informative, sustainable-focused, with a call to action.
Include hashtags and emojis.
```

**Process:**
- AI learns brand voice from examples
- Understands specific format (hook + fact + call to action + hashtags)
- Applies the pattern to the new collection
- Maintains consistent branding

**Expected Output (Few-Shot):**
```
🎋 Bamboo isn't just for pandas anymore—it's fashion's sustainable future!

Our new EcoChic bamboo fiber collection is launching next week, and we're obsessed. Why? 
🌱 Bamboo grows 3 feet per day—it's nature's fastest regenerating resource
💧 Uses 70% less water than conventional cotton
♻️ Biodegradable and naturally antibacterial

This isn't just fashion. It's a promise to our planet.

Be part of the story. 🌿 
Sign up for early access at the link in bio! 👆

#EcoChic #BambooFashion #SustainableStyle #EcoFriendly #SlowFashion #ConsciousConsumer
```

---

### Example 2: Business Example

**Scenario:** A product team needs to prioritize features for next quarter's roadmap.

**Technique:** Multi-step + Comparative prompting

**Input:**
```
Role: Senior Product Manager
Task: Prioritize 6 proposed features for our project management SaaS tool

Context:
- Tool: "TaskFlow" serves 50,000+ users across 5,000 companies
- Current pain points: Users want better reporting and automation
- Resources: 1 development team (6 engineers) for next quarter (12 weeks)
- User segments: Enterprise (40%), SMB (45%), Freelance (15%)
- Revenue impact: Each feature must contribute to retention or acquisition

Features to prioritize:
A) Advanced Analytics Dashboard (8 weeks, high complexity)
B) Automated Workflow Builder (6 weeks, medium complexity)
C) Gantt Chart View (4 weeks, low complexity)
D) Custom Report Builder (5 weeks, medium complexity)
E) Team Collaboration Chat (10 weeks, very high complexity)
F) AI-Powered Task Prioritization (7 weeks, high complexity)

Instructions:
1. Analyze each feature against key criteria:
   - User demand (based on feedback data)
   - Development effort
   - Revenue impact potential
   - Strategic importance
2. Compare and rank the features
3. Recommend top 3 features for next quarter
4. Create a phased implementation timeline for your recommendations
5. Provide justification for rejected features

Constraints:
- Must deliver at least one high-impact feature
- Must consider both enterprise and SMB needs
- Development team cannot be over capacity
- Maximum 500 words

Output Format: Use this structure:
# Q4 Feature Prioritization
## Ranking and Scores
## Recommended Features (Top 3)
## Implementation Timeline
## Rejected Features Justification
## Summary & Recommendation
```

**Process:**
1. Sets role (Senior PM) for expert perspective
2. Provides comprehensive context (tool, users, resources)
3. Lists all features with complexity estimates
4. Gives multi-step instructions (analyze, compare, recommend, timeline, justify)
5. Sets constraints (high-impact, consider all segments, capacity, length)
6. Defines clear output structure

**Expected Output:**
```markdown
# Q4 Feature Prioritization
## Ranking and Scores

| Feature | User Demand (1-10) | Dev Effort (Weeks) | Revenue Impact (1-10) | Strategic Value (1-10) | Composite Score |
|---------|-------------------|-------------------|----------------------|----------------------|-----------------|
| Advanced Analytics Dashboard | 9 | 8 | 8 | 9 | 8.5 |
| Automated Workflow Builder | 7 | 6 | 7 | 9 | 7.5 |
| Gantt Chart View | 8 | 4 | 6 | 6 | 6.8 |
| Custom Report Builder | 9 | 5 | 8 | 7 | 8.3 |
| Team Collaboration Chat | 6 | 10 | 5 | 6 | 5.8 |
| AI-Powered Task Prioritization | 8 | 7 | 9 | 9 | 8.6 |

## Recommended Features (Top 3)

### 1. AI-Powered Task Prioritization (Priority #1)
**Why:** Highest strategic value and revenue impact potential. This feature differentiates us from competitors and addresses a key pain point for all segments.
**Investment:** 7 weeks (team capacity)
**Expected Impact:** +15% premium subscription upgrades, +10% NPS

### 2. Advanced Analytics Dashboard (Priority #2)
**Why:** Highest user demand, serves both enterprise (complex needs) and SMB (simplified views). Unlocks upsell opportunities.
**Investment:** 8 weeks (parallel development)
**Expected Impact:** +20% retention rate, key differentiator

### 3. Custom Report Builder (Priority #3)
**Why:** Enterprise users specifically requesting this. Complements Advanced Analytics Dashboard. 
**Investment:** 5 weeks
**Expected Impact:** +8% revenue from enterprise segment

## Implementation Timeline

**Weeks 1-3:** AI-Powered Task Prioritization (Planning & Architecture)
**Weeks 4-7:** AI-Powered Task Prioritization (Development) + Start Analytics Dashboard
**Weeks 8-10:** Analytics Dashboard (Continued) + Custom Report Builder (Start)
**Weeks 11-12:** All three - Testing, Documentation, Deployment

**Total Commitment:** 12 weeks, 6 engineers
**Buffer:** 1 week spare capacity for bug fixes

## Rejected Features Justification

- **Gantt Chart View:** While in high demand, it's lower strategic value. Consider moving to Q2 next year with some team capacity. 
- **Team Collaboration Chat:** Too high complexity with lower revenue impact. This is better handled through integrations with existing tools (Slack, Teams) rather than building in-house. 

## Summary & Recommendation

Prioritize AI-Powered Task Prioritization, Advanced Analytics Dashboard, and Custom Report Builder this quarter. This combination maximizes revenue impact (AI + analytics) while building strategic differentiation. The features work synergistically—advanced analytics provides data, AI prioritizes tasks based on that data, and custom reporting visualizes the results. 
```

---

### Example 3: Technical Example

**Scenario:** A developer needs to refactor code with proper error handling and optimization.

**Technique:** Persona + Chain of Thought + Context Injection

**Input:**
```
Act as a Senior Software Engineer with 10+ years of Python experience, 
specializing in API development and performance optimization.

CONTEXT:
The following function is part of a customer management system serving 100,000+ 
requests per day. We've identified it as a performance bottleneck and a source 
of several production bugs.

INSTRUCTIONS:
Analyze the code below step by step:

1. First, identify all issues in the current code (performance, security, readability, error handling)
2. Then, refactor the code to address these issues
3. Explain your reasoning for each change
4. Add comprehensive error handling and logging
5. Include optimization suggestions for high-traffic scenarios
6. Write unit tests for critical parts

CURRENT CODE:
```python
def update_customer_data(customer_id, data):
    import json
    conn = get_db_connection()
    cursor = conn.cursor()
    cursor.execute(f"SELECT * FROM customers WHERE id = {customer_id}")
    result = cursor.fetchone()
    if result:
        for key, value in data.items():
            cursor.execute(f"UPDATE customers SET {key} = '{value}' WHERE id = {customer_id}")
    conn.commit()
    conn.close()
    return True
```

CONSTRAINTS:
- Must handle SQL injection vulnerabilities
- Must work with PostgreSQL
- Must be production-ready
- Include proper transaction management
- Add comments explaining optimization decisions

OUTPUT FORMAT:
Provide the response in four sections:
1. Code Analysis (issues identified)
2. Refactored Code (complete new version)
3. Change Reasoning (explain each change)
4. Test Cases (unit tests)
```

**Process:**
1. Senior Engineer role sets high expertise expectation
2. Context explains the production importance
3. Step-by-step instructions guide thorough analysis
4. Security/optimization constraints ensure quality
5. Structured output format ensures completeness

**Expected Output:**
```python
"""
CODE ANALYSIS - Issues Identified:

1. **SQL Injection Vulnerability**: Using f-strings with user input directly
2. **No Error Handling**: No try/except blocks, failing silently
3. **Inefficient Updates**: One UPDATE per field instead of one UPDATE for all fields
4. **No Connection Management**: Not using context managers
5. **No Transaction Management**: Committing changes without rollback on error
6. **No Input Validation**: Not checking customer_id or data structure
7. **Always Returns True**: Even when no changes were made
8. **No Logging**: No visibility into operations
9. **Unsafe Import Placement**: Import inside function, bad practice
10. **No Type Hints**: Makes code harder to understand and maintain
"""

import logging
import json
from typing import Dict, Any, Optional
import psycopg2
from psycopg2 import sql
from psycopg2.extras import RealDictCursor

# Configure logging
logging.basicConfig(
    level=logging.INFO,
    format='%(asctime)s - %(levelname)s - %(message)s',
    handlers=[logging.StreamHandler()]
)
logger = logging.getLogger(__name__)

class CustomerDataUpdateError(Exception):
    """Custom exception for customer data update failures."""
    pass

def update_customer_data(
    customer_id: int, 
    data: Dict[str, Any],
    db_config: Optional[Dict[str, str]] = None
) -> bool:
    """
    Update customer data with proper error handling and SQL injection protection.
    
    Args:
        customer_id: The ID of the customer to update
        data: Dictionary of field:value pairs to update
        db_config: Optional database configuration override
        
    Returns:
        bool: True if update was successful
        
    Raises:
        CustomerDataUpdateError: If the update fails
        ValueError: If input validation fails
    """
    
    # Input validation
    if not isinstance(customer_id, int) or customer_id <= 0:
        raise ValueError(f"Invalid customer_id: {customer_id}")
    
    if not data or not isinstance(data, dict):
        raise ValueError("Data must be a non-empty dictionary")
    
    # Sanitize field names to prevent injection
    allowed_fields = {'name', 'email', 'phone', 'address', 'status', 'updated_at'}
    sanitized_data = {k: v for k, v in data.items() if k in allowed_fields}
    
    if not sanitized_data:
        logger.warning(f"No valid fields to update for customer {customer_id}")
        return False
    
    # Build dynamic update query with parameterized placeholders
    set_clauses = []
    params = []
    
    for key, value in sanitized_data.items():
        set_clauses.append(sql.Identifier(key) + sql.SQL(' = %s'))
        params.append(value)
    
    params.append(customer_id)
    
    query = sql.SQL("""
        UPDATE customers 
        SET {fields}
        WHERE id = %s
        RETURNING id, updated_at
    """).format(
        fields=sql.SQL(', ').join(set_clauses)
    )
    
    conn = None
    cursor = None
    
    try:
        # Use context manager for connection
        conn = get_db_connection(db_config)
        
        # Use autocommit=False for transaction control
        conn.autocommit = False
        cursor = conn.cursor(cursor_factory=RealDictCursor)
        
        # Execute with proper parameterization
        cursor.execute(query, params)
        
        # Check if any rows were affected
        result = cursor.fetchone()
        
        if not result:
            logger.warning(f"No customer found with ID: {customer_id}")
            conn.rollback()
            return False
        
        # Log success with customer ID and timestamp
        logger.info(
            f"Customer {customer_id} updated successfully. "
            f"Updated at: {result['updated_at']}"
        )
        
        # Commit the transaction
        conn.commit()
        return True
        
    except psycopg2.IntegrityError as e:
        logger.error(f"Integrity error updating customer {customer_id}: {str(e)}")
        if conn:
            conn.rollback()
        raise CustomerDataUpdateError(f"Data integrity error: {str(e)}")
        
    except psycopg2.Error as e:
        logger.error(f"Database error updating customer {customer_id}: {str(e)}")
        if conn:
            conn.rollback()
        raise CustomerDataUpdateError(f"Database error: {str(e)}")
        
    except Exception as e:
        logger.error(f"Unexpected error updating customer {customer_id}: {str(e)}")
        if conn:
            conn.rollback()
        raise CustomerDataUpdateError(f"Unexpected error: {str(e)}")
        
    finally:
        if cursor:
            cursor.close()
        if conn:
            conn.close()
            logger.debug(f"Database connection closed for customer {customer_id}")

"""
CHANGE REASONING:

1. **SQL Injection Protection**: Used parameterized queries (%s placeholders) instead of f-strings
2. **Error Handling**: Comprehensive try/except blocks with rollback on failure
3. **Bulk Update**: Single UPDATE statement vs multiple
4. **Context Managers**: Ensures connections are properly closed
5. **Transaction Management**: Explicit commit/rollback control
6. **Input Validation**: Validates customer_id and data structure
7. **Return Values**: Accurate return based on operation success
8. **Logging**: Comprehensive logging for debugging and monitoring
9. **Type Hints**: Improved code clarity and IDE support
10. **Custom Exceptions**: Specific error types for better error handling
11. **Field Whitelist**: Prevents injection through field names
12. **Returning Clause**: Gets confirmation of update with timestamp

PERFORMANCE OPTIMIZATIONS FOR HIGH TRAFFIC (100,000+ req/day):
1. **Connection Pooling**: Use psycopg2's pool module
2. **Batch Updates**: Consider bulk_update for multiple customers
3. **Query Caching**: Cache SELECT results if needed
4. **Indexes**: Ensure indexes on id, updated_at fields
5. **Read Replicas**: Route SELECT queries to replica
6. **Monitoring**: Add performance metrics collection
"""

# UNIT TESTS
import unittest
from unittest.mock import Mock, patch

class TestUpdateCustomerData(unittest.TestCase):
    
    def setUp(self):
        self.valid_customer_id = 12345
        self.valid_data = {
            'name': 'John Doe',
            'email': 'john@example.com',
            'status': 'active'
        }
    
    @patch('path.to.get_db_connection')
    def test_successful_update(self, mock_get_db):
        """Test successful customer update."""
        # Mock database connection and cursor
        mock_conn = Mock()
        mock_cursor = Mock()
        mock_cursor.fetchone.return_value = {'id': 12345, 'updated_at': '2024-01-01'}
        mock_conn.cursor.return_value = mock_cursor
        mock_get_db.return_value = mock_conn
        
        result = update_customer_data(self.valid_customer_id, self.valid_data)
        self.assertTrue(result)
        mock_conn.commit.assert_called_once()
    
    @patch('path.to.get_db_connection')
    def test_invalid_customer_id(self, mock_get_db):
        """Test validation with invalid customer ID."""
        with self.assertRaises(ValueError):
            update_customer_data(-1, self.valid_data)
        
        with self.assertRaises(ValueError):
            update_customer_data(0, self.valid_data)
    
    def test_empty_data(self):
        """Test with empty data dictionary."""
        result = update_customer_data(self.valid_customer_id, {})
        self.assertFalse(result)
    
    def test_invalid_data_type(self):
        """Test with invalid data type."""
        with self.assertRaises(ValueError):
            update_customer_data(self.valid_customer_id, "not a dict")
    
    @patch('path.to.get_db_connection')
    def test_database_error(self, mock_get_db):
        """Test database error handling."""
        mock_conn = Mock()
        mock_cursor = Mock()
        mock_cursor.execute.side_effect = Exception("Database connection failed")
        mock_conn.cursor.return_value = mock_cursor
        mock_get_db.return_value = mock_conn
        
        with self.assertRaises(CustomerDataUpdateError):
            update_customer_data(self.valid_customer_id, self.valid_data)
        
        mock_conn.rollback.assert_called_once()
    
    @patch('path.to.get_db_connection')
    def test_customer_not_found(self, mock_get_db):
        """Test when customer ID doesn't exist."""
        mock_conn = Mock()
        mock_cursor = Mock()
        mock_cursor.fetchone.return_value = None
        mock_conn.cursor.return_value = mock_cursor
        mock_get_db.return_value = mock_conn
        
        result = update_customer_data(self.valid_customer_id, self.valid_data)
        self.assertFalse(result)
        mock_conn.rollback.assert_called_once()

if __name__ == '__main__':
    unittest.main()
```

---

## 4. SUGGESTED PROMPT TEMPLATE

### Universal Prompt Design Template

```
[ROLE]
Act as a [expert role] with [X] years of experience in [domain].
Your expertise includes [specific skills/areas].

[CONTEXT]
Organization: [Company/Team description]
Industry: [Sector]
Current Situation: [Background and circumstances]
Target Audience: [Who this is for]
Key Considerations: [Important factors to consider]

[TASK]
Please [specific action] to [desired outcome].

[INSTRUCTIONS]
1. [Step 1]
2. [Step 2] 
3. [Step 3]
4. [Step 4 (optional)]
5. [Step 5 (optional)]

[CONSTRAINTS]
- Tone: [Professional/Conversational/Formal/etc.]
- Length: [Word/section limit]
- Must Include: [Mandatory elements]
- Must Exclude: [Prohibited content]
- Additional: [Other constraints]

[EXAMPLES] (For few-shot prompting)
Example 1:
Input: [Sample input]
Output: [Sample output]

Example 2:
Input: [Sample input]
Output: [Sample output]

Example 3 (optional):
Input: [Sample input]
Output: [Sample output]

[OUTPUT FORMAT]
# [Main Heading]

## [Section 1]
[Content description]

## [Section 2]
[Content description]

### [Subsection]
[Content description]

[Additional sections as needed]

[DATA or ADDITIONAL CONTEXT TO INJECT]
[Insert any relevant data, documents, or context here]
```

### Technique Selection Guide

| If you need... | Use this technique | How to apply |
|----------------|-------------------|--------------|
| Quick, simple answer | Zero-shot | Direct question/request |
| Specific format matching | One-shot | 1 example + task |
| Consistent quality/format | Few-shot | 2-4 examples + task |
| Detailed guidance | Instruction-based | Clear numbered steps |
| Expert perspective | Persona-based | Detailed role description |
| Decision support | Comparative | Multiple options + criteria |
| Clear structure | Delimiters | ### Sections ### |
| Relevant background | Context injection | Context before task |
| Complex task completion | Multi-step | Sequential steps in one prompt |
| Logical reasoning | Step-by-step | "Show your reasoning" |
| Multi-stage project | Prompt chaining | Split into multiple prompts |

---

## 5. COMPLETE SAMPLE PROMPT

### Production-Ready Prompt: Competitive Analysis Report

```
ROLE:
Act as a Senior Market Intelligence Analyst with 8 years of experience in B2B SaaS competitive analysis. You have conducted competitive analyses for 15+ tech companies, including 3 that achieved unicorn status.

CONTEXT:
Organization: CloudOps AI - A Series B SaaS company providing AI-powered cloud infrastructure optimization. We help companies reduce cloud costs by 25-40% through intelligent resource management.
Industry: B2B Cloud Infrastructure / FinOps
Current Situation: We're launching "Optimize Pro 3.0" - our next-gen platform with enhanced cost prediction and automated rightsizing. Our main competitors are AWS Cost Explorer, CloudHealth, and CloudCheckr.
Target Audience: VP of Cloud Operations, CTO, Cloud Architects at mid-large enterprises
Key Considerations: We need to differentiate clearly, identify gaps in competitors' offerings, and position our AI capabilities as superior.

TASK:
Create a comprehensive competitive analysis report comparing CloudOps AI Optimize Pro 3.0 against our three main competitors.

INSTRUCTIONS:
1. Analyze each competitor's core offering and key features
2. Create a feature-by-feature comparison matrix (include at least 10 features)
3. Identify 3 clear differentiators for CloudOps AI
4. Identify 2 competitive gaps we can exploit
5. Recommend pricing positioning based on competitor analysis
6. Create a "win" strategy for each competitor
7. Provide a SWOT analysis for CloudOps AI relative to the market

CONSTRAINTS:
- Tone: Strategic, data-driven, confident, slightly sales-oriented
- Length: Maximum 1,200 words
- Format: Use markdown tables for comparisons
- Must Include: Executive summary, pricing intelligence
- Must Exclude: Generic competitive advice, emotional language
- Data Sources: Reference our internal sales data and public competitor information
- Deadline: This report will be presented to the Board next week

EXAMPLES:
Example of preferred section:
"Their RTS (Real-Time Savings) metric is outdated—recording savings weekly. Our AI provides hourly optimization recommendations, capturing 40% more savings opportunities."

OUTPUT FORMAT:
Provide the response in the following structure:

# Competitive Analysis Report: Optimize Pro 3.0 Launch

## Executive Summary
[3-4 sentences summarizing key findings and recommendation]

## Competitor Overview
### Competitor 1: AWS Cost Explorer
### Competitor 2: CloudHealth by VMware
### Competitor 3: CloudCheckr

## Feature Comparison Matrix
| Feature | AWS Cost Explorer | CloudHealth | CloudCheckr | CloudOps AI |
|---------|-------------------|-------------|-------------|-------------|
| Feature 1 | Rating | Rating | Rating | Rating |
| [10+ features listed] | | | | |

## Key Differentiators (Our Advantage)
1. [Differentiator 1 with explanation]
2. [Differentiator 2 with explanation] 
3. [Differentiator 3 with explanation]

## Competitive Gaps to Exploit
1. [Gap 1 - Competitor weakness]
2. [Gap 2 - Competitor weakness]

## Pricing Positioning Analysis
[Analysis with recommended pricing strategy]

## Competitor-Specific Win Strategies
### Against AWS Cost Explorer
### Against CloudHealth
### Against CloudCheckr

## SWOT Analysis: CloudOps AI
| Strengths | Weaknesses |
|-----------|------------|
| [List] | [List] |
| **Opportunities** | **Threats** |
| [List] | [List] |

## Strategic Recommendations
[3-4 actionable recommendations]

---

Please start your response with: "Based on our comprehensive competitive analysis, here are the key insights for positioning Optimize Pro 3.0 for market success:"
```

---

## 6. 4-LINE USE CASE STUDY

**Scenario:** Product team struggling to prioritize customer feedback, spending 10+ hours manually analyzing and categorizing 500+ survey responses per quarter.

**Goal:** Create a few-shot prompting system to automatically categorize and prioritize customer feedback into actionable insights within 2 hours.

**Technique Applied:** Few-shot prompting with 5 examples + Step-by-step reasoning with category definitions and priority scoring.

**Result:** Feedback processing time reduced by 80%, priority accuracy improved from 65% to 92%, and team now handles analysis in 1.5 hours with 4x more detail.

---

## 7. HANDS-ON TASKS

### Beginner Tasks

**1. Technique Identification**
Read the following prompts and identify which technique(s) are being used:

Prompt A: *"Summarize this article in 3 sentences."*
Prompt B: *"Act as a Financial Advisor. Here are two investment strategies. Compare them and recommend one."* 
Prompt C: *"Example: 'Meeting at 3pm' → 'You have a meeting scheduled for 3:00 PM.' Now convert: 'Dr. appt 2:30 Thurs'"*
Prompt D: *"Step 1: Read the document. Step 2: Identify key issues. Step 3: Recommend solutions."*

**Deliverable:**
- Identify the technique for each prompt
- Explain why you identified it as such
- Provide one alternative technique for each

**2. Zero-Shot to Few-Shot Transformation**
Take this zero-shot prompt and convert it to a few-shot prompt:

*"Write a customer support response for a user complaining about a delayed delivery."*

**Deliverable:**
- Create the original zero-shot version
- Create a few-shot version with 3 examples of good customer support responses
- Compare and explain why the few-shot version would produce better results

**3. Persona Creation**
Create a detailed persona for the following scenario:

*"I need to create a marketing plan for a new energy drink targeting Gen Z."*

**Deliverable:**
- Define a specific persona (role, age, experience, expertise, perspective)
- Write a prompt that includes the persona
- Explain how the persona affects the AI's response quality

### Intermediate Tasks

**1. Multi-Technique Prompt**
Combine 3 different prompting techniques into a single prompt:

**Task:** Write a comprehensive business case for adopting a new HR software system.

**Required Techniques:**
1. Persona-based (Act as HR Director)
2. Instruction-based (5 clear steps)
3. Comparative (Analyze 2 alternatives)

**Deliverable:**
- Complete prompt using all 3 techniques
- Explanation of why each technique is appropriate
- Expected output example

**2. Prompt Chaining Scenario**
Design a 3-prompt chain for:

**Task:** Create a full content marketing strategy (topic research → content creation → distribution plan)

**Deliverable:**
- Prompt 1: Topic research and keyword identification
- Prompt 2: Content creation (with context from Prompt 1)
- Prompt 3: Distribution and promotion plan (with context from Prompt 2)
- Explanation of how information flows between prompts
- Instructions for implementing the chain

### Advanced Task

**1. Complete Technique Library**
Create a comprehensive set of prompts for a complete business workflow:

**Business Case:** A product team needs to launch a new mobile app from ideation to launch strategy.

**Create 10 prompts using different techniques:**

| Step | Technique | Purpose |
|------|-----------|---------|
| 1 | Persona + Zero-shot | Market analysis |
| 2 | Few-shot (3 examples) | Feature list generation |
| 3 | Instruction-based | MVP definition |
| 4 | Chain of thought | Customer journey mapping |
| 5 | Comparative + Chain | Competitor analysis |
| 6 | Multi-step | Development roadmap |
| 7 | Context injection + Persona | Go-to-market strategy |
| 8 | Delimiters + Multi-step | User testing plan |
| 9 | Prompt chaining (2 prompts) | Marketing campaign |
| 10 | All techniques combined | Full launch presentation |

**Deliverable:**
- All 10 complete prompts
- Explanation of technique selection
- Expected output for each
- Implementation guide
- Metrics for success measurement
- A "Decision Tree" showing when to use each technique

**Evaluation Criteria:**
- Correct technique selection for each step
- Quality and clarity of prompts
- Logical flow between prompts
- Business relevance and applicability
- Explanation quality and depth

---

## 8. COMMON INTERVIEW QUESTIONS

### Beginner Interview Questions

**Q1: What is the difference between zero-shot, one-shot, and few-shot prompting?**

**Answer:**
- **Zero-shot:** No examples provided. The AI relies solely on its training to understand and perform the task. Example: "Translate this to Spanish."
- **One-shot:** One example is provided to demonstrate the desired input-output pattern. Example: "Example: Q: 'Capital of France?' → 'Paris'. Now answer: 'Capital of Japan?'"
- **Few-shot:** Two or more examples (typically 2-5) are provided to demonstrate the pattern, format, and quality expected. Example: Three examples of product descriptions before asking for a new one.

**Q2: What is persona-based prompting and why is it useful?**

**Answer:** Persona-based prompting assigns a specific role, perspective, or personality to the AI, such as "Act as a Senior Financial Analyst" or "You are a supportive career coach." It's useful because it:
- Sets the tone and expertise level
- Aligns the response with the target audience
- Provides a consistent voice across outputs
- Helps the AI adopt the appropriate vocabulary and depth of knowledge
- Makes responses more relevant and credible

**Q3: What is the purpose of using delimiters in a prompt?**

**Answer:** Delimiters (like ###, ---, """ , < >) serve to:
- Clearly separate different sections of the prompt
- Distinguish between instructions, context, data, and examples
- Reduce ambiguity about what text belongs to which part
- Help the AI parse and understand complex, multi-part prompts
- Make prompts more readable for both the AI and humans
- Prevent the AI from confusing instructions with content

### Intermediate Interview Questions

**Q1: When would you use prompt chaining instead of a single prompt with multiple steps?**

**Answer:** Choose prompt chaining over a single multi-step prompt when:
- **Complexity exceeds context window:** The task is too large for one prompt
- **Intermediate results matter:** You need to review or refine outputs between steps
- **Different expertise needed:** Different steps require different personas or perspectives
- **Multiple stakeholders involved:** Different people need to review different stages
- **Iterative refinement needed:** Outputs from one step inform and improve the next
- **Error handling:** You need to validate before proceeding to the next step
- **Efficiency:** Some steps may be reusable across different projects

**Example:** Creating an article: (1) Research outline → (2) Draft content → (3) Edit and polish. Each step benefits from fresh context and focused attention.

**Q2: How do you decide which prompting technique to use for a given task?**

**Answer:** Follow this decision framework:

1. **Assess task complexity:**
   - Simple/Q&A → Zero-shot
   - Moderately complex → One-shot or few-shot
   - Highly complex → Multi-step or chain of thought

2. **Evaluate format requirements:**
   - Need exact format → Few-shot
   - Need freeform response → Zero-shot or instruction-based
   - Need structured output → Instruction-based with delimiters

3. **Consider expertise need:**
   - General knowledge → Zero-shot
   - Specialized domain → Persona-based
   - Expert analysis → Persona + Chain of thought

4. **Analyze tone requirements:**
   - Neutral → Zero-shot
   - Specific brand voice → Persona + Few-shot
   - Persuasive → Comparative + Persona

5. **Account for resources:**
   - One-time use → Simpler technique
   - Repeated use → Invest in detailed templates
   - Team usage → Standardize with instruction-based

6. **Test and iterate:**
   - Start with simplest technique
   - Add complexity only if needed
   - Measure quality improvement

**Q3: Explain how you would combine chain of thought prompting with few-shot prompting for a complex reasoning task.**

**Answer:** Here's a combined approach:

1. **Create few-shot examples that include reasoning:**
   ```
   Example 1:
   Problem: A store has 15 apples, sells 5, gets 8 more. How many apples?
   Reasoning: Starts with 15. Sells 5: 15-5=10. Gets 8: 10+8=18.
   Answer: 18 apples.
   ```

2. **Provide 2-3 examples** with both reasoning and final answer

3. **Structure the final prompt:**
   ```
   Examples of solving problems step by step: 
   [Examples with reasoning]
   
   Now solve this new problem:
   [New problem]
   Please show:
   - Your step-by-step reasoning
   - Final answer clearly marked
   ```

**Why this works:**
- Examples demonstrate the expected reasoning pattern
- Chain of thought ensures the AI "shows its work"
- Quality improves because reasoning forces accuracy
- Easier to verify and audit the AI's logic

---

## 9. QUICK SUMMARY

- **Zero-shot, one-shot, and few-shot** provide increasing levels of guidance through examples—choose based on task complexity and format requirements.

- **Persona-based prompting** transforms response quality by setting expertise, tone, and perspective—essential for professional business contexts.

- **Chain of thought and step-by-step reasoning** dramatically improve accuracy for complex tasks by forcing the AI to "show its work."

- **Prompt chaining** breaks complex, multi-stage projects into manageable steps, enabling better quality and more control.

- **Combine techniques strategically** for maximum impact—the best prompts often use multiple techniques together.

---

## 10. KEY TAKEAWAYS

### When to Use Each Technique

| Technique | Best For | When to Use |
|-----------|----------|-------------|
| Zero-shot | Simple Q&A, basic tasks | First attempt, simple asks |
| One-shot | Format demonstration | Specific output patterns |
| Few-shot | Quality consistency, complex formats | 2-4 examples needed |
| Instruction-based | Detailed guidance | Clear process needed |
| Persona-based | Expert perspective | Tone/expertise matters |
| Comparative | Decision-making | Multiple options to evaluate |
| Delimiters | Structure clarity | Complex, multi-section prompts |
| Context injection | Relevance accuracy | Background information crucial |
| Multi-step | Sequential tasks | Multiple steps in one prompt |
| Chain of thought | Complex reasoning | Logic and verification needed |
| Prompt chaining | Multi-stage projects | Steps need validation |

### When NOT to Use Each Technique

- **Don't overcomplicate:** Simple tasks don't need few-shot or chain of thought
- **Don't use personas** when neutral, factual answers are needed
- **Don't chain prompts** when one prompt would suffice
- **Don't over-constrain** creativity with too many constraints
- **Don't use examples** if the AI clearly understands the task

### Benefits
- **Precision:** Right technique = right results faster
- **Versatility:** Handle any task type effectively
- **Quality:** Better outputs with fewer iterations
- **Efficiency:** Less time spent refining
- **Scalability:** Techniques work across teams
- **Confidence:** Predictable, consistent results

### Limitations
- **Learning curve:** Mastering all techniques takes time
- **Over-engineering:** Sometimes simple works best
- **Model variance:** Techniques work differently across models
- **Token costs:** Examples and context increase token usage
- **Time investment:** Creating complex prompts takes longer upfront

### Best Practices

1. **Start simple, add complexity gradually**
2. **Test techniques before committing to one**
3. **Combine techniques strategically**
4. **Document what works for each use case**
5. **Keep a prompt library of successful examples**
6. **Train your team on technique selection**
7. **Monitor output quality and iterate**
8. **Consider token/API costs when adding examples**
9. **Be mindful of context window limits**
10. **Validate complex outputs with subject matter experts**

---

## 11. KNOWLEDGE CHECK

### Multiple Choice Questions

**Q1. Which prompting technique involves providing no examples to the AI?**
- A) Few-shot prompting
- B) One-shot prompting
- C) Zero-shot prompting
- D) Instruction-based prompting

**Correct Answer: C**
**Explanation:** Zero-shot prompting means giving the AI no examples—just the task itself. The AI relies entirely on its training data to understand and perform the task.

---

**Q2. What is the primary advantage of chain of thought prompting?**
- A) It makes prompts shorter
- B) It forces the AI to show its reasoning, improving accuracy
- C) It requires fewer examples
- D) It works with any AI model

**Correct Answer: B**
**Explanation:** Chain of thought prompting instructs the AI to show its step-by-step reasoning process. This "thinking aloud" approach dramatically improves accuracy for complex tasks because the AI must logically work through the problem rather than jumping to a conclusion.

---

**Q3. When would you choose prompt chaining over a single multi-step prompt?**
- A) When you want to save time on prompt creation
- B) When the task is simple and straightforward
- C) When you need to validate or refine outputs between steps
- D) When you have limited token budget

**Correct Answer: C**
**Explanation:** Prompt chaining is preferred when intermediate results need to be reviewed, validated, or refined before proceeding to the next step. It provides more control and quality assurance than a single prompt.

---

**Q4. What does persona-based prompting primarily control?**
- A) The length of the output
- B) The tone, expertise level, and perspective of the response
- C) The speed of the AI's response
- D) The cost of using the AI

**Correct Answer: B**
**Explanation:** Persona-based prompting defines the AI's "character"—its expertise, experience, tone, and perspective. This fundamentally shapes the quality, depth, and style of the response.

---

**Q5. How many examples are typically recommended for few-shot prompting?**
- A) 10-15 examples
- B) 1 example
- C) 2-5 examples
- D) 20+ examples

**Correct Answer: C**
**Explanation:** Few-shot prompting typically works best with 2-5 high-quality examples. Too few examples (1) is one-shot prompting, while too many examples (10+) can confuse the AI and dilute the pattern.

---



---

*This training material is designed for professional development. Remember: Great prompt engineers build a toolkit of techniques and choose the right tool for each job.*
