# Contributing to LiteLists

Thank you for your interest in contributing to LiteLists! We appreciate your help in making this project better.

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone. Be kind, constructive, and professional in all interactions.

## How to Contribute

### Reporting Bugs

If you find a bug, please open an issue with:
- A clear, descriptive title
- Steps to reproduce the issue
- Expected behavior vs. actual behavior
- Screenshots (if applicable)
- Your environment (OS, browser, device, etc.)

### Suggesting Features

We love new ideas! To suggest a feature:
- Open an issue with the tag `enhancement`
- Describe the feature and its use case
- Explain why it would be valuable to users
- Consider the MVP scope and project goals

### Submitting Pull Requests

1. **Fork the repository** and create your branch from `main`
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes**
   - Write clear, concise commit messages
   - Follow the existing code style
   - Add comments for complex logic
   - Update documentation as needed

3. **Test your changes**
   - Ensure existing tests pass
   - Add tests for new functionality
   - Test on both web and mobile (if applicable)

4. **Submit the PR**
   - Provide a clear description of the changes
   - Reference any related issues
   - Include screenshots for UI changes
   - Wait for review and address feedback

## Development Workflow

### Setting Up Your Environment

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/LiteLists.git
cd LiteLists

# Add upstream remote
git remote add upstream https://github.com/gavelinrobert-beep/LiteLists.git

# Install dependencies
npm install
```

### Branch Naming Convention

- `feature/` - New features (e.g., `feature/add-dark-mode`)
- `fix/` - Bug fixes (e.g., `fix/list-sync-issue`)
- `docs/` - Documentation updates (e.g., `docs/update-readme`)
- `refactor/` - Code refactoring (e.g., `refactor/api-structure`)

### Commit Message Guidelines

Write clear commit messages that describe what changed and why:

```
feat: add real-time list synchronization

- Implement Supabase realtime subscriptions
- Update list component to handle live updates
- Add error handling for connection issues
```

Format: `type: brief description`

Types:
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, etc.)
- `refactor:` - Code refactoring
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks

## Coding Standards

### General Guidelines

- Write clean, readable, and maintainable code
- Use meaningful variable and function names
- Keep functions small and focused
- Avoid unnecessary complexity

### TypeScript/JavaScript

- Use TypeScript for type safety
- Follow ESLint and Prettier configurations
- Use functional components and hooks in React
- Prefer async/await over promise chains

### React/React Native

- Keep components small and reusable
- Use proper prop types or TypeScript interfaces
- Manage state appropriately (local vs. global)
- Follow React best practices and hooks rules

### CSS/Styling

- Use consistent naming conventions
- Keep styles modular and reusable
- Consider mobile-first responsive design
- Follow the existing design system

## Project Structure

```
LiteLists/
├── apps/
│   ├── web/          # Next.js web application
│   └── mobile/       # Expo mobile application
├── packages/
│   ├── shared/       # Shared utilities and types
│   └── ui/           # Shared UI components
├── supabase/         # Supabase migrations and config
└── docs/             # Additional documentation
```

## Getting Help

- Check existing issues and discussions
- Read the documentation
- Ask questions in issue comments
- Be specific about your problem or question

## License

By contributing to LiteLists, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing to LiteLists! 🎉
