#

## GitLab CI

A collection of reusable GitLab CI/CD workflow templates, automation scripts, and developer tools for Python, Go and Docker projects.

## Usage in Your Project

You can include these templates in your own `.gitlab-ci.yml`:

```yaml
include:
  - remote: '$GITLAB_CI_URL'
    rules:
      - if: $GITLAB_CI_URL
  - project: '$GITLAB_CI_PATH'
    ref: '$GITLAB_CI_REF_NAME'
    file: '/ext/.gitlab-ci_py.yml'
    rules:
      - if: $GITLAB_CI_PATH
```

See the files in [`ext/`](ext/) for available templates.

### License

MIT License. See [LICENSE](LICENSE) for details.
