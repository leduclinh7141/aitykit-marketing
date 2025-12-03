# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **curriculum-designer** | Curriculum & lesson planning | sonnet |
| **tutor-assistant** | Personalized tutoring | sonnet |
| **assessment-creator** | Tests, quizzes, rubrics | sonnet |
| **learning-analyst** | Learning analytics & insights | sonnet |
| **content-creator** | Educational content creation | sonnet |
| **student-support** | Student inquiries & guidance | haiku |

---

## 2.2 Curriculum Designer

**File:** `.claude/agents/curriculum-designer.md`

```yaml
---
name: curriculum-designer
description: Curriculum and instructional design specialist. Use for creating lesson plans, learning objectives, course outlines, and curriculum mapping. Handles standards alignment and backward design.
model: sonnet
---
```

### Core Capabilities

- **Lesson Planning**: Daily/weekly lesson plans
- **Curriculum Mapping**: Scope and sequence
- **Standards Alignment**: Common Core, state standards
- **Learning Objectives**: Bloom's taxonomy aligned
- **Unit Design**: Backward design methodology
- **Differentiation**: Multiple learning levels

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Lesson Plan | Markdown | Daily teaching |
| Unit Plan | Markdown | Multi-week units |
| Curriculum Map | Table | Annual planning |
| Standards Matrix | Table | Compliance |

### Skills Used

- `instructional-design` - Pedagogy, design
- `standards-alignment` - Educational standards
- `differentiation` - Learning levels

---

## 2.3 Tutor Assistant

**File:** `.claude/agents/tutor-assistant.md`

```yaml
---
name: tutor-assistant
description: Personalized tutoring specialist. Use for explaining concepts, guiding problem-solving, answering questions, and providing adaptive instruction. Handles Socratic dialogue and scaffolded learning.
model: sonnet
---
```

### Core Capabilities

- **Concept Explanation**: Clear, multi-modal explanations
- **Socratic Dialogue**: Guided questioning
- **Problem Solving**: Step-by-step guidance
- **Misconception Correction**: Identify and address
- **Adaptive Instruction**: Adjust to learner level
- **Practice Generation**: Custom practice problems

### Tutoring Approaches

| Approach | Description | Use Case |
|----------|-------------|----------|
| Socratic | Question-based discovery | Conceptual understanding |
| Scaffolded | Gradual support reduction | Skill building |
| Worked Examples | Step-by-step demos | New procedures |
| Spaced Retrieval | Timed review | Retention |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Explanation | Markdown | Learning |
| Practice Set | Markdown | Reinforcement |
| Study Guide | Markdown | Review |
| Progress Report | Markdown | Tracking |

### Skills Used

- `tutoring` - Pedagogical techniques
- `subject-matter` - Content expertise
- `adaptive-learning` - Personalization

---

## 2.4 Assessment Creator

**File:** `.claude/agents/assessment-creator.md`

```yaml
---
name: assessment-creator
description: Assessment and evaluation specialist. Use for creating tests, quizzes, rubrics, and grading criteria. Handles formative and summative assessments with automated grading support.
model: sonnet
---
```

### Core Capabilities

- **Quiz Generation**: Multiple choice, short answer
- **Test Creation**: Comprehensive assessments
- **Rubric Design**: Criteria-based evaluation
- **Auto-Grading**: Objective question grading
- **Feedback Generation**: Detailed feedback
- **Item Analysis**: Question quality metrics

### Assessment Types

| Type | Purpose | Timing |
|------|---------|--------|
| Diagnostic | Pre-assess knowledge | Start of unit |
| Formative | Check understanding | During learning |
| Summative | Evaluate mastery | End of unit |
| Performance | Apply skills | Project-based |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Quiz | Markdown/JSON | Quick check |
| Test | Markdown/PDF | Formal assessment |
| Rubric | Table | Performance eval |
| Answer Key | Markdown | Grading |

### Skills Used

- `assessment-design` - Test construction
- `rubric-development` - Evaluation criteria
- `item-analysis` - Question quality

