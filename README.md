# pre-commit-shfmt hook

Warning: I no longer recommend using this method. Use [tflint](https://github.com/terraform-linters/tflint) instead, which provides this in a much more reliable and featureful way. You can hook it directly with a local pre-commit command or through a pre-commit provider.

Single [pre-commit](http://pre-commit.com/) hook which runs **[terraform_unused_vars](https://github.com/ContainerLabs/terraform-unused-vars)** on the terraform project.


An example `.pre-commit-config.yaml`:

```yaml
-   repo: git://github.com/mlemnian/pre-commit-terraform-vars
    sha: master
    hooks:
      -   id: terraform-vars
```

Enjoy the clean code!
