# Part 5: Workflow & Configuration Specifications

## 5.1 Primary Education Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Education Workflow

## Learning Cycle Flow

Design → Create → Teach → Assess → Analyze → Improve

### Phase 1: Design
- Delegate to `curriculum-designer` for planning
- Use `instructional-design` skill
- Output: Lesson/unit plans, objectives

### Phase 2: Create
- Delegate to `content-creator` for materials
- Use `content-development` skill
- Output: Slides, worksheets, readings

### Phase 3: Teach
- Delegate to `tutor-assistant` for instruction
- Use `tutoring` skill
- Output: Explanations, guided practice

### Phase 4: Assess
- Delegate to `assessment-creator` for evaluation
- Use `assessment` skill
- Output: Quizzes, tests, grades, feedback

### Phase 5: Analyze
- Delegate to `learning-analyst` for insights
- Use `learning-analytics` skill
- Output: Progress reports, gap analysis

### Phase 6: Support
- Delegate to `student-support` for assistance
- Answer questions, provide guidance
- Output: Student help, resources
```

---

## 5.2 Education Rules

**File:** `.claude/workflows/education-rules.md`

```markdown
# Education Rules

## Instructional Standards
- Align all content to learning objectives
- Use evidence-based pedagogical approaches
- Differentiate for diverse learners
- Include formative assessment checkpoints

## Assessment Standards
- Align assessments to objectives
- Provide clear rubrics and criteria
- Give timely, actionable feedback
- Use multiple assessment types

## Content Standards
- Ensure age/grade appropriateness
- Meet accessibility requirements
- Use inclusive language and examples
- Cite sources appropriately

## Privacy Standards
- Protect student data (FERPA)
- Follow COPPA for minors
- Limit data collection
- Secure all records

## Communication Standards
- Use encouraging, growth-mindset language
- Respond promptly to student questions
- Provide clear instructions
- Maintain appropriate boundaries
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Education Agent Orchestration

## Sequential Workflows

### Course Development Flow
curriculum-designer → content-creator → assessment-creator
1. Design curriculum and objectives
2. Create instructional materials
3. Develop assessments and rubrics

### Learning Support Flow
tutor-assistant → assessment-creator → learning-analyst
1. Provide instruction and practice
2. Assess understanding
3. Analyze and adjust

## Parallel Workflows

### Unit Preparation
- curriculum-designer: Unit plan and objectives
- content-creator: Materials and resources
- assessment-creator: Quizzes and rubrics
→ Complete unit package

### Progress Review
- learning-analyst: Performance analysis
- tutor-assistant: Intervention recommendations
- student-support: Communication to students
→ Comprehensive progress report

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| Objectives defined | curriculum-designer | content-creator |
| Content ready | content-creator | assessment-creator |
| Assessment complete | assessment-creator | learning-analyst |
| Gap identified | learning-analyst | tutor-assistant |
| Student question | student-support | tutor-assistant |
| New unit needed | learning-analyst | curriculum-designer |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-education",
  "description": "AI-powered education kit with specialized agents for curriculum design, tutoring, assessment, analytics, content creation, and student support.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-education.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist educators with curriculum design, content creation, assessment, tutoring, and learning analytics while maintaining educational best practices and student privacy.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Education rules: `./.claude/workflows/education-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## Education Agents

- `curriculum-designer` - Curriculum & lesson planning
- `tutor-assistant` - Personalized tutoring
- `assessment-creator` - Tests & rubrics
- `learning-analyst` - Analytics & insights
- `content-creator` - Educational content
- `student-support` - Student assistance

## Skills Catalog

- `instructional-design` - Pedagogy, planning
- `tutoring` - Instruction, support
- `assessment` - Evaluation, feedback
- `learning-analytics` - Data, insights
- `content-development` - Materials, media
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "canvas": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-canvas"],
      "env": { "CANVAS_API_KEY": "YOUR_KEY", "CANVAS_DOMAIN": "YOUR_DOMAIN" }
    },
    "google-classroom": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-classroom"],
      "env": { "GOOGLE_CREDENTIALS": "YOUR_CREDS" }
    },
    "moodle": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-moodle"],
      "env": { "MOODLE_URL": "YOUR_URL", "MOODLE_TOKEN": "YOUR_TOKEN" }
    },
    "google-docs": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-docs"],
      "env": { "GOOGLE_CREDENTIALS": "YOUR_CREDS" }
    },
    "google-slides": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-slides"],
      "env": { "GOOGLE_CREDENTIALS": "YOUR_CREDS" }
    },
    "youtube": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-youtube"],
      "env": { "YOUTUBE_API_KEY": "YOUR_KEY" }
    },
    "notion": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-notion"],
      "env": { "NOTION_API_KEY": "YOUR_KEY" }
    },
    "kahoot": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-kahoot"],
      "env": { "KAHOOT_API_KEY": "YOUR_KEY" }
    },
    "zoom": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-zoom"],
      "env": { "ZOOM_API_KEY": "YOUR_KEY" }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| Canvas | LMS | HIGH |
| Google Classroom | LMS | HIGH |
| Moodle | LMS | MEDIUM |
| Google Docs | Content | HIGH |
| Google Slides | Presentations | HIGH |
| YouTube | Video content | MEDIUM |
| Notion | Documentation | MEDIUM |
| Kahoot | Gamified assessment | MEDIUM |
| Zoom | Live sessions | MEDIUM |
| Slack | Communication | LOW |
