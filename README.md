## Terraform oh-my-zsh plugin

Plugin for Terraform, more extended than original oh-my-zsh plugin, a tool from Hashicorp for managing infrastructure safely and efficiently.

Current as of Terraform v0.11.7

### Requirements

 * [Terraform](https://terraform.io/)

### Usage

clone this repository into custom directory with name `terraform`:
```shell
git clone https://github.com/hanjunlee/terragrunt-oh-my-zsh-plugin ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/terraform
```

add `terraform` to the plugins array of your `~/.zshrc` file:
```shell
plugins=(... terraform)
```

 * Type `terraform` into your prompt and hit `TAB` to see available completion options

### Features

- When you type at the `-target` option it show the list of resources.
```shell
$ terraform plan -target 

foo.bar bar.baz ...
```
