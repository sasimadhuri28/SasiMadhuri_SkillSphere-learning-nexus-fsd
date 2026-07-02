# Day 1 - GitHub Repository Creation

**Date:** 29 June 2026

---

## Objective
Create a GitHub repository for the SkillSphere Learning Nexus project.

---

## Repository Name

```text
SasiMadhuri_SkillSphere-learning-nexus-fsd
```

---

## Steps Performed

### 1. Logged in to GitHub
- Signed in to my GitHub account.

### 2. Created a New Repository
- Clicked on **New Repository**.
- Entered the repository name:
  `SasiMadhuri_SkillSphere-learning-nexus-fsd`

### 3. Repository Settings
- Selected repository visibility as **Public**.
- Added a **README.md** file.
- Added an **MIT License** to allow others to use, modify, and distribute the project.
- Created the repository.

### 4. Repository Successfully Created
The repository was successfully created and is ready for development and collaboration.

---

## Key Learnings

- Learned how to create a repository on GitHub.
- Understood the purpose of README and License files.
- Learned about the MIT License and its importance in open-source projects.
- Understood the difference between Public and Private repositories.

---

## Outcome

Successfully created the GitHub repository with an MIT License:

`SasiMadhuri_SkillSphere-learning-nexus-fsd`

# Day 2 - JWT Authentication Basics

**Date:** 30 June 2026

---

## Objective

To understand the basics of JWT (JSON Web Token), token generation, validation, hashing, and authentication flow between client and server.

---

## Topics Covered

### 1. What is JWT?

JWT (JSON Web Token) is a lightweight and secure way to transfer information between a client and a server.

- JWT is mainly used for authentication and authorization.
- It allows secure communication between client and server.
- After successful login, the server generates a JWT token and sends it to the client.

---

## 2. Why do we use JWT?

- To verify user identity.
- To provide secure access to protected resources.
- To avoid storing user session information on the server.

---

## 3. Authentication Flow using JWT

1. User enters credentials (username and password).
2. Backend API verifies the credentials.
3. If credentials are valid, the server generates a JWT token.
4. The token is sent to the client.
5. The client sends the token with every request.
6. The server validates the token before processing the request.

---

## 4. Components of JWT

A JWT consists of three parts:

### Header
Contains information about the algorithm and token type.

Example:

```json
{
  "alg": "HS256",
  "typ": "JWT"
}
```

### Payload
Contains user-related information (claims).

Examples:

- User ID
- Username
- Roles

Example:

```json
{
  "userId": 101,
  "username": "sasi"
}
```

### Signature
Used to verify that the token has not been modified.

---

## JWT Structure

```text
Header.Payload.Signature
```

Example:

```text
xxxxx.yyyyy.zzzzz
```

---

## 5. JSON

JSON (JavaScript Object Notation) is a lightweight format used for storing and exchanging data.

It stores data as key-value pairs.

Example:

```json
{
  "name": "Sasi",
  "role": "Student"
}
```

---

## 6. Hashing

Hashing converts data into a fixed-length value.

- Hashing is a one-way process.
- Original data cannot be retrieved from the hash.
- Commonly used for storing passwords securely.

Example:

```text
Password → Hash Value
```

---

## 7. Encryption and Decryption

### Encryption
Converts readable data into unreadable form.

### Decryption
Converts encrypted data back into readable form.

Used for secure communication and data protection.

---

## 8. JWT Utility Classes

Common methods available in JWT utility classes:

### Generate Token

Creates a new JWT token.

```java
generateToken()
```

### Extract Username

Reads username from the token.

```java
extractUsername()
```

### Validate Token

Checks whether the token is valid or not.

```java
validateToken()
```

Returns:

```java
true  // Valid Token
false // Invalid Token
```

---

## 9. Client-Server Communication

```text
Client ---- JWT Token ----> Server

Server validates token before processing the request.
```

---

## Key Learnings

- JWT is used for authentication and authorization.
- JWT enables secure communication between client and server.
- JWT contains Header, Payload, and Signature.
- Tokens are generated after successful login.
- Passwords should be stored in hashed format.
- Token validation is performed for every protected request.
- JSON is used for exchanging data between client and server.

---

## Outcome

Successfully understood the basics of JWT Authentication, token generation, validation, hashing, and secure client-server communication.

# Day 3 - Git Basics

**Date:** 01 July 2026

---

## 1. Repository Setup

### `git init`
Creates a new empty Git repository in the current folder.

```bash
git init
```

### `git clone`
Copies an existing repository from GitHub to your local system.

```bash
git clone <repository-url>
```

### `git config`
Sets Git username and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

---

## 2. Checking Project Status

### `git status`
Shows the current state of your working directory.

```bash
git status
```

### `git log`
Displays the commit history of the repository.

```bash
git log
```

---

## 3. Saving Changes

### `git add`
Adds files to the staging area.

```bash
git add filename
git add .
```

- `git add filename` → Adds a specific file.
- `git add .` → Adds all changed files.

### `git commit`
Saves staged changes permanently in the local repository.

```bash
git commit -m "Your commit message"
```

---

## 4. Remote Repository Management

### `git remote`
Shows or manages connections to remote repositories.

```bash
git remote -v
```

### `git push`
Uploads local commits to GitHub.

```bash
git push origin main
```

### `git pull`
Downloads and merges changes from GitHub.

```bash
git pull origin main
```

### `git fetch`
Downloads latest changes from GitHub without merging.

```bash
git fetch
```

---

## 5. Branching

### `git branch`
Creates or lists branches.

```bash
git branch
git branch feature-branch
```

### `git checkout`
Switches branches or restores files.

```bash
git checkout feature-branch
```

### `git switch`
Modern command used only for switching branches.

```bash
git switch feature-branch
```

---

## 6. Advanced Git Commands

### `git merge`
Combines changes from one branch into another.

```bash
git merge feature-branch
```

### `git rebase`
Moves commits on top of another branch to maintain a clean history.

```bash
git rebase main
```

### `git cherry-pick`
Copies a specific commit from another branch.

```bash
git cherry-pick <commit-id>
```

---

## 7. Undoing Changes

### `git stash`
Temporarily saves uncommitted changes.

```bash
git stash
```

### `git reset`
Unstages files or removes commits.

```bash
git reset HEAD filename
```

### `git revert`
Creates a new commit that undoes a previous commit.

```bash
git revert <commit-id>
```

---

# Important Comparisons

## `git status` vs `git log`

| Command | Purpose |
|---------|---------|
| `git status` | Shows current changes in the project |
| `git log` | Shows commit history |

---

## `git init` vs `git clone`

| Command | Purpose |
|---------|---------|
| `git init` | Creates a new empty repository |
| `git clone` | Copies an existing repository |

---

## `git checkout` vs `git switch`

| Command | Purpose |
|---------|---------|
| `git checkout` | Switches branches and restores files |
| `git switch` | Only switches branches |

---

# Git Fork (Concept)

A **Fork** creates your own copy of someone else's GitHub repository.

### Uses of Fork
- Contribute to open-source projects.
- Make changes without affecting the original repository.
- Send changes back using a Pull Request.

---

# Key Takeaways

- Git tracks changes in your project.
- GitHub stores your code online.
- Branches allow parallel development.
- `git push` uploads code to GitHub.
- `git pull` downloads code from GitHub.
- `git rebase` helps maintain a clean commit history.
