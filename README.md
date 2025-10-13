# Professional Prompt Engineering for Software Development

A comprehensive collection of expertly crafted prompts for AI-assisted software development, with specialized focus on code review, testing, documentation, and development workflows. Designed for use with advanced AI models like GPT-5 and Claude.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Available Prompt Collections](#available-prompt-collections)
- [Getting Started](#getting-started)
- [GPT-5 Meta-Prompting Guide](#gpt-5-meta-prompting-guide)
- [Best Practices](#best-practices)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [License](#license)
- [Resources](#resources)
- [Contact & Support](#contact--support)
- [Supporting the Project](#supporting-the-project)

---

## 🎯 Overview

This repository contains production-ready prompt templates engineered for professional software development workflows. Each prompt is designed with:

- **Structured Output**: Consistent, parseable responses for automation
- **Domain Expertise**: Deep technical knowledge baked into prompts
- **Flexibility**: Adaptable to various project contexts and tech stacks
- **Quality Focus**: Emphasis on security, performance, and best practices

---

## 📚 Available Prompt Collections

### Code Review Prompts

The **[code_review](./code_review/)** directory contains 37+ specialized prompts for comprehensive code review across multiple dimensions:

#### General Review Types (10 prompts)

1. **[Comprehensive PR Review](./code_review/01-comprehensive-pr-review/prompt.md)** - All-encompassing analysis covering quality, security, performance, and architecture
2. **[Security-Focused Review](./code_review/02-security-focused-review/prompt.md)** - STRIDE threat modeling and vulnerability analysis
3. **[Performance Optimization Review](./code_review/03-performance-optimization-review/prompt.md)** - Bottleneck identification and optimization opportunities
4. **[Architecture & Design Review](./code_review/04-architecture-design-review/prompt.md)** - SOLID principles, design patterns, and system design
5. **[Quick Scan](./code_review/05-quick-scan/prompt.md)** - Rapid 2-minute triage for common issues
6. **[Test Coverage & Quality Review](./code_review/07-test-coverage-quality/prompt.md)** - F.I.R.S.T principles and test assessment
7. **[Breaking Changes & API Review](./code_review/08-breaking-changes-api/prompt.md)** - API compatibility and semantic versioning
8. **[Documentation Review](./code_review/09-documentation-review/prompt.md)** - Documentation quality and completeness
9. **[Cross-File Impact Analysis](./code_review/10-cross-file-impact/prompt.md)** - System-wide integration analysis
10. **[Python Review](./code_review/06-language-stack-specific/python-review.md)** - Python-specific best practices

#### Language & Framework Specific Reviews (27 prompts)

**JavaScript/TypeScript Core** (6 prompts)

- Vanilla JS (Frontend/Backend), ES6+ (Frontend/Backend), TypeScript (Frontend/Backend)

**React Ecosystem** (5 prompts)

- React Hooks (JS/TS), React Classes (JS/TS), React Native

**Angular** (2 prompts)

- AngularJS 1.x, Angular 2+

**Vue** (4 prompts)

- Vue 2 (JS/TS), Vue 3 (JS/TS)

**Svelte** (2 prompts)

- Svelte (JS/TS)

**Meta-Frameworks** (2 prompts)

- Next.js (App/Pages Router, SSR/SSG)
- Nuxt.js (Nuxt 3)

**Backend Frameworks** (2 prompts)

- NestJS (Enterprise Node.js)
- Express.js

**API & GraphQL** (1 prompt)

- GraphQL schema, resolvers, performance

**Testing** (1 prompt)

- Jest, Vitest, Cypress (Unit/Integration/E2E)

📖 **[View Complete Code Review Documentation](./code_review/code_review_prompts_summary.md)**

---

### Testing Prompts

The **[testing](./testing/)** directory contains 12+ general testing prompts and framework-specific guides for comprehensive test generation and quality improvement:

#### General Testing Prompts (12 prompts)

1. **[Unit Test Generation](./testing/01-unit-test-generation/prompt.md)** - Generate comprehensive unit tests with edge cases and error handling
2. **[Integration Test Generation](./testing/02-integration-test-generation/prompt.md)** - Create integration tests for APIs, databases, and services
3. **[E2E Test Generation](./testing/03-e2e-test-generation/prompt.md)** - Build complete user workflow tests with Page Object Model
4. **[Test Quality Assessment](./testing/04-test-quality-assessment/prompt.md)** - Evaluate test suite quality using F.I.R.S.T principles
5. **[Coverage Gap Analysis](./testing/05-coverage-gap-analysis/prompt.md)** - Identify untested code paths and edge cases
6. **[Test Refactoring](./testing/06-test-refactoring/prompt.md)** - Improve test readability, maintainability, and DRY
7. **[Mock & Stub Strategy](./testing/07-mock-stub-strategy/prompt.md)** - Design effective mocking approaches for dependencies
8. **[Test Data Factory](./testing/08-test-data-factory/prompt.md)** - Create test fixtures and data builders
9. **[Flaky Test Diagnosis](./testing/09-flaky-test-diagnosis/prompt.md)** - Debug and fix unreliable tests
10. **[Performance Testing](./testing/10-performance-testing/prompt.md)** - Load, stress, and benchmark testing strategies
11. **[Security Testing](./testing/11-security-testing/prompt.md)** - Vulnerability scanning and penetration testing (OWASP)
12. **[Accessibility Testing](./testing/12-accessibility-testing/prompt.md)** - WCAG compliance and a11y testing

#### Language/Framework-Specific Testing (Framework-specific patterns)

- **JavaScript/TypeScript**: Jest, Vitest, Mocha
- **React**: React Testing Library
- **Python**: pytest, unittest
- **E2E Frameworks**: Cypress, Playwright
- **Backend**: NestJS, Express + Supertest
- **API**: REST, GraphQL testing

📖 **[View Complete Testing Documentation](./testing/README.md)**

---
### Refactoring Prompts

The **[refactoring](./refactoring/)** directory contains 10+ specialized prompts for systematic code improvement strategies:

#### Core Refactoring Types (10 prompts)

1. **[Code Smells Detection](./refactoring/01-code-smells-detection/prompt.md)** - Identify long methods, god classes, duplicated code, and other anti-patterns
2. **[SOLID Principles](./refactoring/02-solid-principles/prompt.md)** - Enforce clean architecture principles (SRP, OCP, LSP, ISP, DIP)
3. **[Design Patterns Application](./refactoring/03-design-patterns/prompt.md)** - Strategic application of proven design patterns (creational, structural, behavioral)
4. **[Technical Debt Reduction](./refactoring/04-technical-debt/prompt.md)** - Systematic identification, quantification, and reduction of technical debt
5. **[Performance Refactoring](./refactoring/05-performance-refactoring/prompt.md)** - Algorithmic optimization, database tuning, and resource management
6. **[Testability Improvement](./refactoring/06-testability-improvement/prompt.md)** - Making code test-friendly through dependency injection and clear interfaces
7. **[Readability Enhancement](./refactoring/07-readability-enhancement/prompt.md)** - Improve naming, structure, comments, and code flow
8. **[Modularity & Decoupling](./refactoring/08-modularity-decoupling/prompt.md)** - Reduce coupling, increase cohesion, and define clear boundaries
9. **[Modernization](./refactoring/09-modernization/prompt.md)** - Update to modern language features, APIs, and best practices
10. **[Security Hardening](./refactoring/10-security-hardening/prompt.md)** - Fix vulnerabilities and apply OWASP security guidelines
11. **[Comprehensive Refactoring](./refactoring/12-comprehensive-refactoring/prompt.md)** - Holistic multi-dimensional refactoring strategy
12. **[Extract & Simplify](./refactoring/13-extract-and-simplify/prompt.md)** - Breaking down complex code using extraction techniques
13. **[Legacy Modernization](./refactoring/14-legacy-modernization/prompt.md)** - Systematic transformation of legacy codebases

#### Language & Stack-Specific Refactoring

**[Language-Specific Prompts](./refactoring/11-language-stack-specific/)**

Available now:
- **[Python Refactoring](./refactoring/11-language-stack-specific/python-refactoring.md)** - Pythonic patterns, type hints, modern features
- **[JavaScript/TypeScript Refactoring](./refactoring/11-language-stack-specific/javascript-typescript-refactoring.md)** - ES6+, TypeScript migration, async patterns
- **[React Refactoring](./refactoring/11-language-stack-specific/react-refactoring.md)** - Hooks migration, performance, modern patterns

Coming soon: Java, C#, Go, Rust, Ruby, PHP, Angular, Vue, Spring Boot, Django, .NET

📖 **[View Complete Refactoring Documentation](./refactoring/refactoring_prompts_summary.md)**

### Future Prompt Collections

This repository is designed to accommodate additional prompt collections:

- **🔄 Refactoring Prompts** - Systematic code improvement strategies
- **🧪 Testing Prompts** - Test generation and quality improvement
- **📝 Documentation Prompts** - API docs, README, and technical writing
- **🐛 Debugging Prompts** - Root cause analysis and troubleshooting
- **🏗️ Architecture Prompts** - System design and technical planning

---

## 🚀 Getting Started

### Basic Usage

1. **Select the appropriate prompt** for your task
2. **Copy the prompt template** from the markdown file
3. **Replace placeholders** with your specific context:
   - `{DIFF_CONTENT}` - Your code changes
   - `{PROJECT_CONTEXT}` - Project-specific information
   - `{LANGUAGE}` - Programming language
   - `{FRAMEWORK}` - Framework or library
4. **Submit to your AI model** (GPT-5, Claude, etc.)
5. **Review the structured output** and take action

### Example: Code Review

```markdown
# Using the Comprehensive PR Review prompt

1. Navigate to: code_review/1-comprehensive-pr-review/prompt.md
2. Copy the entire prompt
3. Replace {DIFF_CONTENT} with your git diff output
4. Submit to GPT-5 with high reasoning effort
5. Receive structured feedback with:
   - Code Quality Score (X/10)
   - Critical Issues (🔴)
   - Best Practice Violations (🟡)
   - Optimization Opportunities (🔵)
   - Excellent Practices (✅)
```

---

## 🧠 GPT-5 Meta-Prompting Guide

To maximize the effectiveness of these prompts with GPT-5 and other advanced models, incorporate these meta-prompting tags into your workflow.

### Meta-Prompting Tags Explained

#### `<persistence>`

**Purpose**: Ensures the AI agent completes the entire task autonomously without premature termination.

**Key Behaviors**:

- Continue working until the user's query is completely resolved
- Only terminate when the problem is definitively solved
- Never stop when encountering uncertainty—research or deduce the most reasonable approach
- Don't ask for confirmation or clarification—make informed assumptions and document them
- Act as an autonomous agent, not a conversational assistant

**Example**:

```xml
<persistence>
- You are an agent - please keep going until the user's query is completely resolved
- Only terminate your turn when you are sure that the problem is solved
- Never stop when you encounter uncertainty — research or deduce the most reasonable approach and continue
- Do not ask the human to confirm or clarify assumptions — decide what the most reasonable assumption is, proceed with it, and document it for the user's reference after you finish acting
</persistence>
```

---

#### `<exploration>`

**Purpose**: Guides thorough investigation and planning before implementation.

**Key Behaviors**:

- Never guess—always use tools to read files and gather information
- Decompose requests into explicit requirements, unclear areas, and hidden assumptions
- Map the scope: identify relevant codebase regions, files, functions, or libraries
- Check dependencies: frameworks, APIs, config files, data formats, versioning
- Resolve ambiguity proactively based on repo context and conventions
- Define the output contract: exact deliverables, expected outputs, tests passing
- Formulate an execution plan with research steps and testing strategy

**Example**:

```xml
<exploration>
If you are not sure about file content or codebase structure, use your tools to read files and gather information: do NOT guess or make up an answer.
Before coding, always:
- Decompose the request into explicit requirements, unclear areas, and hidden assumptions
- Map the scope: identify the codebase regions, files, functions, or libraries likely involved
- Check dependencies: frameworks, APIs, config files, data formats, versioning
- Resolve ambiguity proactively based on repo context and conventions
- Define the output contract: exact deliverables, tests passing, etc.
- Formulate an execution plan with research and testing strategy
</exploration>
```

---

#### `<tool_preambles>`

**Purpose**: Structures AI communication for clarity and transparency.

**Key Behaviors**:

- Begin by rephrasing the user's goal in friendly, clear, concise language
- Immediately outline a structured plan detailing each logical step
- Narrate each step succinctly and sequentially during execution
- Mark progress clearly as you work through tasks
- Finish by summarizing completed work distinctly from the upfront plan

**Example**:

```xml
<tool_preambles>
- Always begin by rephrasing the user's goal in a friendly, clear, and concise manner
- Then, immediately outline a structured plan detailing each logical step
- As you execute, narrate each step succinctly and sequentially, marking progress clearly
- Finish by summarizing completed work distinctly from your upfront plan
</tool_preambles>
```

---

#### `<self_reflection>`

**Purpose**: Ensures the AI produces world-class, thoroughly evaluated outputs.

**Key Behaviors**:

- Create an internal quality rubric with 5-7 categories
- Think deeply about what makes an excellent solution
- Use the rubric to evaluate and iterate on the solution internally
- If not hitting top marks across all categories, start again and improve
- Don't show the rubric to users—it's for internal quality control

**Example**:

```xml
<self_reflection>
- First, spend time thinking of a rubric until you are confident
- Create a rubric with 5-7 categories for evaluating solution quality
- Think deeply about every aspect of what makes for a world-class solution
- Use the rubric to internally iterate on the best possible solution
- If your response is not hitting top marks across all categories, start again
</self_reflection>
```

---

#### `<reasoning_effort>`

**Purpose**: Controls how deeply the model thinks and analyzes before responding.

**Key Behaviors**:

- Scale reasoning effort based on task difficulty
- Use **low** for simple, straightforward tasks
- Use **medium** (default) for moderate complexity
- Use **high** for complex, multi-step tasks requiring deep analysis
- Higher reasoning improves output quality for complex problems
- Break separable tasks across multiple turns for peak performance

**Reasoning Effort Levels**:

- **Low**: Quick responses, simple tasks, well-defined problems
- **Medium**: Balanced thinking for moderate complexity
- **High**: Deep analysis, multi-step reasoning, complex problem-solving

**When to Use High Reasoning**:

- Code reviews requiring security and architecture analysis
- Complex refactoring decisions
- Multi-file impact analysis
- Performance optimization requiring algorithmic changes
- System design and architecture decisions

**Example**:

```xml
<reasoning_effort>
For this code review task requiring security analysis, architecture evaluation, and cross-file impact assessment, use HIGH reasoning effort to ensure comprehensive analysis across all dimensions.
</reasoning_effort>
```

---

#### `<code_editing_rules>`

**Purpose**: Establishes comprehensive standards for code quality, structure, and user experience.

**Key Behaviors**:

- Follow guiding principles for clarity, reusability, and consistency
- Adhere to specified technology stack defaults
- Apply UI/UX best practices throughout implementation
- Maintain high visual quality standards

**Subsections Explained**:

**`<guiding_principles>`** - Core development philosophy:

- **Clarity and Reuse**: Every component and page should be modular and reusable. Avoid duplication by factoring repeated UI patterns into components
- **Consistency**: The user interface must adhere to a consistent design system—color tokens, typography, spacing, and components must be unified
- **Simplicity**: Favor small, focused components and avoid unnecessary complexity in styling or logic
- **Demo-Oriented**: The structure should allow for quick prototyping, showcasing features like streaming, multi-turn conversations, and tool integrations
- **Visual Quality**: Follow high visual quality standards (spacing, padding, hover states, etc.)

**`<frontend_stack_defaults>`** - Standard technology choices:

- **Framework**: Next.js (TypeScript)
- **Styling**: TailwindCSS
- **UI Components**: shadcn/ui
- **Icons**: Lucide
- **State Management**: Zustand
- **Directory Structure**: Standardized organization with `/app`, `/components`, `/hooks`, `/lib`, `/stores`, `/types`, `/styles`

**`<ui_ux_best_practices>`** - User experience guidelines:

- **Visual Hierarchy**: Limit typography to 4–5 font sizes and weights for consistent hierarchy; use `text-xs` for captions and annotations; avoid `text-xl` unless for hero or major headings
- **Color Usage**: Use 1 neutral base (e.g., `zinc`) and up to 2 accent colors for visual consistency
- **Spacing and Layout**: Always use multiples of 4 for padding and margins to maintain visual rhythm. Use fixed height containers with internal scrolling when handling long content streams
- **State Handling**: Use skeleton placeholders or `animate-pulse` to indicate data fetching. Indicate clickability with hover transitions (`hover:bg-*`, `hover:shadow-md`)
- **Accessibility**: Use semantic HTML and ARIA roles where appropriate. Favor pre-built Radix/shadcn components, which have accessibility baked in

**Example**:

```xml
<code_editing_rules>
   <guiding_principles>
- Clarity and Reuse: Every component and page should be modular and reusable. Avoid duplication by factoring repeated UI patterns into components.
- Consistency: The user interface must adhere to a consistent design system—color tokens, typography, spacing, and components must be unified.
- Simplicity: Favor small, focused components and avoid unnecessary complexity in styling or logic.
- Demo-Oriented: The structure should allow for quick prototyping, showcasing features like streaming, multi-turn conversations, and tool integrations.
- Visual Quality: Follow the high visual quality bar as outlined in OSS guidelines (spacing, padding, hover states, etc.)
   </guiding_principles>
   <frontend_stack_defaults>
- Framework: Next.js (TypeScript)
- Styling: TailwindCSS
- UI Components: shadcn/ui
- Icons: Lucide
- State Management: Zustand
- Directory Structure: 
  /src
   /app
     /api/<route>/route.ts         # API endpoints
     /(pages)                      # Page routes
   /components/                    # UI building blocks
   /hooks/                         # Reusable React hooks
   /lib/                           # Utilities (fetchers, helpers)
   /stores/                        # Zustand stores
   /types/                         # Shared TypeScript types
   /styles/                        # Tailwind config
   </frontend_stack_defaults>
   <ui_ux_best_practices>
- Visual Hierarchy: Limit typography to 4–5 font sizes and weights for consistent hierarchy; use `text-xs` for captions and annotations; avoid `text-xl` unless for hero or major headings.
- Color Usage: Use 1 neutral base (e.g., `zinc`) and up to 2 accent colors. 
- Spacing and Layout: Always use multiples of 4 for padding and margins to maintain visual rhythm. Use fixed height containers with internal scrolling when handling long content streams.
- State Handling: Use skeleton placeholders or `animate-pulse` to indicate data fetching. Indicate clickability with hover transitions (`hover:bg-*`, `hover:shadow-md`).
- Accessibility: Use semantic HTML and ARIA roles where appropriate. Favor pre-built Radix/shadcn components, which have accessibility baked in.
   </ui_ux_best_practices>
</code_editing_rules>
```

---

#### `<context_understanding>`

**Purpose**: Ensures comprehensive context gathering before action.

**Key Behaviors**:

- If an edit may partially fulfill the query but you're not confident, gather more information
- Bias towards not asking the user for help if you can find the answer yourself
- Use available tools to understand the full context before making changes
- Verify assumptions through exploration rather than guessing

**Example**:

```xml
<context_understanding>
If you've performed an edit that may partially fulfill the user's query, but you're not confident, gather more information or use more tools before ending your turn.
Bias towards not asking the user for help if you can find the answer yourself.
</context_understanding>
```

---

### Complete Meta-Prompt Template

Here's how to structure a complete meta-prompt for GPT-5:

```xml
<persistence>
- You are an agent - keep going until the user's query is completely resolved
- Only terminate when you are sure the problem is solved
- Never stop on uncertainty — research and continue
- Don't ask for confirmation — make reasonable assumptions and document them
</persistence>

<reasoning_effort>
Use HIGH reasoning effort for this complex task requiring deep analysis across multiple dimensions.
</reasoning_effort>

<exploration>
Before acting:
- Decompose the request into requirements and assumptions
- Map the scope and identify relevant code regions
- Check dependencies and resolve ambiguity proactively
- Define the output contract and formulate an execution plan
</exploration>

<self_reflection>
- Create an internal quality rubric with 5-7 categories
- Iterate until the solution hits top marks across all categories
- Don't show the rubric — use it for internal quality control
</self_reflection>

<tool_preambles>
- Rephrase the user's goal clearly
- Outline a structured plan
- Narrate each step during execution
- Summarize completed work at the end
</tool_preambles>

<code_editing_rules>
   <guiding_principles>
- Clarity and Reuse: Every component should be modular and reusable
- Consistency: Adhere to a unified design system
- Simplicity: Favor small, focused components
- Visual Quality: Follow spacing, padding, hover state best practices
   </guiding_principles>
   <frontend_stack_defaults>
- Framework: Next.js (TypeScript)
- Styling: TailwindCSS
- UI Components: shadcn/ui
- Icons: Lucide
- State Management: Zustand
   </frontend_stack_defaults>
   <ui_ux_best_practices>
- Visual Hierarchy: Limit typography to 4-5 font sizes
- Color Usage: Use 1 neutral base and up to 2 accent colors
- Spacing: Use multiples of 4 for padding and margins
- Accessibility: Use semantic HTML and ARIA roles
   </ui_ux_best_practices>
</code_editing_rules>

<context_understanding>
- Gather all necessary context before acting
- Use tools to find answers rather than asking the user
- Verify assumptions through exploration
</context_understanding>
```

---

## 💡 Best Practices

### For Individual Developers

1. **Start Simple**: Use Quick Scan for initial triage, then deep dive with specific prompts
2. **Combine Prompts**: Chain multiple prompts for comprehensive analysis
3. **Customize**: Adapt prompts to your project's specific standards and requirements
4. **Iterate**: Use feedback loops—review, fix, re-review
5. **Learn**: Pay attention to patterns in AI feedback to improve your coding

### For Teams

1. **Standardize**: Agree on which prompts to use for different scenarios
2. **Integrate**: Incorporate prompts into CI/CD pipelines
3. **Track Metrics**: Monitor false positive rates, time saved, issues caught
4. **Train**: Educate team members on effective prompt usage
5. **Customize**: Create team-specific variants with project conventions

### For Organizations

1. **Establish Guidelines**: Define when to use AI review vs. human review
2. **Quality Gates**: Set thresholds for AI-detected issues in CI/CD
3. **Audit**: Regularly review AI suggestions for accuracy and relevance
4. **Feedback Loop**: Collect developer feedback to improve prompts
5. **Compliance**: Ensure AI usage aligns with security and privacy policies

---

## 📖 Usage Examples

### Example 1: Security-Critical Feature Review

```bash
# Scenario: Adding payment processing module
# Risk Level: High
# Prompt Sequence:

1. Security-Focused Review (Critical) → Identify vulnerabilities
2. Comprehensive PR Review → Overall quality check
3. Test Coverage Review → Ensure adequate testing
4. API Review → Verify PCI compliance
5. Documentation Review → Ensure security procedures are documented
```

### Example 2: React Component Development

```bash
# Scenario: New dashboard component with TypeScript
# Framework: React + TypeScript
# Prompt Sequence:

1. React Hooks (TS) Language-Specific Review → Framework best practices
2. Quick Scan → Common issues check
3. Performance Optimization Review → Rendering performance
4. Test Coverage Review → Component testing adequacy
5. Documentation Review → Props and usage documentation
```

### Example 3: Backend API with NestJS

```bash
# Scenario: REST API endpoints with authentication
# Framework: NestJS + TypeScript
# Prompt Sequence:

1. NestJS Language-Specific Review → Framework patterns
2. Security-Focused Review → Auth vulnerabilities
3. API Review → Breaking changes check
4. Testing Review (Jest) → Unit and integration tests
5. Documentation Review → API documentation
```

### Example 4: Performance Optimization

```bash
# Scenario: Database query layer optimization
# Focus: Performance
# Prompt Sequence:

1. Performance Optimization Review → Identify bottlenecks
2. Language-Specific Review (TypeScript Backend) → Code quality
3. Cross-File Impact Analysis → System-wide effects
4. Test Coverage Review → Performance benchmarks
5. Documentation Review → Performance expectations
```

---

## 🤝 Contributing

We welcome contributions to expand and improve this prompt library!

### How to Contribute

1. **Fork** the repository
2. **Create a branch** for your prompt collection or improvement
3. **Follow the existing structure**:
   - Create a directory for your prompt category
   - Include comprehensive documentation
   - Provide usage examples
   - Test prompts with real scenarios
4. **Submit a pull request** with:
   - Clear description of the prompt's purpose
   - Example usage and expected outputs
   - Any relevant context or limitations

### Prompt Quality Guidelines

- **Specific**: Target a well-defined use case
- **Structured**: Produce consistent, parseable output
- **Comprehensive**: Cover all relevant aspects of the domain
- **Tested**: Validated with real-world examples
- **Documented**: Include clear usage instructions

---

## 📄 License

This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)** for **personal and non-commercial use only**.

### Personal Use

For personal, educational, and non-commercial purposes, this project is freely available under the GPL-3.0 license:

✅ **You Can**:

- Use these prompts for personal projects and learning
- Modify and adapt the prompts for non-commercial purposes
- Contribute improvements back to the project

⚠️ **You Must**:

- Disclose source and include license notices
- Share modifications under the same GPL-3.0 license
- Clearly state any significant changes made to original prompts

❌ **You Cannot**:

- Sublicense under different terms
- Hold authors liable for damages

### Commercial Use

**Commercial use of this software requires a separate commercial license.**

Commercial use includes, but is not limited to:

- Integration into commercial products or services
- Use within organizations generating revenue
- Deployment in enterprise or production environments for business purposes
- Distribution as part of commercial offerings

For commercial licensing inquiries, please contact inbox.

We offer flexible commercial licensing options tailored to your organization's needs, including support and maintenance agreements.

### Full License Text

The GPL-3.0 license terms for non-commercial use can be found in the [LICENSE](./LICENSE) file.

```text
Copyright (C) 2022-2026 flickleafy

This program is free software for personal use: you can redistribute it 
and/or modify it under the terms of the GNU General Public License as 
published by the Free Software Foundation, either version 3 of the License, 
or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

Commercial use requires a separate commercial license. Please contact
the copyright holder for commercial licensing terms.
```

---

## 🔗 Resources

- **OpenAI GPT-5 Documentation**: [GPT-5 Prompting Guide](https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide)
- **Code Review Best Practices**: [./code_review/code_review_prompts_summary.md](./code_review/code_review_prompts_summary.md)
- **Language-Specific Prompts**: [./code_review/06-language-stack-specific/](./code_review/6-language-stack-specific/)

---

## 📬 Contact & Support

- **Issues**: Open an issue on GitHub for bugs or feature requests
- **Discussions**: Use GitHub Discussions for questions and ideas
- **Contributions**: See [Contributing](#contributing) section above

---

## 💝 Supporting the Project

This project is open-source and freely available under the GPL-3.0 license. If these prompts have helped improve your development workflow or saved you time, consider supporting continued development and maintenance.

### Ways to Support

**⭐ Star the Repository** - Help others discover these prompts by starring the project on GitHub

**🔗 Share & Recommend** - Share with colleagues, teams, or on social media

**📝 Contribute** - Submit new prompts, improvements, or bug fixes

**☕ Sponsor Development** - Financial contributions help maintain and expand the prompt library:

- **GitHub Sponsors**: [Support via GitHub Sponsors](https://github.com/sponsors/flickleafy)
- **Buy Me a Coffee**: One-time or recurring support for ongoing development
- **Open Collective**: Transparent funding for community-driven improvements

### What Your Support Enables

- 🚀 Development of new specialized prompts
- 📚 Comprehensive documentation and examples
- 🔄 Regular updates for new AI model capabilities
- 🐛 Bug fixes and prompt refinements
- 🌍 Community support and engagement

**All support is voluntary and appreciated, but never required.** These prompts will always remain free and open-source.

---

**Built with ❤️ for the software development community**
