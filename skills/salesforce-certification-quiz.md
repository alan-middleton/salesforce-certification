# Salesforce Certification Quiz

## Description

Activates whenever a user asks to be tested, quizzed, given practice questions, or assessed for a Salesforce certification exam.

Use this skill for individual practice questions, multi-question quizzes, mock exams, knowledge checks, revision drills, diagnostic assessments, resumed quizzes, and user-supplied certification questions that require marking and explanation.

Generates original Salesforce-style questions aligned with the selected Salesforce Certified Exam Guide and its applicable release timeframe. Questions are always written at realistic certification-exam standard. The skill marks every response, explains every option, tracks performance by syllabus domain, and provides targeted final feedback.

Common activation phrases include “quiz me,” “test me,” “ask me questions,” “practice questions,” “mock exam,” “knowledge check,” “continue the quiz,” and “mark this Salesforce question.”

## Instructions

When this skill is activated:

1. Retain any exam, timeframe, topics, question count, delivery format, or question-type preferences already supplied by the user. Do not ask for information already provided.

2. Identify the Salesforce certification exam if it is not already known.

3. Establish the relevant Salesforce Certified Exam Guide, including:
   - Syllabus domains and objectives
   - Domain weightings
   - Expected terminology
   - Applicable release year or timeframe

   Never assume that every Salesforce certification exam uses the same year.

4. Use the official Salesforce Trailhead MCP server when available to verify exam objectives, terminology, weightings, recommended practices, and release-sensitive behaviour. If the timeframe is genuinely unclear and could materially change an answer, clarify it before generating release-sensitive questions.

5. Establish only the missing quiz preferences needed to proceed, such as:
   - Number of questions
   - One-at-a-time or batch delivery
   - Whole syllabus or selected domains
   - Whether the user wants a particular question-type mix

   Do not ask the user to choose a difficulty or knowledge level. Do not offer basic, intermediate, advanced, easy, medium, or hard modes. Every question must meet the mandatory exam-level standard defined below.

6. Before presenting the first question, prepare and validate an internal quiz plan containing:
   - Question number
   - Exam-guide domain and objective
   - Question type
   - Capability or distinction being tested
   - Governing Salesforce principle
   - Correct answer or complete answer set
   - Correct-answer position or combination
   - Why each distractor is plausible but wrong
   - Applicable exam-guide timeframe

   Do not reveal the plan, answer key, answer distribution, or future answers.

7. Ask one original question at a time unless the user explicitly requests a batch.

8. Wait for the learner’s answer before revealing the solution.

9. After every answer:
   - Mark it explicitly **Correct** or **Incorrect**.
   - State the complete correct answer or answer set.
   - Explain the governing Salesforce principle.
   - Review every presented option individually.
   - Explain why each option is correct, incorrect, technically possible but not best, intended for another use case, invalid because of a stated constraint, or applicable only to another release.
   - Add a concise exam-taking takeaway when useful.
   - Update the running score and progress.
   - Continue to the next question unless the learner pauses or asks a follow-up question.

10. If the learner asks a follow-up question:
    - Pause progression.
    - Answer it fully.
    - Retain the current score, question number, and quiz plan.
    - Resume from the same position.
    - Do not count the follow-up as a quiz response.

11. If the learner challenges an answer:
    - Pause the quiz.
    - Re-evaluate the question instead of defending it automatically.
    - Check the applicable exam-guide timeframe and official Salesforce material.
    - Correct the answer, wording, or score when necessary.
    - Do not penalise the learner for an ambiguous, defective, out-of-syllabus, or release-inaccurate question.
    - Resume from the same point after resolving the issue.

12. After the requested number of valid questions is complete, provide:
    - Total score and percentage
    - Performance by exam-guide domain
    - Demonstrated strengths
    - Specific knowledge gaps
    - Repeated misconceptions
    - Important distinctions to revise
    - Targeted Trailhead and exam-guide study recommendations

## Guidelines

### Mandatory exam-level standard

Every generated question must resemble the reasoning standard expected in the applicable Salesforce certification exam. “Exam level” is mandatory and is not a selectable difficulty.

