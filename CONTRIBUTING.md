# Contributing to TestPages

Thank you for your interest in contributing to TestPages! This document provides guidelines and instructions for contributing to this project.

---

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Getting Started](#getting-started)
3. [How to Contribute](#how-to-contribute)
4. [Development Workflow](#development-workflow)
5. [Coding Standards](#coding-standards)
6. [Commit Guidelines](#commit-guidelines)
7. [Pull Request Process](#pull-request-process)
8. [Questions and Support](#questions-and-support)

---

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inspiring community for all. Please be respectful and constructive in your interactions.

### Expected Behavior

- Be respectful and inclusive
- Provide constructive feedback
- Focus on what is best for the project
- Show empathy towards other contributors

### Unacceptable Behavior

- Harassment or discriminatory language
- Trolling or insulting comments
- Public or private harassment
- Publishing others' private information

---

## Getting Started

### Prerequisites

*To be updated based on chosen technology stack*

Current requirements:
- Git for version control
- Text editor or IDE
- Web browser for testing

### Setting Up Your Development Environment

1. **Fork the repository**
   ```bash
   # Click "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/TestPages.git
   cd TestPages
   ```

3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/prof958/TestPages.git
   ```

4. **Install dependencies** *(once project structure is established)*
   ```bash
   # Instructions will be added here
   ```

---

## How to Contribute

### Types of Contributions

We welcome various types of contributions:

1. **Code Contributions**
   - Bug fixes
   - New features
   - Performance improvements
   - Code refactoring

2. **Documentation**
   - README improvements
   - Code comments
   - Tutorial creation
   - Translation

3. **Design**
   - UI/UX improvements
   - Graphics and assets
   - Design mockups

4. **Testing**
   - Bug reports
   - Test case creation
   - Browser compatibility testing

5. **Content**
   - Portfolio content suggestions
   - Copy improvements
   - SEO optimization

---

## Development Workflow

### Before Starting Work

1. **Check existing issues**
   - Look for existing issues or feature requests
   - Comment on the issue to claim it
   - Ask questions if anything is unclear

2. **Create an issue (if needed)**
   - Describe the bug or feature clearly
   - Provide context and examples
   - Wait for approval before starting work

### Working on Changes

1. **Create a new branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/bug-description
   ```

2. **Make your changes**
   - Follow coding standards
   - Write clear, maintainable code
   - Add comments where necessary

3. **Test your changes**
   - Ensure everything works as expected
   - Test across different browsers
   - Check mobile responsiveness

4. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: add new feature description"
   ```

5. **Keep your branch updated**
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

6. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

---

## Coding Standards

### General Guidelines

1. **Write clean, readable code**
   - Use meaningful variable and function names
   - Keep functions small and focused
   - Avoid deep nesting

2. **Comment thoughtfully**
   - Explain "why", not "what"
   - Document complex logic
   - Keep comments up-to-date

3. **Follow existing patterns**
   - Match the style of existing code
   - Use consistent naming conventions
   - Maintain project structure

### HTML Standards

```html
<!-- Use semantic HTML5 elements -->
<header>
  <nav>
    <!-- Navigation -->
  </nav>
</header>

<!-- Use proper indentation (2 spaces) -->
<section id="about">
  <h2>About Me</h2>
  <p>Description text here.</p>
</section>

<!-- Always include alt text for images -->
<img src="photo.jpg" alt="Descriptive text">

<!-- Use lowercase for tags and attributes -->
<div class="container">
  <button type="submit">Submit</button>
</div>
```

### CSS Standards

```css
/* Use meaningful class names (BEM methodology recommended) */
.block__element--modifier {
  /* Properties in alphabetical order */
  color: #333;
  display: flex;
  margin: 0 auto;
}

/* Use consistent spacing */
.selector-1,
.selector-2 {
  property: value;
}

/* Organize by sections */
/* ========================================
   Component Name
   ======================================== */

/* Mobile-first approach */
.element {
  /* Mobile styles */
}

@media (min-width: 768px) {
  .element {
    /* Tablet styles */
  }
}
```

### JavaScript Standards

```javascript
// Use modern ES6+ syntax
const functionName = (param) => {
  // Function body
};

// Use meaningful variable names
const userProfile = getUserProfile();

// Use const by default, let when reassignment needed
const API_URL = 'https://api.example.com';
let counter = 0;

// Add JSDoc comments for functions
/**
 * Calculates the sum of two numbers
 * @param {number} a - First number
 * @param {number} b - Second number
 * @returns {number} Sum of a and b
 */
const add = (a, b) => a + b;

// Handle errors appropriately
try {
  // Code that might throw
} catch (error) {
  console.error('Error message:', error);
}
```

---

## Commit Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, missing semicolons, etc.)
- **refactor**: Code refactoring
- **perf**: Performance improvements
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```bash
feat(hero): add profile image to hero section

fix(navigation): resolve mobile menu toggle issue

docs(readme): update installation instructions

style(css): improve code formatting in main.css

refactor(js): simplify form validation logic

perf(images): optimize image loading with lazy loading
```

### Guidelines

- Use present tense ("add feature" not "added feature")
- Use imperative mood ("move cursor to..." not "moves cursor to...")
- Keep subject line under 50 characters
- Capitalize the subject line
- Don't end the subject line with a period
- Separate subject from body with a blank line
- Wrap body at 72 characters
- Use body to explain what and why, not how

---

## Pull Request Process

### Before Submitting

1. **Ensure your code follows standards**
   - Run linters (if configured)
   - Check formatting
   - Verify no console errors

2. **Update documentation**
   - Update README if needed
   - Add comments to complex code
   - Update relevant docs

3. **Test thoroughly**
   - Test in multiple browsers
   - Check mobile responsiveness
   - Verify all functionality works

### Submitting a Pull Request

1. **Create pull request**
   - Go to your fork on GitHub
   - Click "New Pull Request"
   - Select your branch

2. **Fill out PR template**
   ```markdown
   ## Description
   Brief description of changes
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Documentation update
   - [ ] Code refactoring
   
   ## Testing
   How was this tested?
   
   ## Screenshots (if applicable)
   Add screenshots here
   
   ## Checklist
   - [ ] Code follows project standards
   - [ ] Self-review completed
   - [ ] Documentation updated
   - [ ] Changes tested
   ```

3. **Address review feedback**
   - Respond to comments
   - Make requested changes
   - Push updates to same branch

### After Approval

- Squash commits if requested
- Wait for maintainer to merge
- Delete your branch after merge

---

## Questions and Support

### Getting Help

- **Documentation**: Check PROJECT_ANALYSIS.md and ROADMAP.md
- **Issues**: Search existing issues for answers
- **Discussions**: Use GitHub Discussions for questions
- **Email**: Contact repository owner for private inquiries

### Reporting Bugs

When reporting bugs, include:

1. **Description**: Clear description of the bug
2. **Steps to Reproduce**: How to reproduce the issue
3. **Expected Behavior**: What should happen
4. **Actual Behavior**: What actually happens
5. **Environment**: Browser, OS, screen size
6. **Screenshots**: If applicable

### Suggesting Features

When suggesting features, include:

1. **Use Case**: Why is this feature needed?
2. **Proposal**: How should it work?
3. **Alternatives**: Other solutions considered?
4. **Examples**: Similar implementations elsewhere?

---

## Recognition

Contributors will be recognized in the following ways:

- Listed in README.md contributors section
- Mentioned in release notes
- GitHub contributor badge

---

## Project Maintainers

Current maintainers:
- @prof958 - Project Owner

---

## License

By contributing to TestPages, you agree that your contributions will be licensed under the same license as the project (to be determined).

---

## Additional Resources

- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Conventional Commits](https://www.conventionalcommits.org/)

---

**Thank you for contributing to TestPages!** 🎉

---

*Last Updated: October 20, 2025*
