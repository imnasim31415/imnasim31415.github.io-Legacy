---
title: Getting Started
description: >-
  Get started with Chirpy basics in this comprehensive overview.
  You will learn how to install, configure, and use your first Chirpy-based website, as well as deploy it to a web server.
author: cotes
date: 2019-08-09 20:55:00 +0800
categories: [Blogging, Tutorial]
tags: [getting started]
---

## Creating a Site Repository

When creating your site repository, you have two options depending on your needs:

### Option 1. Using the Starter (Recommended)

This approach simplifies upgrades, isolates unnecessary files, and is perfect for users who want to focus on writing with minimal configuration.


### Option 2. Forking the Theme

This approach is convenient for modifying features or UI design, but presents challenges during upgrades. So don't try this unless you are familiar with Jekyll and plan to heavily modify this theme.


## Setting up the Environment

Once your repository is created, it's time to set up your development environment. There are two primary methods:

### Using Dev Containers (Recommended for Windows)

Dev Containers offer an isolated environment using Docker, which prevents conflicts with your system and ensures all dependencies are managed within the container.

**Steps**:

1. Install Docker:
   - On Windows/macOS, install [Docker Desktop][docker-desktop].
   - On Linux, install [Docker Engine][docker-engine].
2. Install [VS Code][vscode] and the [Dev Containers extension][dev-containers].
3. Clone your repository:
   - For Docker Desktop: Start VS Code and [clone your repo in a container volume][dc-clone-in-vol].
   - For Docker Engine: Clone your repo locally, then [open it in a container][dc-open-in-container] via VS Code.
4. Wait for the Dev Containers setup to complete.

### Setting up Natively (Recommended for Unix-like OS)

For Unix-like systems, you can set up the environment natively for optimal performance, though you can also use Dev Containers as an alternative.





### Customizing the Stylesheet


### Customizing Static Assets


## Deployment



Now you can choose _ONE_ of the following methods to deploy your Jekyll site.

### Deploy Using Github Actions

Prepare the following:

- If you're on the GitHub Free plan, keep your site repository public.

Next, configure the _Pages_ service:

1. Go to your

2. Push any commits to GitHub to trigger the _Actions_ workflow. In the _Actions_ tab of your repository, you should see the workflow _Build and Deploy_ running. Once the build is complete and successful, the site will be deployed automatically.

You can now visit the URL provided by GitHub to access your site.

### Manual Build and Deployment

For self-hosted servers, you will need to build the site on your local machine and then upload the site files to the server.

Navigate to the root of the source project, and build your site with the following command:
