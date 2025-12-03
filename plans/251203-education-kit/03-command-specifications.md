# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── curriculum/
│   ├── lesson.md          # /curriculum:lesson
│   ├── unit.md            # /curriculum:unit
│   ├── map.md             # /curriculum:map
│   └── objectives.md      # /curriculum:objectives
├── tutor/
│   ├── explain.md         # /tutor:explain
│   ├── practice.md        # /tutor:practice
│   ├── review.md          # /tutor:review
│   └── help.md            # /tutor:help
├── assess/
│   ├── quiz.md            # /assess:quiz
│   ├── test.md            # /assess:test
│   ├── rubric.md          # /assess:rubric
│   └── grade.md           # /assess:grade
├── analytics/
│   ├── progress.md        # /analytics:progress
│   ├── gaps.md            # /analytics:gaps
│   ├── predict.md         # /analytics:predict
│   └── report.md          # /analytics:report
├── content/
│   ├── slides.md          # /content:slides
│   ├── video.md           # /content:video
│   ├── worksheet.md       # /content:worksheet
│   └── reading.md         # /content:reading
└── support/
    ├── question.md        # /support:question
    ├── assignment.md      # /support:assignment
    ├── study.md           # /support:study
    └── resources.md       # /support:resources
```

---

## 3.2 Curriculum Commands

### /curriculum:lesson
```yaml
---
description: Create lesson plan for topic
argument-hint: [topic] [grade-level] [duration]
---
```

**Workflow:**
1. Identify learning objectives
2. Align to standards
3. Design activities
4. Plan assessment
5. Include differentiation
6. Output lesson plan

**Agent:** `curriculum-designer`

---

### /curriculum:unit
```yaml
---
description: Design multi-lesson unit plan
argument-hint: [topic] [grade-level] [duration]
---
```

**Workflow:**
1. Define unit goals
2. Map lessons sequence
3. Plan assessments
4. Include resources
5. Output unit plan

**Agent:** `curriculum-designer`

---

### /curriculum:map
```yaml
---
description: Create curriculum map for course/year
argument-hint: [subject] [grade-level] [scope]
---
```

**Workflow:**
1. Define scope and sequence
2. Align to standards
3. Map units to timeline
4. Include assessments
5. Output curriculum map

**Agent:** `curriculum-designer`

---

### /curriculum:objectives
```yaml
---
description: Generate learning objectives
argument-hint: [topic] [level]
---
```

**Workflow:**
1. Identify key concepts
2. Apply Bloom's taxonomy
3. Write measurable objectives
4. Align to standards
5. Output objectives list

**Agent:** `curriculum-designer`

---

## 3.3 Tutor Commands

### /tutor:explain
```yaml
---
description: Explain concept to student
argument-hint: [concept] [level] [context]
---
```

**Workflow:**
1. Assess student level
2. Break down concept
3. Provide examples
4. Check understanding
5. Output explanation

**Agent:** `tutor-assistant`

---

### /tutor:practice
```yaml
---
description: Generate practice problems
argument-hint: [topic] [difficulty] [quantity]
---
```

**Workflow:**
1. Identify skill area
2. Generate problems
3. Vary difficulty
4. Include solutions
5. Output practice set

**Agent:** `tutor-assistant`

---

### /tutor:review
```yaml
---
description: Create study review for topic
argument-hint: [topic] [scope]
---
```

**Workflow:**
1. Identify key concepts
2. Summarize content
3. Add practice questions
4. Include study tips
5. Output review guide

**Agent:** `tutor-assistant`

---

### /tutor:help
```yaml
---
description: Help student with specific problem
argument-hint: [problem] [subject]
---
```

**Workflow:**
1. Analyze problem
2. Identify approach
3. Guide step-by-step
4. Check understanding
5. Output guided solution

**Agent:** `tutor-assistant`

---

## 3.4 Assessment Commands

### /assess:quiz
```yaml
---
description: Create quiz for topic
argument-hint: [topic] [question-count] [types]
---
```

**Workflow:**
1. Identify key concepts
2. Generate questions
3. Create answer key
4. Add instructions
5. Output quiz

**Agent:** `assessment-creator`

---

### /assess:test
```yaml
---
description: Create comprehensive test
argument-hint: [unit-or-topics] [format]
---
```

**Workflow:**
1. Map content coverage
2. Generate question bank
3. Balance difficulty
4. Create answer key
5. Output test

**Agent:** `assessment-creator`

---

### /assess:rubric
```yaml
---
description: Create grading rubric
argument-hint: [assignment-type] [criteria]
---
```

**Workflow:**
1. Define criteria
2. Create performance levels
3. Write descriptions
4. Assign points
5. Output rubric

**Agent:** `assessment-creator`

---

### /assess:grade
```yaml
---
description: Grade student work with feedback
argument-hint: [submission] [rubric-or-key]
---
```

**Workflow:**
1. Evaluate against criteria
2. Calculate score
3. Generate feedback
4. Identify improvements
5. Output grade + feedback

**Agent:** `assessment-creator`

---

## 3.5 Analytics Commands

### /analytics:progress
```yaml
---
description: Generate student progress report
argument-hint: [student-or-class] [period]
---
```

**Workflow:**
1. Gather performance data
2. Calculate metrics
3. Identify trends
4. Compare to goals
5. Output progress report

**Agent:** `learning-analyst`

---

### /analytics:gaps
```yaml
---
description: Identify learning gaps
argument-hint: [student-or-class] [subject]
---
```

**Workflow:**
1. Analyze assessment data
2. Identify weak areas
3. Prioritize gaps
4. Recommend interventions
5. Output gap analysis

**Agent:** `learning-analyst`

---

### /analytics:predict
```yaml
---
description: Predict student outcomes
argument-hint: [student-or-class] [target]
---
```

**Workflow:**
1. Gather historical data
2. Apply prediction model
3. Identify at-risk students
4. Recommend actions
5. Output predictions

**Agent:** `learning-analyst`

---

### /analytics:report
```yaml
---
description: Generate analytics dashboard/report
argument-hint: [scope] [metrics] [period]
---
```

**Workflow:**
1. Define report scope
2. Calculate metrics
3. Create visualizations
4. Add insights
5. Output dashboard

**Agent:** `learning-analyst`

---

## 3.6 Content Commands

### /content:slides
```yaml
---
description: Create presentation slides
argument-hint: [topic] [slide-count]
---
```

**Workflow:**
1. Outline content
2. Design slide structure
3. Add visuals/diagrams
4. Include speaker notes
5. Output slide deck

**Agent:** `content-creator`

---

### /content:video
```yaml
---
description: Create video script for lesson
argument-hint: [topic] [duration]
---
```

**Workflow:**
1. Outline content
2. Write script
3. Add visual cues
4. Plan engagement points
5. Output video script

**Agent:** `content-creator`

---

### /content:worksheet
```yaml
---
description: Create student worksheet
argument-hint: [topic] [type]
---
```

**Workflow:**
1. Define learning activity
2. Create content/problems
3. Add instructions
4. Include answer key
5. Output worksheet

**Agent:** `content-creator`

---

### /content:reading
```yaml
---
description: Create reading material
argument-hint: [topic] [reading-level] [length]
---
```

**Workflow:**
1. Research topic
2. Write at appropriate level
3. Add comprehension questions
4. Include vocabulary
5. Output reading material

**Agent:** `content-creator`

---

## 3.7 Support Commands

### /support:question
```yaml
---
description: Answer student question
argument-hint: [question]
---
```

**Workflow:**
1. Understand question
2. Find relevant info
3. Provide clear answer
4. Offer additional help
5. Output response

**Agent:** `student-support`

---

### /support:assignment
```yaml
---
description: Clarify assignment requirements
argument-hint: [assignment]
---
```

**Workflow:**
1. Parse assignment details
2. Explain requirements
3. Clarify expectations
4. Suggest approach
5. Output clarification

**Agent:** `student-support`

---

### /support:study
```yaml
---
description: Provide study tips and strategies
argument-hint: [subject-or-exam]
---
```

**Workflow:**
1. Understand study context
2. Recommend strategies
3. Suggest resources
4. Create study plan
5. Output study guide

**Agent:** `student-support`

---

### /support:resources
```yaml
---
description: Find learning resources
argument-hint: [topic] [type]
---
```

**Workflow:**
1. Identify resource needs
2. Search available materials
3. Curate relevant resources
4. Organize by type
5. Output resource list

**Agent:** `student-support`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/curriculum:lesson` | Create lesson plan | curriculum-designer |
| `/curriculum:unit` | Design unit plan | curriculum-designer |
| `/curriculum:map` | Curriculum mapping | curriculum-designer |
| `/curriculum:objectives` | Learning objectives | curriculum-designer |
| `/tutor:explain` | Explain concept | tutor-assistant |
| `/tutor:practice` | Practice problems | tutor-assistant |
| `/tutor:review` | Study review | tutor-assistant |
| `/tutor:help` | Problem help | tutor-assistant |
| `/assess:quiz` | Create quiz | assessment-creator |
| `/assess:test` | Create test | assessment-creator |
| `/assess:rubric` | Create rubric | assessment-creator |
| `/assess:grade` | Grade with feedback | assessment-creator |
| `/analytics:progress` | Progress report | learning-analyst |
| `/analytics:gaps` | Gap analysis | learning-analyst |
| `/analytics:predict` | Outcome prediction | learning-analyst |
| `/analytics:report` | Analytics dashboard | learning-analyst |
| `/content:slides` | Presentation slides | content-creator |
| `/content:video` | Video script | content-creator |
| `/content:worksheet` | Student worksheet | content-creator |
| `/content:reading` | Reading material | content-creator |
| `/support:question` | Answer question | student-support |
| `/support:assignment` | Assignment help | student-support |
| `/support:study` | Study tips | student-support |
| `/support:resources` | Find resources | student-support |