An exam-level question should normally require the learner to do one or more of the following:

- Interpret a realistic business or technical requirement.
- Identify multiple material constraints in the stem.
- Distinguish between several genuine Salesforce capabilities.
- Select the best supported or recommended solution rather than one that is merely possible.
- Apply a platform rule to a scenario rather than recite a definition.
- Recognise a prerequisite, limitation, relationship direction, security boundary, order-of-execution implication, or release-specific behaviour.
- Determine why otherwise valid features fail one or more stated requirements.

Do not reduce questions to elementary product recognition when a scenario or capability comparison can test the same objective more authentically.

Avoid questions such as:

- “What is a lookup relationship?”
- “What does Flow Builder do?”
- “Which object stores companies?”
- Questions where three options are obviously invented or unrelated.
- Questions answerable from a single obvious keyword without understanding the rest of the stem.

Direct knowledge questions are acceptable only when the exam objective genuinely tests exact facts such as:

- Supported capabilities
- Configuration prerequisites
- Tool limits
- Named component types
- Relationship rules
- Security behaviour
- Deployment behaviour
- Formula behaviour

Even then, use plausible Salesforce alternatives and require precise discrimination.

For quizzes of 10 or more questions:

- Make most questions application-based or scenario-based.
- Include shorter capability, prerequisite, limitation, and terminology questions to reflect the real exam’s variety.
- Do not allow the quiz to become a sequence of introductory definitions.

Keep questions at exam level even when the learner performs poorly. Adapt explanations, feedback, and study recommendations—not the standard of subsequent questions.

### Scenario construction

A strong scenario should usually contain:

- A recognisable Salesforce role, team, or business context
- A clear desired outcome
- Two or more constraints that affect the solution
- Enough information to identify the applicable feature
- No irrelevant narrative that exists only to increase reading length

Useful constraints include:

- Declarative-only requirements
- Data volume or bulk-processing needs
- Parent/child direction
- Record ownership and sharing model
- Field visibility versus editability
- Immediate versus scheduled execution
- Required versus optional relationships
- Record creation, deletion, reparenting, or cascade behaviour
- Mobile, console, or Lightning page context
- Deployment controls
- External versus Salesforce-stored data
- Exam-era feature availability

Do not omit a permission, edition, licence, setting, object relationship, or execution context when it is necessary to determine the answer.

### Distractor quality

Prefer distractors that are real Salesforce features from the same conceptual area as the correct answer.

Each distractor must be plausible to a partially prepared learner and wrong for a precise reason. Good distractors include:

- A valid feature that solves a different requirement
- A technically possible solution that is less appropriate than a dedicated feature
- A solution that satisfies some but not all constraints
- A feature operating at the wrong security layer
- A relationship with the wrong parent/child direction
- An automation tool that runs at the wrong point in the transaction
- A current-platform capability that is not applicable to the exam timeframe
- A correct configuration paired with the wrong tool or prerequisite

Avoid:

- Joke answers
- Obviously fictitious terminology, except when official taxonomy is the point being tested
- Options from unrelated Salesforce products
- One detailed correct answer surrounded by three very short or vague options
- Grammatical clues linking only the correct option to the stem
- Repeating an exact phrase from the stem only in the correct answer
- Absolute wording used merely to make an option easy to eliminate

All four options should be parallel in style, specificity, and approximate length where practical.

### Question formats

Use a balanced mix of the formats represented in the applicable syllabus and Salesforce question style.

**Single answer**

- Use exactly four options labelled A, B, C, and D.
- Ask for the best answer when more than one approach could technically contribute.

**Multiple select**

- Use exactly four options labelled A, B, C, and D unless a different count is explicitly requested.
- Clearly state **Choose 2** or **Choose 3**.
- Ensure exactly the stated number is defensible.
- Design options so each must be evaluated independently.

**True/False**

- Use A. True and B. False.
- Use sparingly.
- Test a meaningful platform rule, not a trivial definition.
- A compound statement is true only when every material part is true.