---

## 2.5 Learning Analyst

**File:** `.claude/agents/learning-analyst.md`

```yaml
---
name: learning-analyst
description: Learning analytics and insights specialist. Use for analyzing student performance, identifying learning gaps, predicting outcomes, and generating reports. Handles data-driven instructional decisions.
model: sonnet
---
```

### Core Capabilities

- **Performance Analytics**: Grade analysis, trends
- **Gap Identification**: Learning gaps, at-risk students
- **Outcome Prediction**: Success forecasting
- **Engagement Metrics**: Participation, completion
- **Report Generation**: Progress reports, dashboards
- **Intervention Recommendations**: Targeted support

### Key Metrics

| Category | Metrics |
|----------|---------|
| Performance | Grades, scores, mastery levels |
| Engagement | Time on task, completion, participation |
| Progress | Growth, improvement, pace |
| Prediction | At-risk, success probability |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Progress Report | Markdown | Parent/student |
| Class Dashboard | Table | Teacher |
| Intervention Plan | Markdown | Support |
| Outcome Forecast | Table | Planning |

### Skills Used

- `learning-analytics` - Educational data analysis
- `data-visualization` - Dashboards, charts
- `predictive-modeling` - Outcome forecasting

---

## 2.6 Content Creator

**File:** `.claude/agents/content-creator.md`

```yaml
---
name: content-creator
description: Educational content creation specialist. Use for creating lecture materials, presentations, videos scripts, interactive content, and supplementary materials. Handles multi-modal content design.
model: sonnet
---
```

### Core Capabilities

- **Lecture Materials**: Slides, handouts, notes
- **Video Scripts**: Lesson videos, tutorials
- **Interactive Content**: Activities, simulations
- **Reading Materials**: Articles, summaries
- **Practice Materials**: Worksheets, exercises
- **Accessibility**: ADA/508 compliant content

### Content Types

| Type | Format | Use Case |
|------|--------|----------|
| Slides | Markdown/PPT | Lecture |
| Video Script | Markdown | Recording |
| Worksheet | Markdown/PDF | Practice |
| Reading | Markdown | Study |
| Activity | Markdown | Engagement |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Slide Deck | Markdown | Presentation |
| Video Script | Markdown | Production |
| Worksheet | Markdown | Student work |
| Study Guide | Markdown | Review |

### Skills Used

- `content-development` - Material creation
- `multimedia` - Multi-modal design
- `accessibility` - Universal design

---

## 2.7 Student Support

**File:** `.claude/agents/student-support.md`

```yaml
---
name: student-support
description: Student support and guidance specialist. Use for answering student questions, providing study tips, explaining assignments, and offering encouragement. Handles first-line student assistance.
model: haiku
---
```

### Core Capabilities

- **Question Answering**: Course-related questions
- **Assignment Clarification**: Instructions, expectations
- **Study Tips**: Learning strategies
- **Resource Navigation**: Finding materials
- **Encouragement**: Motivation, support
- **Escalation**: Route to instructor

### Common Support Areas

| Area | Examples |
|------|----------|
| Logistics | Due dates, submission |
| Content | Concept clarification |
| Technical | Platform issues |
| Academic | Study strategies |
| Emotional | Encouragement |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Answer | Markdown | Quick help |
| Study Guide | Markdown | Preparation |
| Resource List | Markdown | Materials |
| Escalation | Ticket | Instructor |

### Skills Used

- `student-support` - Assistance
- `study-skills` - Learning strategies
- `communication` - Clear responses

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| Course design | curriculum-designer | content-creator |
| Content creation | content-creator | curriculum-designer |
| Test creation | assessment-creator | curriculum-designer |
| Student tutoring | tutor-assistant | student-support |
| Grade analysis | learning-analyst | assessment-creator |
| Student question | student-support | tutor-assistant |
| Intervention planning | learning-analyst | tutor-assistant |
| Progress reporting | learning-analyst | assessment-creator |
