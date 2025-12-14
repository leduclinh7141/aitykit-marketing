# AityKit Marketing

**AI-Powered Marketing Automation Framework for Claude Code**

A comprehensive marketing kit that brings systematic, efficient marketing workflows to Claude Code. Plan campaigns, generate content, analyze competitors, and automate marketing operations—all powered by specialized AI agents and the Compounding Marketing philosophy.

**✨ New:** Now includes interactive training modules and plugin architecture from [cc4.marketing](https://github.com/cc4-marketing/cc4.marketing)!

## What is Claude Code?

**Claude Code** is Anthropic's official CLI tool that brings AI-powered development assistance directly to your terminal. It enables natural language interaction with your codebase and provides intelligent automation for common development tasks.

- [Claude Code](https://claude.com/product/claude-code)
- [Docs](https://docs.claude.com/en/docs/claude-code/overview)

**Open Code CLI Coding Agents** extend Claude Code with specialized AI agents that handle specific aspects of software development - from planning and research to testing and documentation. This creates a collaborative AI development team that works alongside human developers.

- [Open Code](https://opencode.ai/)
- [Docs](https://opencode.ai/docs)

## Related Projects & Directories

- `aitykit` - Website of AityKit
  - Directory: `../aitykit`
  - Repo: https://github.com/leduclinh7141/aitykit
- `aitykit-marketing` - Marketing Kit repository
  - Directory: `../aitykit-marketing`
  - Repo: https://github.com/leduclinh7141/aitykit-marketing
- `aitykit-cli` - CLI tool for quick project setup
  - Directory: `../aitykit-cli`
  - Repo: https://github.com/mrgoonie/aitykit-cli
- `aitykit-docs` - Public documentation repository: https://docs.aitykit.cc
  - Directory: `../aitykit-docs`
  - Repo: https://github.com/leduclinh7141/aitykit-docs

## Key Benefits

### 🚀 Accelerated Development
- **AI-Powered Planning**: Automated technical planning and architecture design
- **Intelligent Code Generation**: Context-aware code creation and modification
- **Automated Testing**: Comprehensive test generation and execution
- **Smart Documentation**: Synchronized docs that evolve with your code

### 🎯 Enhanced Quality
- **Multi-Agent Code Review**: Specialized agents for security, performance, and standards
- **Automated Quality Assurance**: Continuous testing and validation
- **Best Practices Enforcement**: Built-in adherence to coding standards
- **Security-First Development**: Proactive security analysis and recommendations

### 🏗️ Structured Workflow
- **Agent Orchestration**: Coordinated AI agents working in parallel and sequential workflows
- **Task Management**: Automated project tracking and progress monitoring
- **Documentation Sync**: Always up-to-date technical documentation
- **Clean Git Workflow**: Professional commit messages and branch management

## Documentation

### 📚 Core Documentation
- **[Project Overview & PDR](./docs/project-overview-pdr.md)** - Comprehensive project overview, goals, features, and product development requirements
- **[Codebase Summary](./docs/codebase-summary.md)** - High-level overview of project structure, technologies, and components
- **[Code Standards](./docs/code-standards.md)** - Coding standards, naming conventions, and best practices
- **[System Architecture](./docs/system-architecture.md)** - Detailed architecture documentation, component interactions, and data flow
- **[Commands Reference](./guide/COMMANDS.md)** - Complete guide to all available slash commands

### 📖 Additional Resources
- **[CLAUDE.md](./CLAUDE.md)** - Development instructions and workflows for AI agents
- **[CHANGELOG.md](./CHANGELOG.md)** - Version history and release notes
- **[Windows Statusline Support](./docs/statusline-windows-support.md)** - Windows compatibility guide for Claude Code statusline
- **[Statusline Architecture](./docs/statusline-architecture.md)** - Technical documentation for statusline implementation

## Quick Start

### For New Users (Start with Training)

Learn marketing automation through hands-on practice:

```bash
# Navigate to project
cd aitykit-marketing

# Launch Claude Code
claude

# Begin interactive training
/training:start-0-0
```

**Time:** 4-6 hours for complete training
**What You'll Build:** Campaign briefs, content library, brand guidelines
**Practice Project:** Markit agency for Planerio client

### For Experienced Users (Jump to Production)

Start using marketing automation immediately:

```bash
# Plan a campaign
/campaign:plan "Q1 Product Launch"

# Generate content
/content:good "Blog post about our new feature"

# SEO research
/seo:keywords "your topic"

# Competitor analysis
/competitor:deep "competitor-url.com"

# Create email sequence
/sequence:welcome "your-product" "trial users"
```

### Installation

**Prerequisites:**
- [Claude Code](https://code.claude.com/docs/en/setup) installed and configured
- Git for version control

**Clone Repository:**
```bash
git clone https://github.com/leduclinh7141/aitykit-marketing.git
cd aitykit-marketing
claude
```

📖 **Complete Documentation:**
- **[Usage Guide](./docs/usage-guide.md)** - Complete command reference and workflows
- **[Training Guide](./training/README.md)** - Interactive learning path
- **[Plugin Guide](./plugins/README.md)** - Plugin system overview
- **[CC4 Integration Summary](./docs/cc4-integration-summary.md)** - What's new details
- **[Commands Reference](./guide/COMMANDS.md)** - All slash commands
- **[Skills Catalog](./guide/SKILLS.md)** - Available marketing skills

## What's New 🎉

### CC4.Marketing Integration (2025-12-14)

✅ **Interactive Training Modules**
- 19 hands-on lessons (`/training:*` commands)
- Practice project: Markit agency → Planerio client
- Learn by doing real marketing work

✅ **Plugin Architecture**
- Content Factory: High-volume content generation
- Campaign Manager: Systematic campaign planning
- Modular, specialized workflows

✅ **Persona Reviewers**
- 6 specialized review agents (Brand, SEO, Conversion, Startup Founder, Marketing Manager, Solopreneur)
- Multi-perspective content validation

✅ **Enhanced Documentation**
- Complete usage guide (`./docs/usage-guide.md`)
- Plugin system overview (`./plugins/README.md`)
- Training guide (`./training/README.md`)

**See:** `./docs/cc4-integration-summary.md` for complete details

## Project Structure

```
├── .claude/                 # Claude Code configuration
│   ├── agents/             # Marketing agents + persona reviewers
│   ├── commands/           # Slash commands + training lessons
│   ├── hooks/              # Claude Code hooks
│   ├── skills/             # Marketing domain skills
│   ├── workflows/          # Core workflows and protocols
│   ├── CLAUDE.md           # Global development instructions
│   └── send-discord.sh     # Notification script
├── plugins/                # Plugin extensions (NEW)
│   ├── content-factory/    # Batch content generation
│   └── campaign-manager/   # Campaign planning & review
├── training/               # Interactive training (NEW)
│   ├── exercises/markit/   # Practice project
│   └── README.md          # Training guide
├── docs/                   # Documentation
│   ├── usage-guide.md     # Complete usage reference (NEW)
│   └── cc4-integration-summary.md  # Integration details (NEW)
├── .opencode/              # Open Code CLI agent definitions
│   ├── agent/              # Specialized agent configurations
│   │   ├── planner.md      # Technical planning agent
│   │   ├── researcher.md   # Research and analysis agent
│   │   ├── tester.md       # Testing and validation agent
│   │   ├── debugger.md     # Issue analysis agent
│   │   ├── code-reviewer.md# Code quality agent
│   │   ├── docs-manager.md # Documentation agent
│   │   ├── git-manager.md  # Version control agent
│   │   └── project-manager.md # Progress tracking agent
│   └── command/            # Custom command definitions
├── docs/                   # Project documentation
│   ├── codebase-summary.md # Auto-generated codebase overview
│   ├── code-standards.md   # Development standards
│   ├── project-overview-pdr.md # Product requirements
│   └── development-roadmap.md  # Project roadmap
├── plans/                  # Implementation plans and reports
│   ├── templates/          # Plan templates
│   └── reports/            # Agent-to-agent communication
├── CLAUDE.md              # Project-specific Claude instructions
├── AGENTS.md              # Agent coordination guidelines
└── README.md              # This file
```

## The AI Agent Team

This boilerplate includes specialized AI agents that work together to deliver high-quality software:

### 🎯 Core Development Agents

#### **Planner Agent**
- Researches technical approaches and best practices
- Creates comprehensive implementation plans
- Analyzes architectural trade-offs
- Spawns multiple researcher agents for parallel investigation

#### **Researcher Agent**
- Investigates specific technologies and frameworks
- Analyzes existing solutions and patterns
- Provides technical recommendations
- Supports the planner with detailed findings

#### **Tester Agent**
- Generates comprehensive test suites
- Validates functionality and performance
- Ensures cross-platform compatibility
- Reports on test coverage and quality metrics

### 🔍 Quality Assurance Agents

#### **Code Reviewer Agent**
- Performs automated code quality analysis
- Enforces coding standards and conventions
- Identifies security vulnerabilities
- Provides improvement recommendations

#### **Debugger Agent**
- Analyzes application logs and error reports
- Diagnoses performance bottlenecks
- Investigates CI/CD pipeline issues
- Provides root cause analysis

### 📚 Documentation & Management Agents

#### **Docs Manager Agent**
- Maintains synchronized technical documentation
- Updates API documentation automatically
- Ensures documentation accuracy
- Manages codebase summaries

#### **Git Manager Agent**
- Creates clean, conventional commit messages
- Manages branching and merge strategies
- Handles version control workflows
- Ensures professional git history

#### **Project Manager Agent**
- Tracks development progress and milestones
- Updates project roadmaps and timelines
- Manages task completion verification
- Maintains project health metrics

## Agent Orchestration Patterns

### Sequential Chaining
Use when tasks have dependencies:
```bash
# Planning → Implementation → Testing → Review
/plan "implement user dashboard"
# Wait for plan completion, then:
/cook "follow the implementation plan"
# After implementation:
/test "validate dashboard functionality"
# Finally:
/review "ensure code quality standards"
```

### Parallel Execution
Use for independent tasks:
```bash
# Multiple researchers exploring different approaches
planner agent spawns:
- researcher (database options)
- researcher (authentication methods)
- researcher (UI frameworks)
# All report back to planner simultaneously
```

### Context Management
- Agents communicate through file system reports
- Context is preserved between agent handoffs
- Fresh context prevents conversation degradation
- Essential information is documented in markdown

## Development Workflow

### 1. Feature Development
```bash
# Start with planning
/plan "add real-time notifications"

# Research phase (automatic)
# Multiple researcher agents investigate approaches

# Implementation
/cook "implement notification system"

# Quality assurance
/test
/review

# Documentation update
/docs

# Project tracking
/watzup  # Check project status
```

### 2. Bug Fixing
```bash
# Analyze the issue
/debug "investigate login failures"

# Create fix plan
/plan "resolve authentication bug"

# Implement solution
/fix "authentication issue"

# Validate fix
/test
```

### 3. Documentation Management
```bash
# Update documentation
/docs

# Generate codebase summary
repomix  # Creates ./docs/codebase-summary.md

# Review project status
/watzup
```

## Configuration Files

### CLAUDE.md
Project-specific instructions for Claude Code. Customize this file to define:
- Project architecture guidelines
- Development standards and conventions
- Agent coordination protocols
- Specific workflows for your project

### .opencode/agent/*.md
Individual agent configurations defining:
- Agent expertise and responsibilities
- Interaction patterns
- Output formats
- Quality standards

### plans/templates/*.md
Reusable templates for:
- Feature implementation plans
- Bug fix procedures
- Refactoring strategies
- Architecture decisions

## Gemini Skills Configuration

This project includes several Gemini-powered skills that require a Google Gemini API key:

- **gemini-audio** - Audio analysis and speech generation
- **gemini-video-understanding** - Video analysis and understanding
- **gemini-document-processing** - PDF document processing
- **gemini-image-gen** - AI image generation
- **gemini-vision** - Image analysis and vision capabilities

### API Key Setup

The Gemini skills check for `GEMINI_API_KEY` in the following order (priority from highest to lowest):

1. **Environment Variable** (Recommended for development)
   ```bash
   export GEMINI_API_KEY='your-api-key-here'
   ```

2. **Project Root `.env`** (Recommended for project-specific keys)
   ```bash
   # Create .env in project root
   echo 'GEMINI_API_KEY=your-api-key-here' > .env
   ```

3. **`.claude/.env`** (For Claude-specific configuration)
   ```bash
   # Copy example and edit
   cp .claude/.env.example .claude/.env
   # Then edit .claude/.env and set your API key
   ```

4. **`.claude/skills/.env`** (For shared skills configuration)
   ```bash
   # Copy example and edit
   cp .claude/skills/.env.example .claude/skills/.env
   # Then edit .claude/skills/.env and set your API key
   ```

5. **Individual Skill Directory `.env`** (For skill-specific keys)
   ```bash
   # Example for gemini-audio skill
   cp .claude/skills/gemini-audio/.env.example .claude/skills/gemini-audio/.env
   # Then edit and set your API key
   ```

### Getting Your API Key

Get your free Gemini API key at: https://aistudio.google.com/apikey

### Vertex AI Support

To use Vertex AI instead of Google AI Studio:

```bash
# Enable Vertex AI
export GEMINI_USE_VERTEX=true
export VERTEX_PROJECT_ID=your-gcp-project-id
export VERTEX_LOCATION=us-central1  # Optional, defaults to us-central1
```

Or in `.env` file:
```
GEMINI_USE_VERTEX=true
VERTEX_PROJECT_ID=your-gcp-project-id
VERTEX_LOCATION=us-central1
```

### Usage Examples

```bash
# Audio analysis
claude "Analyze this audio file and summarize the key points: audio.mp3"

# Video understanding
claude "Describe what happens in this video: video.mp4"

# Document processing
claude "Extract all tables from this PDF: document.pdf"

# Image generation
claude "Generate an image of a serene mountain landscape"

# Image analysis
claude "What objects are in this image: photo.jpg"
```

## Model Context Protocol (MCP)

✍️ Please read [my technical blog article about MCP here](https://faafospecialist.substack.com/p/claude-code-solution-to-use-mcp-servers).

### Pre-requisites

In AityKit, you need to setup the MCP servers in `.claude/.mcp.json` file.

Copy the example file:
```bash
mv .claude/.mcp.json.example .claude/.mcp.json
```

Then add your MCP servers, below are some examples:

### [Context7](https://github.com/upstash/context7)
```json
{
   "mcpServers": {
      "context7": {
         "command": "npx",
         "args": ["-y", "@upstash/context7-mcp", "--api-key", "YOUR_API_KEY"],
      }
   }
}
```

### [Human MCP](https://github.com/mrgoonie/human-mcp/)

```json
{
   "mcpServers": {
      "human": {
         "command": "npx",
         "args": ["@goonnguyen/human-mcp@latest"],
         "env": { "GOOGLE_GEMINI_API_KEY": "YOUR_API_KEY" }
      }
   }
}
```

### [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp)
```json
{
   "mcpServers": {
      "chrome-devtools": {
         "command": "npx",
         "args": ["-y", "chrome-devtools-mcp@latest"]
      }
   }
}
```

## Best Practices

### Development Principles
- **YANGI**: You Aren't Gonna Need It - avoid over-engineering
- **KISS**: Keep It Simple, Stupid - prefer simple solutions
- **DRY**: Don't Repeat Yourself - eliminate code duplication

### Code Quality
- All code changes go through automated review
- Comprehensive testing is mandatory
- Security considerations are built-in
- Performance optimization is continuous

### Documentation
- Documentation evolves with code changes
- API docs are automatically updated
- Architecture decisions are recorded
- Codebase summaries are regularly refreshed

### Git Workflow
- Clean, conventional commit messages
- Professional git history
- No AI attribution in commits
- Focused, atomic commits

## Usage Examples

### Starting a New Feature
```bash
# Research and plan
claude "I need to implement user authentication with OAuth2"
# Planner agent creates comprehensive plan

# Follow the plan
claude "Implement the authentication plan"
# Implementation follows the detailed plan

# Ensure quality
claude "Review and test the authentication system"
# Testing and code review agents validate the implementation
```

### Debugging Issues
```bash
# Investigate problem
claude "Debug the slow database queries"
# Debugger agent analyzes logs and performance

# Create solution
claude "Optimize the identified query performance issues"
# Implementation follows debugging recommendations

# Validate fix
claude "Test query performance improvements"
# Tester agent validates the optimization
```

### Project Maintenance
```bash
# Check project health
claude "What's the current project status?"
# Project manager provides comprehensive status

# Update documentation
claude "Sync documentation with recent changes"
# Docs manager updates all relevant documentation

# Plan next sprint
claude "Plan the next development phase"
# Planner creates detailed roadmap for upcoming work
```

## Advanced Features

### Multi-Project Support
- Manage multiple repositories simultaneously
- Shared agent configurations across projects
- Consistent development patterns

### Custom Agent Creation
- Define project-specific agents
- Extend existing agent capabilities
- Create domain-specific expertise

### Integration Capabilities
- Discord notifications for project updates
- GitHub Actions integration
- CI/CD pipeline enhancement

## Customization Guide

### 1. Project Setup
- Update `CLAUDE.md` with your project specifics
- Modify agent configurations in `.opencode/agent/`
- Customize plan templates in `plans/templates/`

### 2. Agent Specialization
- Add domain-specific knowledge to agents
- Create custom agents for unique requirements
- Configure agent interaction patterns

### 3. Workflow Optimization
- Define project-specific commands
- Create shortcuts for common tasks
- Establish team coding standards

## Contributing

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Follow the agent orchestration workflow
4. Ensure all tests pass and documentation is updated
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Learn More

### Claude Code Resources
- [Claude Code Documentation](https://claude.ai/code)
- [Open Code CLI Documentation](https://docs.opencode.ai)
- [Agent Development Guide](https://docs.opencode.ai/agents)

### Community
- [Claude Code Community](https://discord.gg/claude-code)
- [Discussion Forum](https://github.com/anthropic/claude-code/discussions)
- [Example Projects](https://github.com/topics/claude-code)

### Support
- [Issue Tracker](https://github.com/anthropic/claude-code/issues)
- [Feature Requests](https://github.com/anthropic/claude-code/discussions/categories/ideas)
- [Documentation](https://docs.claude.ai/code)

---

**Start building with AI-powered development today!** This boilerplate provides everything you need to create professional software with intelligent agent assistance.