# 🤝 Contributing to Uncle-Factz

First of all, thank you for your interest in contributing to **Uncle-Factz**! 🎉

Uncle-Factz is an open-source AI-powered fact-checking project that combines multi-agent reasoning, evidence retrieval, and blockchain-based tamper-evident records.

The goal of this project is simple:

> **Build a community-driven fact-checking system where people can collectively improve how claims are researched, evaluated, and verified.**

Whether you want to fix a bug, improve the UI, add a new feature, improve the AI prompts, work on the blockchain layer, or improve the documentation — **your contribution is welcome.**

---

## 📌 Before You Start

Please take a moment to:

1. Read this guide.
2. Check the existing [Issues](../../issues).
3. Look for issues labelled:

   * `good first issue`
   * `help wanted`
   * `bug`
   * `enhancement`
4. Avoid working on an issue that someone else is already actively developing.
5. If you are unsure about an idea, open an issue and discuss it before implementing a large change.

For larger changes, discussing the idea first can prevent duplicated work and make sure the proposed feature fits the project's direction.

---

# 🧩 Ways You Can Contribute

You don't need to be an AI or blockchain expert to contribute.

### 🐛 Fix Bugs

Found something that isn't working?

You can:

* Investigate the problem.
* Create an issue if one doesn't already exist.
* Fix the problem.
* Submit a pull request.

---

### ✨ Add Features

You can propose and implement improvements such as:

* New fact-checking capabilities
* Better claim analysis
* Improved evidence retrieval
* Better consensus mechanisms
* New UI features
* Better result visualization
* Blockchain improvements
* Database improvements
* Performance improvements
* Accessibility improvements

---

### 🤖 Improve AI Reasoning

The AI layer is one of the most important parts of Uncle-Factz.

Contributors can experiment with:

* Better prompts
* Better agent instructions
* Improved consensus logic
* Better evidence evaluation
* Improved uncertainty handling
* Source-quality evaluation
* Reducing hallucinations
* Better disagreement detection
* Better explanations of verdicts

When changing AI behaviour, please explain **why the change improves the system**.

---

### ⛓️ Improve the Blockchain Layer

The project currently uses Solidity and a public testnet to store tamper-evident verdict information.

Possible contributions include:

* Improving smart contracts
* Improving contract security
* Better event structures
* On-chain voting
* Reputation systems
* Better verification
* Gas optimization
* Blockchain integration improvements

**Important:** Smart-contract changes should be reviewed carefully because mistakes can have serious consequences.

---

### 🎨 Improve the Frontend

The frontend uses React, Vite, and Tailwind.

You can contribute by improving:

* UI/UX
* Responsive design
* Accessibility
* Loading states
* Error handling
* Claim submission experience
* Verdict visualization
* Evidence presentation
* Blockchain verification interfaces

---

### 🐍 Improve the Backend

The backend uses Python and FastAPI.

Possible contributions include:

* API improvements
* Better error handling
* Performance improvements
* Database improvements
* AI pipeline improvements
* Better validation
* Testing
* API documentation

---

### 📚 Improve Documentation

Documentation contributions are extremely valuable.

You can improve:

* README
* Installation instructions
* API documentation
* Architecture documentation
* Developer guides
* Examples
* Comments
* Tutorials

Even fixing a typo is a valid contribution!

---

# 🛠️ Setting Up the Project

## 1. Fork the Repository

Fork the repository to your GitHub account.

Then clone your fork:

```bash
git clone https://github.com/YOUR-USERNAME/Uncle-factz.git
cd Uncle-factz
```

---

## 2. Create a Branch

Don't work directly on `main`.

Create a separate branch:

```bash
git checkout -b feature/your-feature-name
```

Examples:

```bash
git checkout -b feature/improve-verdict-ui
```

```bash
git checkout -b fix/api-error-handling
```

```bash
git checkout -b docs/update-installation
```

---

# 🐍 Backend Setup

Create a virtual environment:

```bash
python -m venv venv
```

Activate it.

### Linux/macOS

```bash
source venv/bin/activate
```

### Windows

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create your local environment file using the project's `.env.example`.

**Never commit your ****`.env`**** file or API keys.**

Start the backend:

```bash
uvicorn main:app --reload
```

---

# ⚛️ Frontend Setup

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

---

# ⛓️ Smart Contract Development

The blockchain components are located in the `contracts` directory.

Before modifying smart contracts:

1. Understand the existing contract.
2. Test your changes locally.
3. Check for security implications.
4. Explain the purpose of the change in your pull request.

Do not deploy experimental contracts to a public network without understanding what the deployment does.

---

# 🌿 Branch Naming

Please use descriptive branch names.

### Features

```text
feature/feature-name
```

### Bug fixes

```text
fix/bug-name
```

### Documentation

```text
docs/documentation-name
```

### Refactoring

```text
refactor/component-name
```

### Tests

```text
test/component-name
```

Examples:

```text
feature/agent-confidence-score
fix/tavily-error
docs/setup-guide
refactor/consensus-engine
test/verdict-api
```

---

# 💬 Issues

Before opening an issue, search existing issues to make sure the problem or feature hasn't already been discussed.

## 🐛 Bug Reports

A good bug report should include:

