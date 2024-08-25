<!-- This README is based on the template on the Riverside Valley helpdesk repo (https://github.com/RiversideValley/.github). 
Here are variables to replace:
{repo name pretty}
{repo description noemoji}
{repo name}
{repo platform}
{repo platform colour}
{repo lang}
{repo lang colour}
{mpn name}
{mpn id}
{screenshot one}
{screenshot two}
{screenshot three}
{repo copyright}

Special::CODEBASE
Special::BUILDING
-->

# 🖼️ {repo name pretty}

#### {repo description noemoji}

<p align="center">
  <a title="GitHub Releases" target="_blank" href="https://github.com/RiversideValley/{repo name}">
    <img align="left" src="https://img.shields.io/github/v/release/RiversideValley/{repo name}?include_prereleases" alt="Release" />
  </a>
  <a title="Repository Size" target="_blank" href="https://github.com/RiversideValley/{repo name}/activity">
    <img align="left" src="https://img.shields.io/github/repo-size/RiversideValley/{repo name}?color=%23cc0000" alt="Size" />
  </a>
  <a title="Platform" target="_blank" href="https://github.com/topics/{repo platform}">
    <img align="left" src="https://img.shields.io/badge/platform-{repo platform}-{repo platform colour}" alt="Platform" />
  </a>
  <a title="Language" target="_blank" href="https://github.com/RiversideValley/{repo name}/search?l=c%23">
    <img align="left" src="https://img.shields.io/badge/language-{repo lang}-{repo lang colour}" alt="Language" />
  </a>
</p>

<br/>

---

## 🎁 Installation

<p>
  <a title="Microsoft Store" target="_blank" href="https://apps.microsoft.com/store/detail/{mpn name}/{mpn id}">
  <a style="text-decoration:none" href="https://apps.microsoft.com/detail/{mpn id}?launch=true&mode=mini">
    <picture>
      <source media="(prefers-color-scheme: light)" srcset="https://get.microsoft.com/images/en-us%20dark.svg" width="200" />
      <img src="https://get.microsoft.com/images/en-us%20light.svg" width="200" />
    </picture></a>
  <a title="GitHub" href="https://github.com/RiversideValley/{repo name}/releases/latest">
    <img src="https://user-images.githubusercontent.com/74561130/160255105-5e32f911-574f-4cc4-b90b-8769099086e4.png" width="157" alt="Get it from GitHub" />
  </a>
<p/>

### 🔨 Building from source

This is the best way to ensure you're on the most recent update in the code stream. However, this is experimental and certain functions may not work as intended.
See [this section](#-building-the-code).

### 📸 Screenshots

{screenshot one}|{screenshot two}|{screenshot three}
---|---|---
[![App screenshot](https://user-images.githubusercontent.com/71598437/212673147-54e79843-76aa-44ff-9db3-60b025334f07.png)](https://github.com/RiversideValley/Emerald)|[![App screenshot](https://user-images.githubusercontent.com/71598437/212673147-54e79843-76aa-44ff-9db3-60b025334f07.png)](https://github.com/RiversideValley/Emerald)|[![App screenshot](https://user-images.githubusercontent.com/71598437/212673147-54e79843-76aa-44ff-9db3-60b025334f07.png)](https://github.com/RiversideValley/Emerald)

## 🦜 Contributing & Feedback

There are multiple ways to participate in the community:

- Upvote popular feature requests
- [Submit a new feature](https://github.com/RiversideValley/{repo name}/pulls)
- [File bugs and feature requests](https://github.com/RiversideValley/{repo name}/issues/new/choose).
- Review source [code changes](https://github.com/RiversideValley/{repo name}/commits)

### 🏗️ Codebase Structure

<!-- Change as appropriate to the app -->

```
.
├──Emerald.App                       // Emerald app code and packager
|  ├──Emerald.App                    // Emerald app code (such as code related to UI but not Minecraft)
|  └──Emerald.App.Package            // Package code for generating an uploadable MSIX bundle.
├──Emerald.Core                      // Emerald core code (such as code related to launching and modifying Minecraft
└──Emerald.CoreX                     // Emerald core code for the ability to run different Minecraft installation profiles and mods.
```

## 🔨 Building the Code

### 1️⃣ Prerequisites

Ensure you have following components:

<!-- Change as appropriate to the app -->

- [Git](https://git-scm.com/)
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) with following individual components:
  - Universal Windows Platform Software Development Kit
  - .NET 7
  - Windows App Software Development Kit
  - Windows 11 SDK
- [Windows 11 or Windows 10](https://www.microsoft.com/en-us/windows) (version 1809+)
- At least 4GB of RAM
- [Microsoft Edge WebView2 Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2/)

### 2️⃣ Git

Clone the repository:

```git
git clone https://github.com/RiversideValley/{repo name}
```
(`main` is the latest branch)

### 3️⃣ Build the project

- Open `Emerald.sln`.
- Set the Startup Project to `Emerald.Package`
- Build with `DEBUG|x64` (or `DEBUG|Any CPU`)

## ⚖️ License

Copyright (c) {repo copyright} Riverside Valley Corporation

Licensed under the MIT license as stated in the [LICENSE](LICENSE.md).
