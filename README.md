# Security Audit Reporter 🔒

[![GitHub release](https://img.shields.io/github/v/release/rkneela0912/security-audit-reporter)](https://github.com/rkneela0912/security-audit-reporter/releases) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Run security audits and post formatted reports on pull requests

## Quick Start

```yaml
name: Security Audit Reporter
on:
  pull_request:
    types: [opened, synchronize]

jobs:
  run:
    runs-on: ubuntu-latest
    permissions:
      pull-requests: write
      issues: write
      contents: read
    
    steps:
      - uses: rkneela0912/security-audit-reporter@v1
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
```

## Features

- Automated workflow integration
- Easy configuration
- Comprehensive documentation
- MIT licensed

## Inputs

| Input | Description | Required |
|-------|-------------|----------|
| `github_token` | GitHub token for API access | ✅ Yes |

## License

[MIT License](LICENSE)

## Support

⭐ Star this repo if you find it helpful!

For issues or questions, [open an issue](https://github.com/rkneela0912/security-audit-reporter/issues).
