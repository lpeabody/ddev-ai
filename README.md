[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/lpeabody/ddev-ai/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/lpeabody/ddev-ai/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/lpeabody/ddev-ai)](https://github.com/lpeabody/ddev-ai/commits)
[![release](https://img.shields.io/github/v/release/lpeabody/ddev-ai)](https://github.com/lpeabody/ddev-ai/releases/latest)

# DDEV Ai

## Overview

This add-on integrates Ai into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get lpeabody/ddev-ai
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Ai |
| `ddev logs -s ai` | Check Ai logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.ai --ai-docker-image="busybox:stable"
ddev add-on get lpeabody/ddev-ai
ddev restart
```

Make sure to commit the `.ddev/.env.ai` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `AI_DOCKER_IMAGE` | `--ai-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@lpeabody](https://github.com/lpeabody)**
