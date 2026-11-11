# Go app template

Template to create Go application (e.g. Discord Bot, API Server etc.)

## Pre-requirements

- [Go1.27+](https://go.dev/)
- [mise](https://mise.jdx.dev/)
- Container Runtime (Docker / OrbStack / colima etc.)

## How to setup

### Clone by gonew

1. Install [gonew](https://pkg.go.dev/golang.org/x/tools/cmd/gonew) command

   ```bash
   go install golang.org/x/tools/cmd/gonew@latest
   ```

1. Run gonew

   ```bash
   gonew github.com/aqyuki/go-app-template <your.domain>/<project-name>
   ```

1. Move to project directory and initialize Git

   ```bash
   cd <project-directory>
   git init
   ```

1. Install dependencies

   ```bash
   mise install
   ```

### Clone by manualy

1. Clone this repository

   ```bash
   git clone https://github.com/aqyuki/go-app-template go-app-template
   ```

1. Rename directory

   ```bash
   mv go-app-template <your-project-name>
   ```

1. Move to project directory and change import path

   ```bash
   cd <your-project-directory>
   rm -rf .git
   git init
   go mod edit -module <your.domain>/<project-name>
   ```

1. Install dependencies

   ```bash
   mise install
   ```
