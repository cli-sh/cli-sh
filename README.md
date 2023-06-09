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
              cli-sh.dev | v0.1.0
```

## Usage

1. Copy the `cli` script to your project root and make it executable.

    ```sh
    chmod +x ./cli
    ```

2. Create a `scripts` directory in your project.

    ```sh
    mkdir ./scripts
    ```

3. Create a script for your command in the `scripts` directory.

    ```sh
    echo '#!/bin/sh' > ./scripts/hello.sh
    echo 'echo hello world!' >> ./scripts/hello.sh
    chmod +x ./scripts/hello.sh
    ```
4. Run your command.

    ```sh
    ./cli hello
    ```

## Examples

- [Basic example](examples/basic/README.md)

## Convention over Configuration

This minimal cli uses a convention over configuration approach. This means that
you can use it without any configuration, but you can also customize it to your
needs.

### Command location

Commands are defined as shell scripts in the `scripts` directory.
