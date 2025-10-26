# Dependency Update Summarizer 📦

[![GitHub release](https://img.shields.io/github/v/release/rkneela0912/dependency-update-summarizer)](https://github.com/rkneela0912/dependency-update-summarizer/releases) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Summarize Dependabot PRs with breaking changes

## Quick Start

```yaml
name: Dependency Update Summarizer
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
      - uses: rkneela0912/dependency-update-summarizer@v1
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

For issues, [open an issue](https://github.com/rkneela0912/dependency-update-summarizer/issues).

## 💡 📦 Smart dependency updates

Make your workflow more efficient with automation!

## 🤝 Contributing

Contributions are welcome! Feel free to:
- 🐛 Report bugs
- 💡 Suggest features
- 🔧 Submit pull requests

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.