Include an appropriate mixture of:

- Technical scenarios
- Business scenarios
- Feature-capability distinctions
- Configuration prerequisites
- Platform limitations
- Security and sharing
- Data modelling and relationships
- User interface and mobile
- Automation and order of execution
- Reporting and dashboards
- Data management
- Application lifecycle and deployment
- Release-sensitive behaviour where relevant

### Exam-era accuracy

- Base every question on the selected exam’s syllabus.
- Use terminology and behaviour expected by that exam guide’s timeframe.
- Never assume all exams are aligned to 2023 or any other year.
- Use exam-era terminology in the question.
- If current terminology or functionality differs materially, give the exam answer first and explain the current distinction only after the learner answers.
- Clearly label current-platform information.
- Do not introduce Agentforce or newer functionality unless it appears in the applicable exam guide or the learner explicitly requests a current comparison.
- If current Trailhead content conflicts with the applicable exam-guide timeframe, preserve the exam-era expected answer and explain the difference separately.

### Question validation

Before presenting each question, verify all of the following:

1. The objective is within the selected exam syllabus.
2. The expected answer is correct for the applicable timeframe.
3. The question tests application, discrimination, or precise capability knowledge at exam level.
4. The scenario contains every material fact needed to answer.
5. Exactly the stated number of options is correct.
6. Every distractor is plausible and wrong for a specific documented reason.
7. No unstated edition, licence, permission, setting, interface, data model, or release changes the answer.
8. No uncommon but valid capability unintentionally creates another correct answer.
9. The correct answer is not exposed by wording, length, grammar, or option structure.
10. Qualifiers such as **all**, **always**, **never**, **only**, **must**, **may**, and **automatically** are technically intentional.
11. The question distinguishes a technically possible solution from the best exam answer when relevant.
12. The explanation can clearly justify all options without relying on “because Salesforce says so.”

If any check fails, rewrite or replace the question before showing it.

Take particular care with:

- Lookup, master-detail, external lookup, and indirect lookup direction
- Cross-object formulas versus child aggregation
- Object-level, record-level, and field-level access
- Sharing rules versus restriction rules
- Field-level security versus page layouts
- Security versus Dynamic Forms and component visibility
- Record types, business processes, page layouts, and Lightning pages
- Formula, validation, roll-up summary, and automation use cases
- Before-save versus after-save automation
- Scheduled paths and entry-condition behaviour
- Workflow Rules, Process Builder, Flow, and Approval Process for the applicable timeframe
- Data Import Wizard versus Data Loader capabilities and interfaces
- Fixed-running-user versus dynamic dashboards
- Change sets, dependencies, validation, and flow activation
- Standard named capabilities versus outcomes that could be custom-built

### Answer distribution

For single-answer questions:

- Pre-plan the answer key before asking Question 1.
- Distribute correct positions as evenly as mathematically possible across A, B, C, and D.
- A 20-question single-answer quiz must contain exactly 5 answers in each position.
- For other totals, keep position counts within 1 where mathematically possible.
- Avoid obvious answer sequences.
- Do not disclose the distribution.

For multi-select questions:

- Vary correct positions and combinations.
- Do not repeatedly use the same combination.
- Balance individual letter frequency across the quiz where practical.

Verify the actual distribution before final feedback. Never claim it was balanced unless checked.

### Marking rules

For single-answer questions:

- If the learner gives multiple answers without identifying one final choice, mark the response Incorrect.

For multi-select questions:

- Require the complete correct set.
- A partially correct response is Incorrect.
- Identify correct selections, incorrect selections, and omitted required answers.
- If the learner selects more answers than requested, mark the response Incorrect.

If a question is found to be ambiguous, defective, outside the syllabus, or release-inaccurate:

- Exclude it from scoring.
- Replace it if necessary to preserve the requested number of valid questions.
- Explain the correction clearly.

### Skill continuity

- This skill owns setup, planning, delivery, marking, explanations, score tracking, domain tracking, pauses, challenges, resumptions, and final feedback.
- Preserve quiz state across brief digressions.
- If the learner says “continue” or “next,” proceed from the next unanswered question rather than restarting.
- Do not silently shorten the requested quiz.
- Do not provide final feedback before the requested number of valid questions is complete.

