# Git Commit Message Template

This repository contains a Git commit message template designed to help standardize and streamline commit messages in your projects. Consistent and clear commit messages are essential to maintaining a readable and maintainable project history. This template provides a simple, easy-to-follow structure for writing meaningful commit messages. It is based on the recommendations of [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).

## Tips for Git Messages

1. Separate the title from the description with a blank line.
2. The title should not exceed 50 characters.
3. Capitalize the first word of the title.
4. Do not end the title with a period.
5. Use the imperative mood in the title line.
6. The description should not exceed 72 characters per line.
7. Use the description to explain _what_ and _why_, instead of _how_.

### Recommended Title Types

- **feat**: New feature
- **fix**: Bug fix
- **refactor**: Code refactoring
- **style**: Formatting, missing commas, etc.; no code changes
- **docs**: Documentation changes
- **test**: Add or refactor tests; no production code changes
- **chore**: Changes to the build process or auxiliary tools and libraries such as documentation generation
- **perf**: Code change that improves performance
- **ci**: Changes to CI configuration files and scripts (e.g., GitHub Actions, CircleCI)
- **build**: Changes that affect the build system or external dependencies (e.g., gulp, broccoli, npm)
- **revert**: Reverts a previous commit
- **wip**: Work in progress; for intermediate commits to keep patches reasonably sized
- **hack**: Temporary workaround to move forward; avoid if possible

## Commit Structure

### Title (Subject Line)

- **Purpose**: Summarize changes concisely.
- **Format**: `<type>: <subject>`
- **Example**:

```bash
feat: add user authentication
```

### Body (Detailed Description)

- **Purpose**: Provide a more detailed explanation of the changes made and why.
- **Format**: Use the imperative mood (e.g., "Add", "Fix", "Update"). Wrap text at 72 characters. Separate paragraphs with a blank line.
- **Example**:

```bash
Fix issue with the user login process
by updating the authentication method. The previous method
was not compatible with new security requirements.

This fix ensures users can log in
without errors and improves overall application security.
```

### Footer (Optional)

- **Purpose**: Include any additional information, such as related issue numbers or references.
- **Format**: Use keywords like `Closes`, `Fixes`, `Refs` followed by the issue number.
- **Example**:

```bash
Closes #123
```

### Note

- **Purpose**: Special instructions, test steps, rake tasks, etc.
- **Example**:

```bash
Note:
Special instructions, test steps, rake tasks, etc.
```

### Co-author

- **Purpose**: Include all contributors at the end of the commit message.
- **Format**: `Co-authored-by: name <user@users.noreply.github.com>`
- **Example**:

```bash
Co-authored-by: John Doe <john.doe@example.com>
```

## Example Commit Message

```bash
feat: add user authentication

Add a new feature for user authentication
using JWT. This feature allows users to log in
securely and receive a token for subsequent requests.

- Implement JWT-based authentication
- Add middleware to protect routes
- Update user model with authentication methods

Closes #45

Note:

- Update environment variables with the secret key.
- Apply database migrations.

Co-authored-by: Jane Doe <jane.doe@example.com>
```

## How to Use the Template

1. Clone the Repository: Clone this repository to your local machine.

```bash
git clone git@github.com:brayandiazc/template-gitmessage.git
```

2. Navigate to the Root Directory: Move to the directory where you cloned the repository.

```bash
cd template-gitmessage
```

3. Copy the Template File: Copy the .gitmessage file to your home directory.

```bash
cp .gitmessage ~
```

4. Configure Git: Set the template as your default commit message template by running the following command:

```bash
git config --global commit.template ~/.gitmessage
```

## Author

- [Brayan Diaz C](https://github.com/brayandiazc)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

⌨️ with ❤️ by [Brayan Diaz C](https://github.com/brayandiazc) 😊
