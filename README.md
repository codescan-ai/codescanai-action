<!-- action-docs-all source="action.yml" project="codescanai/codescanai-action" version="v1.0.0" -->
## CodeScanAI Action

The action wraps the [codescan-ai](https://github.com/codescan-ai/codescan) project that helps scan your codebase for bad coding practices and potential security vulnerabilty.

## Inputs

| name | description | required | default |
| --- | --- | --- | --- |
| `version` | <p>Version of CodeScanAI to install</p> | `false` | `latest` |
| `provider` | <p>AI provider to use</p> | `true` | `""` |
| `model` | <p>AI model from the provider to use</p> | `false` | `""` |
| `directory` | <p>Directory to scan</p> | `false` | `.` |
| `changes_only` | <p>Scans only files with recent changes</p> | `false` | `false` |
| `repo` | <p>GitHub repository</p> | `false` | `""` |
| `pr_number` | <p>Pull request number</p> | `false` | `""` |
| `github_token` | <p>GitHub API token</p> | `false` | `""` |
| `host` | <p>Custom AI server host</p> | `false` | `""` |
| `port` | <p>Custom AI server port</p> | `false` | `""` |
| `token` | <p>Token for authenticating with the custom AI server</p> | `false` | `""` |
| `endpoint` | <p>API endpoint for the custom server</p> | `false` | `/api/v1/scan` |
| `output_file` | <p>Optional output file to store CodeScanAI results</p> | `false` | `""` |


## Runs

This action is a `composite` action.

## Usage

```yaml
- uses: codescanai/codescanai-action@v1.0.0
  with:
    version:
    # Version of CodeScanAI to install
    #
    # Required: false
    # Default: latest

    provider:
    # AI provider to use
    #
    # Required: true
    # Default: ""

    model:
    # AI model from the provider to use
    #
    # Required: false
    # Default: ""

    directory:
    # Directory to scan
    #
    # Required: false
    # Default: .

    changes_only:
    # Scans only files with recent changes
    #
    # Required: false
    # Default: false

    repo:
    # GitHub repository
    #
    # Required: false
    # Default: ""

    pr_number:
    # Pull request number
    #
    # Required: false
    # Default: ""

    github_token:
    # GitHub API token
    #
    # Required: false
    # Default: ""

    host:
    # Custom AI server host
    #
    # Required: false
    # Default: ""

    port:
    # Custom AI server port
    #
    # Required: false
    # Default: ""

    token:
    # Token for authenticating with the custom AI server
    #
    # Required: false
    # Default: ""

    endpoint:
    # API endpoint for the custom server
    #
    # Required: false
    # Default: /api/v1/scan

    output_file:
    # Optional output file to store CodeScanAI results
    #
    # Required: false
    # Default: ""
```
<!-- action-docs-all source="action.yml" project="codescanai/codescanai-action" version="v1.0.0" -->