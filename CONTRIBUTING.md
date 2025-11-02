# Contributing to GoldenPine MCP Server

## Contribution Types

**Accepted contributions:**
- Usage examples (function demonstrations)
- Tutorials (multi-step implementations)
- Edge case documentation (error solutions)
- Bug reports (MCP server issues)

**Not accepted:**
- Duplicate content
- Untested code
- Off-topic material
- Improperly formatted submissions

## Submission Process

### Standard Workflow

1. Fork repository
2. Create topic branch
3. Add content following format specifications
4. Test code in TradingView
5. Submit pull request
6. Respond to review feedback

### Using GitHub Desktop

1. Fork repository via GitHub web interface
2. Clone to local machine via GitHub Desktop
3. Create new branch in GitHub Desktop
4. Add files to appropriate directory
5. Commit changes
6. Push to fork via GitHub Desktop
7. Create pull request via GitHub web interface

## Format Specifications

### Examples

**File location**: `examples/[category]/[function-name]-[use-case].md`

**Required format:**

```markdown
## Example: [Function] - [Use Case]

**Category**: [Trend/Momentum/Volume/Other]
**Difficulty**: [Beginner/Intermediate/Advanced]
**Contributor**: [@username]

### Description
[1-2 sentence explanation]

### Code
```pine
//@version=6
indicator("[Name]", overlay=true)
// Implementation with comments
```

### Output
[Expected result description]

### Key Concepts
- Concept 1: Explanation
- Concept 2: Explanation

### Common Mistakes
- Error pattern: Prevention method

### Related
- [Function]: [Connection]
```

### Tutorials

**File location**: `tutorials/[difficulty]/[topic].md`

**Required format:**

```markdown
## Tutorial: [Name]

**Goal**: [Learning objective]
**Prerequisites**: [Required knowledge]
**Difficulty**: [Beginner/Intermediate/Advanced]
**Contributor**: [@username]

### Introduction
[Tutorial purpose and scope]

### Step 1: [Title]
[Instructions]

```pine
// Step code
```

[Explanation]

[Repeat for all steps]

### Complete Code
```pine
//@version=6
// Full implementation
```

### Verification
[Testing instructions]

### Troubleshooting
- Issue: Solution
```

### Edge Cases

**File location**: `edge-cases/[issue-description].md`

**Required format:**

```markdown
## Edge Case: [Issue]

**Functions Affected**: [List]
**Severity**: [Low/Medium/High]
**Contributor**: [@username]

### Problem
[Clear description]

### Failing Code
```pine
// Demonstrates issue
```

**Error**: [Message if applicable]

### Root Cause
[Technical explanation]

### Solution
```pine
// Corrected implementation
```

### Prevention
- Technique 1
- Technique 2
```

## Validation Requirements

**All submissions must:**
- Use Pine Script v6 syntax
- Include tested, working code
- Follow format specifications exactly
- Provide clear explanations
- Add educational value

**Submissions will be rejected if:**
- Code untested or broken
- Format not followed
- Duplicate existing content
- Lacks proper documentation
- Contains plagiarized material

## Review Process

1. Automated format validation (if configured)
2. Maintainer code testing in TradingView
3. Technical review for accuracy
4. Feedback provided if changes required
5. Merge upon approval
6. Contributor added to CONTRIBUTORS.md

**Expected timeline**: 2-3 days for review

## Quality Standards

**Code requirements:**
- Syntax valid for Pine Script v6
- Comments explain non-obvious logic
- Follows TradingView best practices
- Demonstrates stated concept clearly

**Documentation requirements:**
- Technical accuracy
- Clear explanations for target difficulty
- Appropriate detail level
- Professional tone

## LLM-Assisted Formatting (Optional)

Contributors may use language models to format submissions. Provide the following template to your LLM:

**For Examples:**

```
Format this Pine Script example for GoldenPine MCP Server contribution:

Function: [function name]
Use case: [specific application]
Difficulty: [level]
Code: [paste code]
Output: [expected result]
Key concepts: [2-3 concepts]
Common mistakes: [1-2 errors to avoid]

Generate in exact format specified in CONTRIBUTING.md Examples section.
```

**For Tutorials:**

```
Format this Pine Script tutorial for GoldenPine MCP Server contribution:

Goal: [learning objective]
Prerequisites: [required knowledge]
Difficulty: [level]
Steps: [provide each step with code and explanation]
Common issues: [problems users may encounter]

Generate in exact format specified in CONTRIBUTING.md Tutorials section.
```

Verify LLM output matches format specifications before submission.

## Technical Support

**Questions**: Open GitHub issue with [QUESTION] tag  
**Problems**: Open GitHub issue with [BUG] tag  
**Discussion**: Use GitHub Discussions if enabled

---

**Contribution Standards Version**: 1.0  
**Last Updated**: 2025-11-02
