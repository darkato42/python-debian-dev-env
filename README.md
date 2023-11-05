# Python Development Environment

This repository contains a basic configuration for a Python development environment using Visual Studio Code Dev Containers.

## Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/)
- [Docker](https://www.docker.com/products/docker-desktop)
- VS Code Extensions:
  - [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Getting Started

To get started with the Python development environment, follow these steps:

1. Clone this repository to your local machine.
    ```sh
    git clone <repository-url>
    ```
2. Open the cloned repository folder in Visual Studio Code.
3. When prompted by VS Code, click on `Reopen in Container`. This will start the process of building your Docker container based on the configuration specified in `.devcontainer/devcontainer.json`.
   - Alternatively, you can open the command palette (`Ctrl+Shift+P` or `Cmd+Shift+P` on Mac) and select `Remote-Containers: Reopen in Container`.
4. After the container is built and started, VS Code will attach to it and open the `/app` workspace folder.

Now, you're ready to start developing with Python in this containerized environment. Any changes you make will be reflected within the container.

## Verifying the Setup

To verify that the development environment is set up correctly, you can run the following commands in the VS Code terminal:

```sh
python --version
cat /etc/os-release
```

## Files

- `hello-world.py`: A simple Python script that prints "Hello, World!" to the console.
- `.devcontainer/devcontainer.json`: The configuration file that VS Code uses to set up your development container.

Feel free to modify the `hello-world.py` script to test the development environment and Python setup.

## Support

If you encounter any issues with the setup, please ensure you have the latest versions of Docker, Visual Studio Code, and the Remote - Containers extension installed. For further assistance, consult the [VS Code documentation on Dev Containers](https://code.visualstudio.com/docs/remote/containers).
