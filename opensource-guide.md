# Open source project guide for Siradel

This guide provides a comprehensive framework for deciding whether to open source a project at Siradel and the steps required to do so successfully.

## Making the decision

Before open-sourcing any project, carefully evaluate it against the following criteria:

**Could this be useful to someone else?**
- Does the project solve a common problem in the industry?
- Would other developers or organizations benefit from this solution?
- Is there potential for community contributions and collaboration?

**Does the project rely on proprietary infrastructure?**
- Check for dependencies on internal Siradel systems or APIs
- Consider publishing only the non-proprietary components
- Identify any proprietary libraries or frameworks that cannot be open sourced
- Ensure the project can function independently without access to internal resources

**Can we commit to maintaining the project, or should it be published as an archive?**
- **Active maintenance**: Regular updates, bug fixes, feature development, community engagement
- **Archive mode**: Published for reference only, with clear documentation that it's no longer maintained
- Consider the team's capacity and long-term availability
- Evaluate the complexity of ongoing maintenance requirements

**Is the project of sufficient quality to represent Siradel publicly?**
- Code follows established best practices and standards
- Comprehensive documentation is available or can be created
- The codebase is clean, well-structured, and maintainable
- No embarrassing or unprofessional content in code or comments

**Remember**: Poor-quality open source projects can damage both our open source reputation and the company's image.

## Implementation process

Once you've decided to proceed with open-sourcing, follow these steps:

### Step 1: Obtain approval
- Discuss the decision with your direct manager.
- Contact the designated open source representatives in the organization.

### Step 2: Repository Setup
- Create a private repository using the template repository, or apply the template to an existing project.
- Follow the steps outlined in the template repository to customize the repository for your project.
- This includes writing a clear README, setting up issue templates, and configuring CI/CD pipelines if applicable.

### Step 3: Project preparation

#### Code cleaning
Thoroughly clean the project of sensitive or inappropriate content:
- Check all commit messages, comments, and documentation for inappropriate language or content
- Remove API keys, passwords, tokens, and other sensitive information
- Consider squashing the entire project history if there's risk of secrets in historical commits

#### License verification
- Create a comprehensive list of all project dependencies.
- Ensure all dependency licenses are compatible with your chosen open source license.
- Maintain clear records of all license requirements and attributions. Some licenses may require specific notices or attributions in the documentation or source files, such as specifying changes for Apache 2.0.

#### Access control setup
- Edit `.github/CODEOWNERS` file to define maintainers (for active projects only).
- Grant admin privileges to the designated siradel-oss team for the repository.

### Step 4: License selection and application
- Choose an appropriate open source license based on project goals and company policy.
- Apply the license to the project with proper copyright notices.
- Ensure license files are prominently placed and correctly formatted.
- Don't forget to also license non-code assets with appropriate licenses if applicable (CC BY 4.0, CC BY-ND 4.0, SIL Open Font License, etc.).

Each file covered by the license should include a header with the appropriate copyright and license information. In addition, the repository should contain the full license text. Tools such as [addlicense](https://github.com/google/addlicense) can help automate this process.

Example using SPDX tags:

```cpp
/**
 * SPDX-FileCopyrightText: Copyright 2026 Siradel
 * SPDX-License-Identifier: MIT
 */
```

The given year should correspond to the year of file creation, if known, or of first publication. When refactoring or moving code around, use your best judgment to determine whether the original year should be retained or updated.

### Step 5: Publication
- Change repository visibility from private to public.
- Clearly indicate whether the project is actively maintained or archived.

## Post-publication steps

### Documentation and promotion
- Add the project to Siradel's list of open source projects, if significant.
    - In this repository, `profile/README.md`.
- Depending on the project's significance, consider internal or external announcements.

### Ongoing Management
For active projects:
- Establish a process for handling issues and pull requests.
- Set expectations for response times and contribution guidelines.
- Plan regular maintenance and update schedules.
- See the [maintenance guidelines](maintenance-guidelines.md) for more details.

For archived projects:
- Clearly mark the repository as archived.
- Provide contact information for questions about the project's history.
- Document the reason for archiving and any recommended alternatives.
