# github-actions-workflows #

[![GitHub Build Status](https://github.com/cisagov/github-actions-workflows/workflows/build/badge.svg)](https://github.com/cisagov/github-actions-workflows/actions)

This repository stores [reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
for use in our organization's GitHub Actions workflows.

## Workflows available ##

- [common-lint.yml](#common-lintyml)

### [common-lint.yml](.github/workflows/common-lint.yml) ##

The standard linting workflow for our projects.

#### Inputs ####

| Name | Description | Type | Default | Required |
| ---- | ----------- | ---- | ------- | -------- |
| go-version | The version of [Go](https://github.com/golang/go) to use in the workflow. | `string` | `"1.19"` | no |
| packer-version | The version of [Packer](https://github.com/hashicorp/packer) to use instead of what is provided by [cisagov/setup-env-github-action]. | `string` | `""` | no |
| python-version | The version of [Python](https://github.com/python/cpython) to use in the workflow. | `string` | `"3.10"` | no |
| run-tmate | Start a workflow debugging session with [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate). | `boolean` | `false` | no |
| shfmt-version | The version of [shfmt](https://github.com/mvdan/sh#shfmt) to use instead of what is provided by [cisagov/setup-env-github-action]. | `string` | `""` | no |
| terraform-version | The version of [Terraform](https://github.com/hashicorp/terraform) to use instead of what is provided by [cisagov/setup-env-github-action]. | `string` | `""` | no |
| terraform-docs-version | The version of [terraform-docs](https://github.com/terraform-docs/terraform-docs) to use instead of what is provided by [cisagov/setup-env-github-action]. | `string` | `""` | no |

#### Secrets ####

Workflow accepts no secrets.

<!--
| Name | Description | Required |
| ---- | ----------- | -------- |
| Secret name | Secret description | Is it required? |
-->

## Contributing ##

We welcome contributions!  Please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for
details.

## License ##

This project is in the worldwide [public domain](LICENSE).

This project is in the public domain within the United States, and
copyright and related rights in the work worldwide are waived through
the [CC0 1.0 Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0
dedication. By submitting a pull request, you are agreeing to comply
with this waiver of copyright interest.

[cisagov/setup-env-github-action]: https://github.com/cisagov/setup-env-github-action
