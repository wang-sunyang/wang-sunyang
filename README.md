<div align="center">

<img src="https://avatars.githubusercontent.com/u/223229607?v=4&s=200" width="110" alt="Wang Sunyang" />

<sub>[简体中文](README.zh-CN.md) &nbsp;·&nbsp; **English**</sub>

</div>

---

# Wang Sunyang · 王孙阳

**Indie developer · Native Android · No WebView shells, no dependency bloat**

One person doing product, code, QA and release. I believe *one less abstraction layer means one less class of bugs*.

[![Website](https://img.shields.io/badge/website-yangyang2857--rgb.github.io-2ea44f?logo=githubpages&logoColor=white)](https://wang-sunyang.github.io/)
[![Location](https://img.shields.io/badge/location-Hubei%C2%B7Jingzhou%2C%20China-1f6feb?logo=googlemaps&logoColor=white)](#)
[![Followers](https://img.shields.io/github/followers/wang-sunyang?label=followers&color=8957e5)](https://github.com/wang-sunyang?tab=followers)
[![Profile views](https://komarev.com/ghpvc/?username=wang-sunyang&label=views&color=3DDC84&style=flat)](https://github.com/wang-sunyang)

## About me

| | |
| --- | --- |
| **Who I am** | Vocational student and a one-person dev team: product, coding, testing and release all run by me |
| **Approach** | Native first. If the platform API can do it, no framework; if the system toolchain can do it, no build system |
| **Currently building** | A Gradle-free Android build chain, a guardrail SDK for AI agent function calls, an audit-only disk CLI that never deletes, and a dependency-free personal site |
| **What I believe** | Fewer dependencies, fewer failure surfaces. A reproducible build beats a clever one |

## What I'm building

### OneStar

> A native Android build experiment with no Gradle and no AGP: `aapt2` + `javac` + `d8` + `apksigner` + `zig cc`, all driven by one `build.sh`.

[![Repo](https://img.shields.io/badge/repo-onestar-1f6feb?logo=github&logoColor=white)](https://github.com/wang-sunyang/onestar)
[![build](https://img.shields.io/github/actions/workflow/status/wang-sunyang/onestar/android.yml?branch=main&label=build&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/onestar/actions/workflows/android.yml)
[![regression](https://img.shields.io/github/actions/workflow/status/wang-sunyang/onestar/regression.yml?branch=main&label=regression&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/onestar/actions/workflows/regression.yml)
[![Release](https://img.shields.io/github/v/release/wang-sunyang/onestar?label=release&color=3DDC84)](https://github.com/wang-sunyang/onestar/releases)
[![License](https://img.shields.io/github/license/wang-sunyang/onestar?label=license&color=2ea44f)](https://github.com/wang-sunyang/onestar/blob/main/LICENSE)

- Supports **Android 5.0+ (API 21)**, localized into **15 languages**
- JNI pieces cross-compiled with `zig cc`, no NDK Gradle wrapper
- No Gradle cache, no daemon — predictable build times

### AppFunction Guard

> Android 16 lets AI agents call functions inside your app. This project adds the doorman, the doorbell and the visitor log the platform forgot.

[![Repo](https://img.shields.io/badge/repo-appfunction--guard-1f6feb?logo=github&logoColor=white)](https://github.com/wang-sunyang/appfunction-guard)
[![build](https://img.shields.io/github/actions/workflow/status/wang-sunyang/appfunction-guard/build.yml?branch=main&label=build&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/appfunction-guard/actions/workflows/build.yml)
[![publish](https://img.shields.io/github/actions/workflow/status/wang-sunyang/appfunction-guard/publish-central.yml?branch=main&label=publish&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/appfunction-guard/actions/workflows/publish-central.yml)
[![License](https://img.shields.io/github/license/wang-sunyang/appfunction-guard?label=license&color=2ea44f)](https://github.com/wang-sunyang/appfunction-guard/blob/main/LICENSE)
[![Status](https://img.shields.io/badge/status-alpha-orange)](#)

- **Per-function** access control over `AppFunctions`: authorization, rate limiting and auditing in one chain
- Kotlin 2.2, `minSdk 26`, MIT licensed

### wang-sunyang.github.io

> A hand-written HTML / CSS / JavaScript site: no framework, no build step, no third-party dependencies. Edit a file, `git push`, done.

[![Site](https://img.shields.io/badge/website-online-2ea44f?logo=githubpages&logoColor=white)](https://wang-sunyang.github.io/)
[![pages](https://img.shields.io/github/actions/workflow/status/wang-sunyang/wang-sunyang.github.io/pages/pages-build-deployment?branch=main&label=pages&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/wang-sunyang.github.io/actions)
[![Repo](https://img.shields.io/badge/repo-yangyang2857--rgb.github.io-1f6feb?logo=github&logoColor=white)](https://github.com/wang-sunyang/wang-sunyang.github.io)

- `dependencies: 0`, hosted on GitHub Pages
- Single-page long scroll, dark/light themes, hand-written browser fallbacks

### moltdisk

> Most of the bulk in your projects is build output that can be rebuilt from source. This finds it, measures it, and shows the evidence for why it is disposable — then it stops. It deletes nothing.

[![Repo](https://img.shields.io/badge/repo-moltdisk-1f6feb?logo=github&logoColor=white)](https://github.com/wang-sunyang/moltdisk)
[![ci](https://img.shields.io/github/actions/workflow/status/wang-sunyang/moltdisk/ci.yml?branch=main&label=ci&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/moltdisk/actions/workflows/ci.yml)
[![Release](https://img.shields.io/github/v/release/wang-sunyang/moltdisk?label=release&color=DEA584)](https://github.com/wang-sunyang/moltdisk/releases)
[![License](https://img.shields.io/github/license/wang-sunyang/moltdisk?label=license&color=2ea44f)](https://github.com/wang-sunyang/moltdisk/blob/main/LICENSE)

- Walks `node_modules` / `target` / `dist` / `venv` / `Pods` and common caches, ranks them by size, explains each verdict
- Rust 2021, MSRV 1.80; no delete module, no `remove_dir_all`, and `-y` is a hard error

### Marvis · Persona Spec

> A persona spec that a program can check: the style guide says who she is, this says which line she says next.

[![Repo](https://img.shields.io/badge/repo-marvis--persona--spec-1f6feb?logo=github&logoColor=white)](https://github.com/wang-sunyang/marvis-persona-spec)
[![lint](https://img.shields.io/github/actions/workflow/status/wang-sunyang/marvis-persona-spec/persona-lint.yml?branch=main&label=lint&logo=githubactions&logoColor=white)](https://github.com/wang-sunyang/marvis-persona-spec/actions/workflows/persona-lint.yml)
[![License](https://img.shields.io/github/license/wang-sunyang/marvis-persona-spec?label=license&color=2ea44f)](https://github.com/wang-sunyang/marvis-persona-spec/blob/main/LICENSE)

- 30 line slots, 20 banned phrases, a working lint script and 10 baseline tests, plus the Fault Bloom visual system
- Two-stage CI: greyscale reporting first, blocking gate once the backlog reaches zero

## Toolbox

<div align="center">

**Languages**

![Kotlin](https://img.shields.io/badge/-Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/-Java-ED8B00?logo=openjdk&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/-Shell-4EAA25?logo=gnubash&logoColor=white)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black)

**Platform & toolchain**

![Android](https://img.shields.io/badge/-Android-3DDC84?logo=android&logoColor=white)
![aapt2](https://img.shields.io/badge/-aapt2-8957e5)
![d8](https://img.shields.io/badge/-d8-8957e5)
![apksigner](https://img.shields.io/badge/-apksigner-8957e5)
![JNI](https://img.shields.io/badge/-JNI-1f6feb)
![zig cc](https://img.shields.io/badge/-zig%20cc-F7A41D?logo=zig&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/-GitHub%20Pages-2ea44f?logo=githubpages&logoColor=white)

</div>

## Numbers

<div align="center">

![Streak](https://streak-stats.demolab.com?user=wang-sunyang&theme=github-dark&hide_border=true&locale=en)

</div>

| Repo | Language | Latest release | Last commit |
| --- | --- | --- | --- |
| [onestar](https://github.com/wang-sunyang/onestar) | ![lang](https://img.shields.io/github/languages/top/wang-sunyang/onestar) | ![release](https://img.shields.io/github/v/release/wang-sunyang/onestar) | ![last](https://img.shields.io/github/last-commit/wang-sunyang/onestar) |
| [appfunction-guard](https://github.com/wang-sunyang/appfunction-guard) | ![lang](https://img.shields.io/github/languages/top/wang-sunyang/appfunction-guard) | — | ![last](https://img.shields.io/github/last-commit/wang-sunyang/appfunction-guard) |
| [wang-sunyang.github.io](https://github.com/wang-sunyang/wang-sunyang.github.io) | ![lang](https://img.shields.io/github/languages/top/wang-sunyang/wang-sunyang.github.io) | — | ![last](https://img.shields.io/github/last-commit/wang-sunyang/wang-sunyang.github.io) |
| [moltdisk](https://github.com/wang-sunyang/moltdisk) | ![lang](https://img.shields.io/github/languages/top/wang-sunyang/moltdisk) | ![release](https://img.shields.io/github/v/release/wang-sunyang/moltdisk) | ![last](https://img.shields.io/github/last-commit/wang-sunyang/moltdisk) |
| [marvis-persona-spec](https://github.com/wang-sunyang/marvis-persona-spec) | ![lang](https://img.shields.io/github/languages/top/wang-sunyang/marvis-persona-spec) | — | ![last](https://img.shields.io/github/last-commit/wang-sunyang/marvis-persona-spec) |

### CI status

| Repo | Workflow | Status |
| --- | --- | --- |
| onestar | `android.yml` | ![build](https://img.shields.io/github/actions/workflow/status/wang-sunyang/onestar/android.yml?branch=main&label=status) |
| onestar | `regression.yml` | ![regression](https://img.shields.io/github/actions/workflow/status/wang-sunyang/onestar/regression.yml?branch=main&label=status) |
| appfunction-guard | `build.yml` | ![build](https://img.shields.io/github/actions/workflow/status/wang-sunyang/appfunction-guard/build.yml?branch=main&label=status) |
| appfunction-guard | `publish-central.yml` | ![publish](https://img.shields.io/github/actions/workflow/status/wang-sunyang/appfunction-guard/publish-central.yml?branch=main&label=status) |
| wang-sunyang.github.io | `pages-build-deployment` | ![pages](https://img.shields.io/github/actions/workflow/status/wang-sunyang/wang-sunyang.github.io/pages/pages-build-deployment?branch=main&label=status) |
| moltdisk | `ci.yml` | ![ci](https://img.shields.io/github/actions/workflow/status/wang-sunyang/moltdisk/ci.yml?branch=main&label=status) |
| marvis-persona-spec | `persona-lint.yml` | ![lint](https://img.shields.io/github/actions/workflow/status/wang-sunyang/marvis-persona-spec/persona-lint.yml?branch=main&label=status) |

## Contact

- Website: <https://wang-sunyang.github.io/>
- Studio: [Nightglean Studio](https://github.com/nightglean)
- Questions or ideas: open an issue in the relevant repo — faster than email

<div align="center">

<sub>One less abstraction layer, one less class of bugs.</sub>

</div>
