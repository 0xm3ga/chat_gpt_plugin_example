# ChatGPT Plugin Example (by 0xm3ga)

In this repository, I showcase a simple example of how I approach the creation of custom ChatGPT plugins. For this simple example, I am using two endpoints from my `aws_api_example` repository.

The goal here is to demonstrate how a ChatGPT Plugin can enhance ChatGPT's existing UI with your APIs.

## Code qaulity

### Pre-commit Hooks

This project uses pre-commit hooks to maintain code quality. Make sure to install `pre-commit` using `pip install pre-commit` command, and then install git commit hooks using `pre-commit install`. The hooks are set up with the following tools:

- **mypy**: A static type checker for Python, `mypy` catches bugs and prevents crashes by detecting and alerting you of type errors before runtime.

- **isort**: `isort` sorts and organizes Python imports, ensuring they're consistently styled and arranged, which enhances code readability.

- **black**: `black` is a Python code formatter. It enforces a consistent code style across the entire project, freeing developers from having to think about formatting and reducing cognitive load.

- **flake8**: `flake8` is a Python tool for style guide enforcement. It catches logical errors, undefined names, and other potential issues, improving the overall quality and reliability of your code.

Each tool is configured in the `setup.cfg` file at the root of this repository, and the pre-commit hooks are defined in the `.pre-commit-config.yaml`. The hooks automatically check your code each time you make a commit, ensuring that all code adheres to the project's quality standards.