* What happened?
* What did you expect to happen?
* Steps to reproduce the issue
* Operating system
* Relevant error messages
* Relevant screenshots/logs
* Any other useful information

### Example

```text
### Bug
The verdict page stays on the loading screen.

### Steps to reproduce
1. Start the backend.
2. Start the frontend.
3. Submit a claim.
4. Open the verdict page.

### Expected behaviour
The verdict should appear after processing.

### Actual behaviour
The page remains on the loading screen.

### Environment
OS: Ubuntu 24.04
Browser: Chrome
```

---

# 💡 Feature Requests

When proposing a feature, explain:

1. What problem does it solve?
2. How would it work?
3. Why would it improve Uncle-Factz?
4. Are there alternative approaches?
5. Is this something you are willing to implement?

---

# 🔀 Pull Request Process

When your work is ready:

### 1. Check your changes

```bash
git status
```

Review your changes carefully.

### 2. Commit your changes

Use a clear commit message:

```bash
git add .
git commit -m "Improve verdict confidence display"
```

Try to keep commits focused on one logical change.

### 3. Push your branch

```bash
git push origin feature/your-feature-name
```

### 4. Open a Pull Request

Open a PR from your branch to the repository's `main` branch.

Your PR should clearly explain:

* What you changed
* Why you changed it
* How you tested it
* Related issue number, if applicable

Example:

```text
Closes #12
```

---

# 📝 Pull Request Guidelines

Before submitting a PR, make sure:

* [ ] The code works locally.
* [ ] Existing functionality is not unnecessarily broken.
* [ ] New functionality has been tested.
* [ ] No API keys or secrets are committed.
* [ ] The code follows the existing project structure.
* [ ] Documentation has been updated if necessary.
* [ ] The PR has a clear title.
* [ ] The PR description explains the change.
* [ ] Screenshots are included for significant UI changes.
* [ ] Blockchain changes have been tested carefully.

---

# 🧪 Testing

Before submitting your PR, test the parts of the application affected by your changes.

At minimum:

```text
Frontend → Does the UI work?
Backend  → Does the API work?
AI       → Does the reasoning pipeline behave correctly?
Blockchain → Does the contract behave as expected?
```

If you introduce a new feature, please consider adding tests where appropriate.

---

# 🔐 Security

**Never commit:**

* API keys
* Private keys
* Passwords
* Tokens
* `.env` files
* Wallet credentials
* Other secrets

If you discover a security vulnerability, **do not publicly post sensitive exploit details in an issue.**

Instead, contact the project maintainer privately so the issue can be investigated responsibly.

---

# 🤖 AI Contribution Guidelines

Because Uncle-Factz is an AI-assisted fact-checking project, changes to AI prompts, agents, evidence retrieval, and consensus logic should be made carefully.

When modifying AI behaviour, please consider:

### Evidence

Does the system rely on verifiable sources?

### Uncertainty

Does the system admit when there isn't enough evidence?

### Hallucination

Could the change cause the model to confidently invent information?

### Bias

Could the change systematically favour one type of claim or source?

### Consensus

Does the change improve genuine disagreement handling rather than simply forcing agreement?

### Transparency

Can a user understand why the system reached its conclusion?

A fact-checking system should prefer:

> **"There isn't enough evidence to determine this."**

over an unsupported confident answer.

---

# ⛓️ Blockchain Contribution Guidelines

The blockchain layer is intended to provide **tamper-evident records**, not automatically prove that a verdict is objectively correct.

When contributing to this part of the project, keep this distinction in mind.

For example:

```text
Blockchain proves:
"The stored verdict record has not been silently modified."

Blockchain does NOT automatically prove:
"The verdict itself is correct."
```

Contributions should preserve this distinction.

---

# 🎯 Good First Contributions

New contributors can start with smaller improvements such as:

* Fixing documentation
* Improving error messages
* Improving UI components
* Adding loading states
* Improving accessibility
* Adding tests
* Fixing small bugs
* Improving API validation
* Adding examples
* Improving README documentation

Look for issues labelled:

```text
good first issue
help wanted
```

---

# 🌍 Community Philosophy

Uncle-Factz is intended to be improved **collectively**.

You don't need to be the original developer to make the project better.

We encourage contributors to:

* Share ideas
* Ask questions
* Review pull requests
* Improve existing implementations
* Challenge assumptions
* Experiment with new approaches
* Help other contributors
* Improve documentation

Constructive disagreement is welcome.

The goal isn't to prove that one contributor is right.

The goal is to make the project better.

---

# ❤️ Recognition

Every meaningful contribution matters.

Contributors may be recognized through:

* GitHub contributor history
* Release notes
* Project acknowledgements
* Documentation credits

Thank you for helping build Uncle-Factz! 🚀

---

## 📜 License

By contributing to this repository, you agree that your contributions will be licensed under the same license that applies to this project.

If you have questions about licensing or contributions, please open an issue for discussion.

---

## 🚀 Ready to Contribute?

1. Fork the repository.
2. Clone your fork.
3. Create a branch.
4. Make your changes.
5. Test your changes.
6. Commit your work.
7. Push your branch.
8. Open a Pull Request.
9. Participate in the review.
10. Help make Uncle-Factz better.

**Welcome to the family. 👴🤖**

Someone has to check before it gets forwarded.
