# Contributing to Fair Forward Dataset Explorer

Thank you for your interest in contributing to the Fair Forward Dataset Explorer! This project aims to help researchers and developers better understand AI fairness datasets, and we welcome contributions from the community.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Standards](#coding-standards)
- [Testing Guidelines](#testing-guidelines)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)
- [Feature Requests](#feature-requests)

## Code of Conduct

This project is committed to providing a welcoming and inclusive environment for all contributors. We expect all participants to:

- Be respectful and considerate of others
- Focus on what is best for the community
- Show empathy towards other community members
- Accept constructive feedback gracefully
- Help create a positive environment for everyone

## How Can I Contribute?

### Reporting Bugs

- Use the GitHub issue tracker
- Include a clear and descriptive title
- Describe the exact steps to reproduce the bug
- Provide specific examples to demonstrate the steps
- Describe the behavior you observed after following the steps
- Explain which behavior you expected to see instead and why
- Include details about your environment (OS, browser, Node.js version)

### Suggesting Enhancements

- Use the GitHub issue tracker with the "enhancement" label
- Provide a clear and descriptive title
- Describe the current functionality and why you think it should be enhanced
- Explain how this enhancement would be useful to most users
- List any other similar applications and how they handle this feature

### Code Contributions

- Fix bugs or add features
- Improve documentation
- Add tests
- Optimize performance
- Improve accessibility
- Add new visualization types

## Development Setup

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Git
- Modern web browser

### Getting Started

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/fair-forward-explorer.git
   cd fair-forward-explorer
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Add your Hugging Face API token if you have one
   HUGGINGFACE_API_TOKEN=your_token_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Create a new branch for your changes**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

## Coding Standards

### TypeScript

- Use TypeScript for all new code
- Define proper types for all functions and variables
- Use interfaces for object shapes
- Avoid using `any` type - use proper typing instead
- Use strict TypeScript configuration

### React Components

- Use functional components with hooks
- Follow React best practices
- Use proper prop types and interfaces
- Keep components focused and single-purpose
- Use meaningful component and prop names

### Code Style

- Use 2 spaces for indentation
- Use single quotes for strings
- Use semicolons at the end of statements
- Use camelCase for variables and functions
- Use PascalCase for components and interfaces
- Keep lines under 100 characters
- Add trailing commas in objects and arrays

### File Organization

- Place components in the `src/components/` directory
- Group related components in subdirectories
- Use index files for clean imports
- Keep utility functions in `src/utils/`
- Place types in `src/types/`

## Testing Guidelines

### Writing Tests

- Write tests for all new functionality
- Test both success and error cases
- Use descriptive test names
- Mock external dependencies
- Test component rendering and user interactions

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage

# Run specific test file
npm test -- --testPathPattern=ComponentName
```

### Test Coverage

- Aim for at least 80% test coverage
- Focus on critical business logic
- Test user interactions and edge cases
- Mock API calls and external services

## Pull Request Process

### Before Submitting

1. **Ensure your code follows the coding standards**
2. **Write or update tests** for your changes
3. **Update documentation** if needed
4. **Test your changes** thoroughly
5. **Check that all tests pass**

### Pull Request Guidelines

1. **Use a clear and descriptive title**
2. **Provide a detailed description** of your changes
3. **Reference any related issues** using keywords like "Fixes #123"
4. **Include screenshots** for UI changes
5. **List any breaking changes** or new dependencies

### Pull Request Template

```markdown
## Description
Brief description of what this PR accomplishes.

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
- [ ] All tests pass
- [ ] New tests added for new functionality
- [ ] Manual testing completed

## Screenshots (if applicable)
Add screenshots for UI changes.

## Checklist
- [ ] Code follows the style guidelines
- [ ] Self-review of code completed
- [ ] Documentation updated
- [ ] No console errors or warnings
```

## Code Review Process

1. **Automated checks** must pass (tests, linting, type checking)
2. **At least one maintainer** must approve the PR
3. **Address any feedback** from code reviews
4. **Squash commits** if requested
5. **Maintainers will merge** approved PRs

## Reporting Issues

### Bug Reports

When reporting bugs, please include:

- **Environment details**: OS, browser, Node.js version
- **Steps to reproduce**: Clear, numbered steps
- **Expected behavior**: What you thought would happen
- **Actual behavior**: What actually happened
- **Screenshots**: If applicable
- **Console errors**: Any error messages

### Security Issues

- **Do not** report security vulnerabilities in public issues
- Email security concerns to [security@yourdomain.com]
- Include detailed information about the vulnerability
- Allow time for the security team to respond

## Feature Requests

When requesting features:

- **Explain the problem** you're trying to solve
- **Describe the solution** you'd like to see
- **Provide examples** of similar features in other apps
- **Consider the impact** on existing functionality
- **Think about edge cases** and accessibility

## Getting Help

- **Documentation**: Check the README and inline code comments
- **Issues**: Search existing issues for similar problems
- **Discussions**: Use GitHub Discussions for questions
- **Community**: Join our community channels

## Recognition

Contributors will be recognized in:

- The project README
- Release notes
- GitHub contributors list
- Project documentation

## Questions?

If you have questions about contributing:

- Open a GitHub issue
- Start a GitHub discussion
- Contact the maintainers directly

Thank you for contributing to making AI fairness more accessible and understandable!
