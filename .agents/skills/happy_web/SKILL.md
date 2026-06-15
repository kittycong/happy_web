```markdown
# happy_web Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `happy_web` TypeScript codebase. It covers file organization, code style, commit practices, and testing patterns, providing clear examples and step-by-step workflows for efficient contribution and maintenance.

## Coding Conventions

### File Naming
- Use **kebab-case** for all file names.
  - Example:  
    ```
    user-profile.ts
    app-config.ts
    ```

### Import Style
- Use **relative imports** for referencing modules.
  - Example:
    ```typescript
    import { fetchData } from './utils/fetch-data';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // In utils/math.ts
    export function add(a: number, b: number): number {
      return a + b;
    }
    ```

### Commit Messages
- Follow **conventional commit** format.
- Common prefixes: `docs`, `feat`
- Example:
  ```
  feat: add user authentication module
  docs: update README with setup instructions
  ```

## Workflows

### Feature Development
**Trigger:** When implementing a new feature  
**Command:** `/feature-development`

1. Create a new branch for your feature.
2. Use kebab-case for any new files.
3. Write TypeScript code using relative imports and named exports.
4. Commit changes with a `feat:` prefix and a concise description.
5. Open a pull request for review.

### Documentation Update
**Trigger:** When updating or adding documentation  
**Command:** `/docs-update`

1. Edit or create documentation files as needed.
2. Commit changes with a `docs:` prefix and a concise description.
3. Open a pull request for review.

## Testing Patterns

- Test files follow the `*.test.*` naming convention.
  - Example: `user-profile.test.ts`
- The specific testing framework is not detected; follow existing patterns in the repository.
- Place test files alongside the modules they test or in a dedicated `tests` directory, as per project structure.
- Example test file:
  ```typescript
  // user-profile.test.ts
  import { getUserProfile } from './user-profile';

  describe('getUserProfile', () => {
    it('returns correct user data', () => {
      // test implementation
    });
  });
  ```

## Commands
| Command                | Purpose                                      |
|------------------------|----------------------------------------------|
| /feature-development   | Start a new feature development workflow     |
| /docs-update           | Update or add documentation                  |
```
