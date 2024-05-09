# Extensive RV Builder

[![CI](https://github.com/AbakNacchan/RV/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/AbakNacchan/RV/actions/workflows/ci.yml)

※ Get the [latest CI release](https://github.com/AbakNacchan/RV/releases) ※

<details><summary><big>Features</big></summary>
<ul>
 <li>Supports all existing and upcoming RV apps</li>
 <li>Can create Magisk modules and non-root APKs</li>
 <li>Updates regularly with the newest versions of apps and patches</li>
 <li>Optimizes APKs and modules for size</li>
 <li>Modules</li>
    <ul>
     <li>Recompile invalidated odex files for faster performance</li>
     <li>Get updates from the Magisk app</li>
     <li>Avoid breaking SafetyNet or triggering root detections</li>
     <li>Manage the installation of the appropriate version of the stock app and other related tasks</li>
     <li>Supports Magisk and KernelSU</li>
    </ul>
</ul>
Be aware that GitHub Actions will trigger the <a href="../../actions/workflows/ci.yml">CI workflow</a> to build the modules and APKs daily if there is a change in RV patches. You might want to turn it off.
</details>

## To include/exclude patches or to patch other apps
[**See the list of patches**](https://j-hc.github.io/rvmm-config-gen/)

 * Star the repo
 * Use the repo as a [template](https://github.com/AbakNacchan/revanced-extended/fork)
 * Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

Also see [`CONFIG.md`](./CONFIG.md).

## Building Locally
### On Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/AbakNacchan/RV/main/build-termux.sh)
```

### On Desktop
```console
$ git clone https://github.com/AbakNacchan/RV
$ cd revanced-extended
$ ./build.sh
```