### User-supplied questions

When the learner supplies a practice question:

- Answer it using the selected exam and timeframe.
- State the correct answer or complete answer set.
- Review every option.
- Explain the governing Salesforce principle.
- Identify any ambiguity, exception, or release-sensitive distinction.
- Observe useful construction patterns and incorporate them into later generated questions in the same session.

Useful patterns include:

- Four genuine Salesforce capabilities where only some fit the requirement
- Qualified statements contrasted with incorrect absolutes
- Exact prerequisites
- Relationship direction
- Security-layer distinctions
- Official taxonomy
- Dedicated capability versus generic automation
- Correct configuration paired with the wrong tool
- Best solution versus merely possible solution

### Performance tracking

Track:

- Overall score
- Score by exam-guide domain
- Strong domains
- Weak domains
- Repeated misconceptions
- Questions excluded or corrected because of ambiguity

Do not claim that a practice score guarantees certification success.

## Examples

**Example 1: Too basic versus exam level**
- Weak question: “What is a roll-up summary field?”
- Expected improvement: Present a master-detail scenario requiring a filtered MAX, SUM, MIN, or COUNT calculation and include formula, Flow, and lookup-based alternatives that fail specific requirements.

**Example 2: Genuine-feature distractors**
- User request: “Ask me a Lightning record-page question.”
- Expected behavior: Use four genuine components such as Tabs, Accordion, Path, and Carousel. Require the learner to select the components that reduce page clutter while preserving access, rather than identify fabricated names.

**Example 3: Best solution rather than possible solution**
- Scenario: A parent must show a real-time aggregate of qualifying child records in a master-detail relationship.
- Expected behavior: Make a native filtered roll-up summary the best answer. A Flow may be possible but should be rejected as unnecessary complexity, while a cross-object formula cannot aggregate children.

**Example 4: Security-layer discrimination**
- Scenario: A user has Read/Write record access but cannot edit one field.
- Expected behavior: Test field-level security against sharing, role hierarchy, page layout, and restriction-rule alternatives. Explain why record access does not grant field edit access.

**Example 5: Multi-constraint relationship question**
- Scenario: A child may temporarily exist without a parent, can be reparented, and must survive parent deletion; the parent also needs a count.
- Expected behavior: Require an optional lookup plus declarative automation for the count. Master-detail distractors should fail the lifecycle constraints; a native lookup roll-up should fail because it is unsupported.

**Example 6: Release-sensitive question**
- User request: “With Workflow Rules and Process Builder retired, what creates an approval process?”
- Expected behavior: Determine the selected exam’s timeframe. Give the answer expected by that exam guide and discuss newer functionality only in the review if materially relevant.

**Example 7: Precise short-form question**
- Scenario: Ask which formula function returns different results for several discrete field values.
- Expected behavior: Use CASE, CONTAINS, BEGINS, and OR as genuine formula-function options. Explain that CASE performs multi-branch value mapping while the others perform Boolean tests.

**Example 8: Ambiguity challenge**
- User request: “I thought Data Loader could connect directly to a database. Is CSV required?”
- Expected behavior: Pause, investigate graphical versus command-line capabilities, acknowledge imprecise wording, exclude or correct the question if necessary, and resume without unfairly penalising the learner.

**Example 9: Multi-select marking**
- Correct set: A and D.
- Learner response: A and C.
- Expected behavior: Mark Incorrect, identify A as correctly selected, explain why C is wrong, identify D as omitted, review every option, update the score, and continue.

**Example 10: Poor performance does not lower question standard**
- Learner outcome: Several incorrect answers in one domain.
- Expected behavior: Continue asking exam-level questions. Provide clearer post-answer teaching and recommend targeted revision, but do not switch to elementary definitions unless the learner ends the quiz and explicitly asks for foundational teaching.

## Reference question patterns

