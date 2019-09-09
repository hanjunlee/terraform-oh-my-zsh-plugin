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

### Expanding ZSH prompt with current Terraform workspace name

If you want to get current Terraform workspace name in your ZSH prompt open
your .zsh-theme file and in a chosen place insert:

```shell
PROMPT=$'%{$fg[white]%}$(tf_prompt_info)%{$reset_color%} '
```
