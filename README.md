# My Git Puller and Builder

A Go-based tool that listens for Git webhooks, pulls the repository, and executes build steps defined in a YAML file.

## Installation

1. Download the latest release from [here](https://github.com/your-username/your-repo/releases/latest).
2. Extract the binary: `tar -xzf my-git-builder_v1.0.0_linux_arm64.tar.gz`
3. Make the binary executable: `chmod +x my-git-builder`

## Usage

1. Create a `build.yaml` file in the root of your project with the desired build steps. For example:

   ```yaml
   steps:
     - npm install
     - npm run build
     - pm2 restart my-app
