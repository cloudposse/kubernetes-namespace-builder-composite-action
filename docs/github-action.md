<!-- markdownlint-disable -->

## Inputs

| Name | Description | Default | Required |
|------|-------------|---------|----------|
| app-name | Name of the application |  | false |
| deny-list | Comma seperated list of strings to deny in the namespace name | kube-system,kube-public,default | false |
| flavor | Flavor of naming, either `pr-number`, `branch-name`, or `custom`. Note `name` must be set if using `custom` | pr-number | false |
| name | name for namespace if using flavor `custom`, still prefixed |  | true |
| override-branch-name | Override the branch name, useful for manually helping calculate the branch name | N/A | false |
| override-pr-number | Override the PR number, useful for manually helping calculate the PR number | N/A | false |
| prefix | Prefix for namespace |  | false |
| suffix | Suffix for namespace, appended if still under max length (63 characters) |  | false |


## Outputs

| Name | Description |
|------|-------------|
| kubernetes-namespace | Generated kubernetes namespace |
<!-- markdownlint-restore -->
