# Cli-sh

```
            /$$ /$$                   /$$
           | $$|__/                  | $$
   /$$$$$$$| $$ /$$          /$$$$$$$| $$$$$$$
  /$$_____/| $$| $$ /$$$$$$ /$$_____/| $$__  $$
 | $$      | $$| $$|______/|  $$$$$$ | $$  \ $$
 | $$      | $$| $$         \____  $$| $$  | $$
 |  $$$$$$$| $$| $$         /$$$$$$$/| $$  | $$
  \_______/|__/|__/        |_______/ |__/  |__/

  A minimal, customizable CLI written in shell
              cli-sh.dev | v0.2.0
```

## Usage

1. Copy the `cli` script to your project root and make it executable.

    ```sh
    chmod +x ./cli
    ```

2. Create a `commands` directory in your project.

    ```sh
    mkdir ./commands
    ```

3. Create a script for your command in the `commands` directory.

    ```sh
    echo '#!/bin/sh' > ./commands/hello.sh
    echo 'echo hello world!' >> ./commands/hello.sh
    chmod +x ./commands/hello.sh
    ```
4. Run your command.

    ```sh
    ./cli hello
    ```

## Convention over Configuration

This minimal cli uses a convention over configuration approach. This means that
you can use it without any configuration, but you can also customize it to your
needs.

### Command location

Commands are defined as shell scripts in the `commands` directory.

## Features

### Shell script commands

Use shell scripts as building blocks for your cli commands.

[Example](examples/basic/README.md)

### Hooks

Use hooks to intercept, extend and alter command execution.

[Example](examples/hooks/README.md)
