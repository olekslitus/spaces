# spaces
Use containers for Development Environment.


## Interface

### CLI

#### Example
```
spaces new dev --distro ubuntu:20.04 
spaces enter dev
sudo apt install cmake
spaces update dev
```

#### Create new space
```
# Defaults to use the host OS as base for the container.
spaces new dev

# You can create a copy of the space.
spaces new dev --copy old-dev
```


### GNOME Shell Extensions
Should look something like [Places Status Indicator](https://extensions.gnome.org/extension/8/places-status-indicator/).

## Concerns
- Tools
  - Build Tools
  - Test Tools
  - Debug Tools
  - Utility Tools
    - Log Acquire and Analysis
    - Database Access
- SSH Config
- Tool Configs
  - IDE config
    - vim config
    - CLion config
    - VSCode config
    - Eclipse config
  - Bash Config
  - Azure CLI config
- Git Credentials
- Repositories
- Setup has to be reguraly synced and updated across a team without breaking work

## Anlogous Things
- [Microsoft Edge Workspaces](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-workspaces)
- [Chrome Workspaces Extenssion](https://chromewebstore.google.com/detail/workspaces/hpljjefgmnkloakbfckghmlapghabgfa)

## Existing Tools
- Containers
  - [Docker](https://docs.docker.com/engine/)
  - [Podman](https://podman.io/)
  - [Docker Compose](https://docs.docker.com/compose/)
  - [Development Containers](https://containers.dev/)
  - [Toolbx](https://containertoolbx.org/)
  - [Distrobox](https://distrobox.it/)
- Virtual Machines
  - [Virtual Box](https://www.virtualbox.org/)
- [Nix](https://nixos.org/)
  - [mkShell](https://ryantm.github.io/nixpkgs/builders/special/mkshell/)
  - [Devenv](https://devenv.sh/)
    - [Use custom packages in devenv](https://devenv.sh/guides/using-with-flakes/#modifying-your-flakenix-file)
  - [devbox](https://www.jetify.com/devbox)
  - [Flox](https://flox.dev/)
  - [Devshell](https://numtide.github.io/devshell/)
- Remote
  - [GitHub Codespaces](https://github.com/features/codespaces)
  - [Gitpod](https://www.gitpod.io/)
- Tools
  - [Vagrant](https://www.vagrantup.com/)
  - [Direnv](https://direnv.net/)
  - [asdf](https://asdf-vm.com/)