The following are original illustrative questions, not live certification questions. They demonstrate the expected construction standard. Adapt their structure and reasoning depth to the selected certification, syllabus objective, and exam-guide timeframe. Do not repeatedly reuse them verbatim.

### Reference Question 1: Native capability versus unnecessary automation

A company tracks `Project__c` records as masters of `Milestone__c` records in a master-detail relationship. Management needs each project to display the most recent completion date among milestones whose Status is Completed. The value must update when qualifying milestones are created, edited, deleted, or undeleted.

What should the app builder configure?

A. A cross-object formula on `Project__c` that references `Milestone__c.Completion_Date__c`  
B. A filtered roll-up summary field using MAX on `Completion_Date__c`  
C. A before-save flow on `Milestone__c` that updates the project  
D. A scheduled flow that recalculates every project each night

**Correct answer: B**

**Why this is exam level:** The learner must recognise the relationship type, the supported aggregate, the filter requirement, and automatic recalculation behaviour. Flow is technically possible but inferior to the dedicated native capability. A cross-object formula cannot aggregate an arbitrary child collection, and a nightly process fails the immediate-update requirement.

### Reference Question 2: Relationship direction

Invoices remain in an external billing system and are exposed in Salesforce as `Invoice__x`. Each invoice contains a customer key. Salesforce Account is the required parent, and Account has a matching field configured as Unique and External ID. Invoice data must not be copied into Salesforce.

Which relationship should be configured?

A. Master-detail relationship  
B. Standard lookup relationship  
C. External lookup relationship  
D. Indirect lookup relationship

**Correct answer: D**

**Why this is exam level:** All choices are genuine relationship concepts. The learner must determine where the child and parent reside. An external-object child relating to a Salesforce parent through the parent’s unique External ID requires an indirect lookup; an external lookup instead has an external object as parent.

### Reference Question 3: Security layer versus presentation layer

Opportunity organization-wide defaults are Private. An opportunity owner grants an internal specialist Read/Write access to one opportunity. The specialist can edit other fields but cannot edit `Discount_Percentage__c`.

What should the administrator examine first?

A. The specialist’s field-level security for `Discount_Percentage__c`  
B. Whether the specialist is below the owner in the role hierarchy  
C. Whether a restriction rule grants field edit access  
D. Whether the opportunity page layout is assigned through the correct app

**Correct answer: A**

**Why this is exam level:** The stem proves that record-level edit access already exists and isolates the issue to one field. The learner must distinguish field-level security from sharing, role hierarchy, restriction rules, and page presentation.

### Reference Question 4: Several valid components, only two valid uses

Users report that a Lightning record page is crowded. Several components are needed only occasionally, but users must still be able to access them without navigating away.

Which two standard components should the app builder use? **Choose 2.**

A. Accordion  
B. Path  
C. Tabs  
D. Carousel

**Correct answers: A and C**

**Why this is exam level:** Every option is a real component. Accordion and Tabs organise other components into collapsible or selectable sections. Path displays process progress and guidance; Carousel displays rotating visual content. The learner cannot answer by eliminating fabricated names.

### Reference Question 5: Multiple lifecycle constraints

A company tracks `Building__c` and related `Inspection__c` records. An inspection must be allowed to exist temporarily without a building, users must be able to move it to another building, and deleting a building must not delete its inspections. Building must also display the number of related inspections using declarative functionality.

Which design best meets the requirements?

A. Master-detail with a native roll-up summary  
B. Master-detail with reparenting enabled and a native roll-up summary  
C. Optional lookup with a record-triggered flow maintaining the count  
D. Optional lookup with a native roll-up summary

**Correct answer: C**

**Why this is exam level:** The learner must evaluate every lifecycle requirement. Master-detail fails optional-parent and cascade-delete requirements. Lookup satisfies lifecycle independence, but a native roll-up summary is unavailable for an ordinary lookup, so declarative automation must maintain the count.

### Reference Question 6: Shared dashboard versus viewer-specific access

Opportunity organization-wide defaults are Private. Regional managers already receive appropriate access through the role hierarchy. They must use one dashboard, with each manager seeing metrics only for records that the individual manager can access. The company does not want regional dashboard copies or broader record access.

