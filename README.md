# Security Audit Reporter 🔒

[![GitHub release](https://img.shields.io/github/v/release/rkneela0912/security-audit-reporter)](https://github.com/rkneela0912/security-audit-reporter/releases) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Run security audits and post formatted reports

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
    steps:
      - uses: rkneela0912/security-audit-reporter@v1
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
```

## Features

- Automated GitHub Actions workflow
- Easy to configure
- Production-ready
- MIT licensed

## Inputs

| Input | Description | Required |
|-------|-------------|----------|
| `github_token` | GitHub token for API access | ✅ Yes |

## License

[MIT License](LICENSE)

## Support

⭐ Star this repo if you find it helpful!

For issues, [open an issue](https://github.com/rkneela0912/security-audit-reporter/issues).

## 💡 🔒 Catch vulnerabilities early

Make your workflow more efficient with automation!

## 🤝 Contributing

Contributions are welcome! Feel free to:
- 🐛 Report bugs
- 💡 Suggest features
- 🔧 Submit pull requests

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.
