![CrowdStrike Logo (Light)](https://raw.githubusercontent.com/CrowdStrike/.github/main/assets/cs-logo-light-mode.png#gh-light-mode-only)
![CrowdStrike Logo (Dark)](https://raw.githubusercontent.com/CrowdStrike/.github/main/assets/cs-logo-red-dark-mode.png#gh-dark-mode-only)

# CrowdStrike GitHub Organization

This repository provides default community health files, policies, and reusable workflows for the [@CrowdStrike](https://github.com/crowdstrike/) GitHub organization.

These standards help ensure consistency and clarity across all repositories managed by CrowdStrike.

## Branding: Logo Usage

To maintain a unified brand presence, all repositories in the CrowdStrike organization should include the official CrowdStrike logo at the top of their README.md files.

The logos are hosted in the [assets/](https://github.com/CrowdStrike/.github/tree/main/assets) directory of this repository and are configured to support GitHub’s light and dark themes.

### How to Embed

Add the following Markdown snippet at the top of your README.md file ***before*** any headings or content:

```markdown
![CrowdStrike Logo (Light)](https://raw.githubusercontent.com/CrowdStrike/.github/main/assets/cs-logo-light-mode.png#gh-light-mode-only)
![CrowdStrike Logo (Dark)](https://raw.githubusercontent.com/CrowdStrike/.github/main/assets/cs-logo-red-dark-mode.png#gh-dark-mode-only)
```

## Default Community Files

This repository includes a set of default community health files that automatically apply to all repositories within the CrowdStrike organization ***unless those repositories include their own versions*.** If a repository has a local copy of any of these files, that version takes precedence.

### CODE_OF_CONDUCT.md

Establishes expected standards of behavior for contributors and participants in the community. It helps create a respectful and inclusive environment by outlining unacceptable behavior and defining a process for reporting issues.

### CONTRIBUTING.md

Explains whether the project accepts external contributions and, if so, how contributors can collaborate effectively with project maintainers to streamline development. This typically includes:

- How to propose changes via pull requests
- How to file issues or suggest features
- Any coding conventions or review expectations

### SECURITY.md

Provides instructions on how to report potential security vulnerabilities. It ensures that responsible disclosure practices are followed and includes contact details for our security team, who will review and investigate all submitted reports.

### SUPPORT.md

The purpose of this file is to clearly define the level of support users can expect when using a CrowdStrike open source project. By setting expectations upfront, we help users understand whether support will be provided by the community or through formal CrowdStrike support channels. Unless otherwise specified, the default support level is **Community Support**.

Public repositories under CrowdStrike’s GitHub organization follow one of two support models:

- **Community Support:** Users receive assistance primarily through GitHub Issues. The CrowdStrike Support Team is not involved unless the issue is later confirmed to relate to CrowdStrike products or APIs, and a maintainer initiates a formal escalation.

- **Direct Support:** Users may receive assistance either through GitHub Issues or by contacting the CrowdStrike Support Team directly via the standard support process.

> [!TIP]
> The default `SUPPORT.md` is intentionally generic. Maintainers are encouraged to create a customized `SUPPORT.md` in their repositories to provide project-specific guidance and clarify support expectations based on their team’s processes. For inspiration, refer to [FalconPy](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md)

#### Default Support Path is Community

As mentioned above, the default support level for public repositories is **Community Support**. If a repository does not include its own `SUPPORT.md`, it will automatically inherit the Community Support version from this repository.

If you, as a maintainer, determine that your project qualifies for **Direct Support**, you can reference the [Direct Support Template](https://github.com/CrowdStrike/.github/docs/SUPPORT-direct.md) as a starting point. Customize it as needed and commit it directly to your repository to override the default support behavior.

#### Embed Snippet into README.md

While the `SUPPORT.md` file is inherited by default, it’s considered best practice for each repository to include a brief support statement in the README.md. Use the appropriate snippet below and replace the placeholders in curly braces.

#### Community Supported

```markdown
## Support

{REPO NAME} is an open source project designed to {DESCRIPTION}. It is not a formal CrowdStrike produc and as such, it carries no formal support, expressed or implied.

For additional details on the support policy for this project, please see [SUPPORT.md]({PROJECT URL}/SUPPORT.md).
```

#### Direct Supported

```markdown
## Support

{REPO NAME} is a community-driven, open source project designed to {DESCRIPTION}. While not a formal CrowdStrike product, {REPO NAME} is maintained by CrowdStrike and supported in partnership with the open source developer community.

For additional details on the support policy for this project, please see [SUPPORT.md]({PROJECT URL}/SUPPORT.md).
```