What should the administrator configure?

A. A dashboard running as the system administrator  
B. A dynamic dashboard running as the logged-in user  
C. A dashboard filter that requires managers to select their region  
D. A dashboard running as one regional manager

**Correct answer: B**

**Why this is exam level:** The learner must distinguish dashboard filters from record security and fixed-running-user dashboards from viewer-specific dynamic dashboards. Several options can display regional information, but only the dynamic dashboard automatically respects each viewer’s existing access.

### Reference Question 7: Prerequisite versus resulting action

An administrator wants declarative automation to send a custom in-app and mobile notification when a high-priority Case is escalated.

What must be configured before the automation action can be completed?

A. An email letterhead  
B. A custom notification type  
C. A notification workflow action  
D. A Lightning message channel

**Correct answer: B**

**Why this is exam level:** This is a concise prerequisite question rather than a long scenario. The distractors are genuine platform concepts, but only a custom notification type is the required setup dependency for a custom-notification action.

### Reference Question 8: Qualified statements and exact multi-select count

For which two organization-wide defaults can sharing rules extend record access? **Choose 2.**

A. Private  
B. Public Read Only  
C. Public Read/Write  
D. Controlled by Parent

**Correct answers: A and B**

**Why this is exam level:** The learner must apply the principle that sharing rules only open access. Private leaves read and edit access available to grant; Public Read Only leaves edit access available to grant. Public Read/Write has no additional ordinary record access to add, while Controlled by Parent derives access from the parent.

### Reference Question 9: Same product area, different responsibilities

A company has Direct Sale and Partner Sale Opportunity record types. Each type needs a different set of Stage values and a different field arrangement. Partner Sale must require `Partner__c` in the editing interface. Both types should continue to use one Lightning record page.

Which configuration is best?

A. Separate sales processes and page layouts assigned through the record types  
B. Separate Lightning record pages activated by record type  
C. Component visibility rules on one Lightning page  
D. Validation rules that reject inappropriate Stage values

**Correct answer: A**

**Why this is exam level:** All options can affect some aspect of the user experience, but only record types with sales processes and page-layout assignments satisfy Stage availability, field arrangement, and layout-level requiredness together. The learner must understand where each configuration responsibility belongs.

### Reference Question 10: Precise short-form capability question

Which formula function is most appropriate for returning a different result for each of several discrete values in one field?

A. OR  
B. BEGINS  
C. CASE  
D. CONTAINS

**Correct answer: C**

**Why this is exam level:** Short questions are acceptable when they test an exact syllabus capability. Every option is a real formula function. CASE maps multiple values to different results; the other functions evaluate Boolean conditions. This is precise discrimination rather than elementary terminology recognition.

### How to generalise these examples

When generating new questions, reproduce the reasoning patterns rather than the names or answer positions:

- Dedicated native feature versus generic automation
- Correct feature at the wrong security layer
- Parent/child direction determining relationship type
- Several real components with different purposes
- A solution that satisfies only some constraints
- Fixed versus viewer-specific context
- Required prerequisite versus eventual action
- Qualified rule versus an overbroad statement
- Configuration responsibilities split across related features
- Exact capability discrimination among genuine functions or tools

Vary objects, industries, constraints, correct-answer positions, question types, and syllabus domains. Do not transform these examples into a repeated question bank.

## Notes

- The applicable release year belongs to the individual exam guide, not to Salesforce certifications generally.
- Exam-level difficulty should come from applying syllabus knowledge, integrating constraints, and distinguishing genuine Salesforce capabilities—not from obscure trivia or deceptive wording.
- Strong questions often contain four real features. The incorrect answers should be valid elsewhere but fail this scenario for an identifiable reason.
- Short capability questions are useful when they test exact exam-relevant behaviour; they must not dominate the quiz.
- Deterministic workflow matters: plan first, validate every question, administer the requested number, mark every answer, and provide final feedback only after completion.
- Treat learner corrections and supplied examples as evidence for improving later question construction in the same session.