# Contributing Guidelines

Thanks for your interest in contributing to **tiny-fmod**. This is a small personal project I maintain, so I keep the contribution process intentionally lightweight and focused. Following the guidelines below helps ensure reviews stay quick and changes remain safe and intentional.

## Important Restrictions

Before contributing, please understand these limitations:

### Intellectual Property

- Only submit code you personally wrote or have explicit permission to contribute.
- Do not submit decompiled or reverse-engineered code from any source.
- If you want to integrate third-party code, open an issue first to discuss it.
- All contributions are distributed under the MIT License.

### What Will Not Be Accepted

- Decompiled or reverse-engineered code
- Large PRs that touch unrelated areas
- Style-only changes with no functional benefit
- Breaking API changes without prior discussion

Keep changes **intentional**, **scoped**, and **reviewable**.

## Getting Started Locally

Setting up your development environment is straightforward:

```bash
git clone https://github.com/AristurtleDev/tiny-fmod.git
cd tiny-fmod
dotnet restore
dotnet build
```

### Branching

All work should create a new branch based on the `main` branch. When submitting a PR, target the changes to be merged back into `main`.

## Ways to Contribute

### Bug Reports and Fixes

Found a bug? First check our [existing issues](https://github.com/AristurtleDev/tiny-fmod/issues) to avoid duplicates. When creating a bug report, provide a clear description of the problem, step-by-step reproduction instructions, expected versus actual behavior, configuration details, and error messages when available. Include a minimal code example or link to a reproduction repository when possible. Text is preferred over screenshots for searchability.

### Feature Requests and Implementation

Since this is a small wrapper library, features are intentionally limited.  Before implementing any new feature, submit a [feature request](https://github.com/AristurtleDev/tiny-fmod/issues/new/choose) explaining what problem the feature solves.

### Documentation and Examples

Help other developers by improving API documentation, creating usage examples, writing tutorials or guides, and updating the wiki. Clear documentation is just as valuable as code contributions.

## Code Quality and Standards

The codebase maintains the following consistent standards to ensure it remains readable, maintainable, and performant:

### Architecture and Design

Follow existing patterns and conventions, other developers should be able to build on your work. Prefer composition over inheritance where appropriate, keep dependencies minimal and well-justified, and ensure new features integrate well with existing components. Don't break existing APIs without strong justification, and consider deprecation paths for necessary breaking changes.

### Vender Code

Files in the `/FMOD/FMOD` directory are upstream wrapper code. Treat these as **vendor code*8.  Do no modify them unless there is a verified bug or the change is required for compatibility.  If changes must be mad here, the reasoning should always be clearly documented.

## Pull Request Process

### Before You Submit

Fork the repository and create a branch from `main` with a descriptive name. Make focused commits with clear, descriptive messages that explain what changed and why.

### The Pull Request

Complete the PR checklist. **I will not review incomplete submissions**. Verify no overlapping PRs exist, follow the contribution guidelines and code of conduct, and write a descriptive title that summarizes your changes. Fill out the PR template with a clear description of the purpose and problem solved, links to related issues (use "closes #123" to auto-close issues), and a high-level overview of technical changes.

Keep PRs reasonably sized and focused on a single concern. Include tests that verify your changes work correctly, update documentation for any API changes.  Be patient during review, we're all volunteers with varying availability.

## Code Review Process

Understanding our review process helps set proper expectations and ensures smoother collaboration.

### What to Expect

I aim to acknowledge new PRs within 3-5 business days, though initial response times may vary during holidays or when I have competing priorities. Simple fixes typically get reviewed within 1-2 weeks, while complex features may take longer. Other community members may provide feedback before maintainer review.

### Review Focus Areas

Reviewing evaluates contributions across several dimensions. Code quality includes adherence to established coding standards, proper error handling, performance considerations, and clear, self-documenting code.

Documentation requirements include XML documentation for public APIs, updated README or wiki pages for new features, clear commit messages and PR descriptions, and migration notes for breaking changes.

### During Review

Address all reviewer comments, even if just to explain your reasoning. Make requested changes in new commits rather than force-pushing during review, ask questions if feedback isn't clear, and be open to alternative approaches suggested by reviewers. My reviews focus on the code rather than the person, provide constructive feedback with explanations, and may offer mentoring for newer contributors.

## Licensing

**tiny-fmod** is under the [MIT License](https://opensource.org/licenses/MIT) unless a portion of code is explicitly stated elsewhere. See the [LICENSE](LICENSE) for more details. Third-party libraries used by **tiny-fmod** are under their own licenses, we always seek permission from the original author of those libraries.. Please refer to those libraries for details on the license they use.

We accept contributions in "good faith" that it isn't bound to a conflicting license. By submitting a PR you agree to distribute your work under the **tiny-fmod** Extended license and copyright.


---

Thank you for contributing!

💖 Chris Whitley (Aristurtle 🐢)
