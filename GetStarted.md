---
id: VSCode-Remote-Containers
title: VS Code Remote - Containers
sidebar_position: 1
sidebar_label: Getting Started
tags:
  - VS Code
  - Containers
  - Docker
  - Remote
  - Development
---

I have been playing around for a while with a number of solutions for my development environment. At present, I'm fairly committed to VS Code, and for a while I was fully dedicated to my MacBook Pro as my daily driver. As things have progressed and I began to build out a dedicated office space, I included in my setup, a pretty hefty Windows / Linux duel boot machine. It's a joy to use and when I begin programming on this machine, I love it. Then, I'll be called away to finish some household task, and invariably I'll be multi-tasking household / dad duties and popping over to my MacBook Pro to continue where I left off. It's a good computer, but I really like the option of working on the go, in my living room or on the deck outside, or to sit at my desk in a different environment to mix things up. It boosts my productivity and keeps me fresh. I have also been slowly shifting my daily driver from MacOS to Linux, and not having my codebase present and up to date on whichever machine I'm using is a real pain.

So, here I sit, kids all tucked into bed, and me in my office thinking, "I could just write a bit on this desktop and then merge what I've worked on with what was started on the laptop. It's no big deal!" -narrators voice: It's always a big deal and inevitably something gets lost- So, I fuss with the 37 cables to get the MacBook Pro set up on my desk and then look at my sweet desktop and think, "Sorry buddy, I kind of just need to use this laptop here to pick up from where I left off." What a waste of a beautiful machine.

If you've ever been in this situation, you'll know the pain of having to switch between machines, and the inevitable "I forgot to push my changes" moment, the moment where you smash your head on the desk trying to fish that cable that slipped of your desk so you can jam it into the laptop. These moments that remind you of the frailty of your existence and the fragility of your workflow. Enter VS Code Remote - Containers. This is not the only solution to this problem. I've half-heartedly attempted a variety of others. I have even deployed a self-hosted VS-Code based instance on my home server but as it turns out, VS Code Remote - Containers powered by Docker is likely the best solution for me. So, today I will finally get this set up and running in full - no false starts, no half-hearted attempts, no excuses. Let's get this done.

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop)
- [VS Code](https://code.visualstudio.com/)
- [VS Code Remote - Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [Git](https://git-scm.com/)

## Getting Started

You can follow the Microsoft Learn guide [here](https://learn.microsoft.com/en-us/training/modules/use-docker-container-dev-env-vs-code/2-exercise-prepare-project) if you'd like, as this is the primary source for this guide, however, their guide uses a Python project and I will be using a Node.js (Docusaurus / React) project. I will be using the same project structure as the guide, but with a Node.js project instead.

For this reason, I will presume that you already have a project that you'd like to containerize. If you don't have a project, you can clone the project I will be using from

### Step 1

1. Open your project in VS Code.

2. Ensure that you have the Remote - Containers extension installed.
