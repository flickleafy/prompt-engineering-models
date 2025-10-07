# Code Review Prompts Collection

This directory contains a comprehensive collection of AI-powered code review prompts designed for pull request analysis. Each prompt is optimized for specific review scenarios and produces structured, actionable feedback.

## 📁 Structure

```text
code_review/
├── code_review_prompts_summary.md          # Main guide with TOC and usage instructions
├── 01-comprehensive-pr-review/              # All-encompassing review
│   └── prompt.md
├── 02-security-focused-review/              # STRIDE threat modeling
│   └── prompt.md
├── 03-performance-optimization-review/      # Performance analysis
│   └── prompt.md
├── 04-architecture-design-review/           # SOLID & design patterns
│   └── prompt.md
├── 05-quick-scan/                           # Rapid 2-minute triage
│   └── prompt.md
├── 06-language-specific/                    # Language-specific reviews
│   ├── README.md
│   ├── python-review.md
│   └── javascript-typescript-review.md
├── 07-test-coverage-quality/                # F.I.R.S.T principles
│   └── prompt.md
├── 08-breaking-changes-api/                 # API compatibility
│   └── prompt.md
├── 09-documentation-review/                 # Documentation quality
│   └── prompt.md
└── 10-cross-file-impact/                   # System-wide analysis
    └── prompt.md
```

## 🚀 Quick Start

1. **Start here**: Read [code_review_prompts_summary.md](./code_review_prompts_summary.md) for an overview and usage guidance

2. **Choose your review type**: Select the appropriate prompt based on your needs:
   - **Quick check?** → Use [05-quick-scan](./05-quick-scan/prompt.md)
   - **Comprehensive review?** → Use [01-comprehensive-pr-review](./01-comprehensive-pr-review/prompt.md)
   - **Security concerns?** → Use [02-security-focused-review](./02-security-focused-review/prompt.md)
   - **Performance critical?** → Use [03-performance-optimization-review](./03-performance-optimization-review/prompt.md)

3. **Customize the prompt**: Replace `{PLACEHOLDERS}` with your PR details

4. **Run the review**: Feed the prompt to your AI model (GPT-4, GPT-5, Claude, etc.)

5. **Act on findings**: Address critical issues, schedule improvements

## 📋 Prompt Categories

### Core Reviews

- **Comprehensive PR Review**: Covers all aspects - quality, security, performance, architecture
- **Quick Scan**: 2-minute rapid triage for common issues

### Specialized Reviews

- **Security-Focused**: STRIDE + OWASP analysis
- **Performance Optimization**: Bottleneck detection and optimization
- **Architecture & Design**: SOLID principles and design patterns
- **Test Coverage & Quality**: F.I.R.S.T principles assessment

### Integration Reviews

- **Breaking Changes & API**: Semantic versioning and compatibility
- **Documentation Review**: Quality and completeness
- **Cross-File Impact**: System-wide integration analysis

### Language-Specific

- **Python**: PEP 8, type hints, modern features
- **JavaScript/TypeScript**: ES6+, TypeScript, React

## 🎯 Usage Patterns

### Pattern 1: Quick Triage

```text
1. Quick Scan (2 min)
2. If issues found → Run targeted review
```

### Pattern 2: Standard PR

```text
1. Quick Scan
2. Comprehensive Review
3. Test Coverage Review
```

### Pattern 3: High-Risk Changes

```text
1. Security-Focused Review
2. Comprehensive Review
3. Test Coverage Review
4. Cross-File Impact Analysis
```

### Pattern 4: Major Refactoring

```text
1. Architecture & Design Review
2. Breaking Changes & API Review
3. Cross-File Impact Analysis
4. Test Coverage Review
5. Documentation Review
```

## 🔧 Customization

Each prompt can be customized by:

- Adding project-specific coding standards
- Adjusting severity thresholds
- Including team conventions
- Adding domain-specific checks
- Modifying output formats

## 📊 Output Format

All prompts produce structured output with:

- **Severity levels**: Critical 🔴, Important 🟡, Minor 🔵
- **Actionable recommendations**: Specific fixes with code examples
- **Approval status**: Ready/Changes Needed/Blocked
- **Confidence level**: High/Medium/Low

## 🤝 Contributing

To add new prompts or improve existing ones:

1. Follow the established structure
2. Include comprehensive checklists
3. Provide clear output formats
4. Add usage examples
5. Update the summary document

## 📖 Additional Resources

- **Best Practices**: See [code_review_prompts_summary.md](./code_review_prompts_summary.md#best-practices-for-using-these-prompts)
- **Example Scenarios**: Check the summary for real-world usage examples
- **Metrics & Evaluation**: Learn how to measure prompt effectiveness

## 🔍 When to Use Which Prompt

| Scenario | Recommended Prompts |
|----------|-------------------|
| New feature (routine) | Quick Scan → Comprehensive → Test Coverage |
| Security-sensitive code | Security → Comprehensive → Test Coverage |
| Performance optimization | Performance → Cross-File Impact → Test Coverage |
| API changes | Breaking Changes → Comprehensive → Documentation |
| Large refactoring | Architecture → Breaking Changes → Cross-File Impact |
| Bug fix (small) | Quick Scan |
| Bug fix (complex) | Comprehensive → Test Coverage |
| Documentation update | Documentation Review |

## ⚡ Pro Tips

1. **Chain prompts**: Run multiple prompts in sequence for comprehensive coverage
2. **Iterate**: Re-run specific prompts after addressing findings
3. **Customize**: Add project-specific rules to prompts
4. **Automate**: Integrate into CI/CD pipelines
5. **Track metrics**: Monitor false positives and coverage over time
6. **Educate**: Share findings with team to improve code quality

## 🎓 Learning Path

1. Start with **Quick Scan** to understand the basics
2. Move to **Comprehensive Review** for full coverage
3. Add **Security** and **Performance** reviews as needed
4. Master **Architecture** and **Cross-File Impact** for complex changes
5. Customize prompts for your specific needs
