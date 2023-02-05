<div align="center" id="top"> 
  <img src="./.github/app.gif" alt="Gitlab Ce" />

  &#xa0;

  <!-- <a href="https://gitlabce.netlify.app">Demo</a> -->
</div>

<h1 align="center">Gitlab Ce</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/alandolsi/gitlab-ce?color=56BEB8">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/alandolsi/gitlab-ce?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/alandolsi/gitlab-ce?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/alandolsi/gitlab-ce?color=56BEB8">

  <!-- <img alt="Github issues" src="https://img.shields.io/github/issues/alandolsi/gitlab-ce?color=56BEB8" /> -->

  <!-- <img alt="Github forks" src="https://img.shields.io/github/forks/alandolsi/gitlab-ce?color=56BEB8" /> -->

  <!-- <img alt="Github stars" src="https://img.shields.io/github/stars/alandolsi/gitlab-ce?color=56BEB8" /> -->
</p>

<!-- Status -->

<!-- <h4 align="center"> 
	🚧  Gitlab Ce 🚀 Under construction...  🚧
</h4> 

<hr> -->

<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0; 
  <a href="#sparkles-features">Features</a> &#xa0; | &#xa0;
  <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0;
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <a href="#memo-license">License</a> &#xa0; | &#xa0;
  <a href="https://github.com/alandolsi" target="_blank">Author</a>
</p>

<br>

## :dart: About ##

This project is a Gitlab Community Edition (CE) with Docker Compose.

## :sparkles: Features ##

:heavy_check_mark: Gitlab Comunnity Edition;\
:heavy_check_mark:  Gitlab Runner with Docker Compose;

## :rocket: Technologies ##

The following tools were used in this project:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Gitlab](https://gitlab.com/)
- [Gitlab Runner](https://docs.gitlab.com/runner/)

## :white_check_mark: Requirements ##

Before starting :checkered_flag:, you need to have [Git](https://git-scm.com) and [Node](https://nodejs.org/en/) installed.

## :checkered_flag: Starting ##

```bash
# Clone this project
$ git clone https://github.com/alandolsi/gitlab-ce

# Access
$ cd gitlab-ce

# start docker-compose
$ docker-compose up -d

# .env file
# The ip address to listen on
GITLAB_HOST=192.168.*.*
GITLAB_IPV4=192.168.*.*
GITLAB_RUNNER_IPV4=192.168.*.*

# The port to listen on
GITLAB_SSH_PORT=6022
GITLAB_HTTP_PORT=6080
GITLAB_HTTPS_PORT=6443

# Synology NAS Volume
VOLUME=/volume1
GITLAB_HOME=$VOLUME/docker/gitlab-ce
GITLAB_CONFIG=$GITLAB_HOME/config
GITLAB_DATA=$GITLAB_HOME/data
GITLAB_LOGS=$GITLAB_HOME/logs
GITLAB_RUNNER_HOME=$GITLAB_HOME/gitlab-runner
GITLAB_RUNNER_CONFIG=$GITLAB_RUNNER_HOME/config

# smtp settings
SMTP_ENABLED=true
SMTP_PORT=587
SMTP_ADDRESS=mail.***.de
SMTP_USER = webmaster@***.de
SMTP_PASSWORD = ***
SMTP_DOMAIN = ***.de
SMTP_AUTHENTICATION = login

```

## :memo: License ##

This project is under license from MIT. For more details, see the [LICENSE](LICENSE.md) file.


Made with :heart: by <a href="https://github.com/alandolsi" target="_blank">Abdellatif Landolsi</a>

&#xa0;

<a href="#top">Back to top</a>
