---
description: >-
  New to Equator? Learn here to master this ultimate toolbox which boosts your
  render stuffs in Minecraft.
cover: https://github.com/KrLite/Equator-v2/blob/artwork/Banner.png?raw=true
coverY: 52
layout: landing
---

# 🪐 Landing on Equator

## How Comes Equator?

**Equator** is a Powerful Modding Library for Minecraft which focuses on making rendering stuffs easier.

It may be a headache to many modders to render stuffs in Minecraft, through **Mojang's Blaze3D** renderer. **Equator** makes it much easier by wrapping the **Blaze3D** renderer and provides simple APIs for you to use.

**Equator** is aimed to be a not-too-complicated library, and humanized experience is the first priority. Throughout your way of rendering, that you can easily get the result you want is always the goal of **Equator.** Features like **immutable classes** and **chaining** are the embodiment of this goal.

## Introduce Equator to Your Project

1. Implement **Equator** to your project through [**JitPack**](https://jitpack.io) or [**Modrinth Maven.**](https://docs.modrinth.com/docs/tutorials/maven/)

{% tabs %}
{% tab title="JitPack" %}
{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://jitpack.io" }
}

dependencies {
    modImplementation "com.github.KrLite.Equator-v2:build:?-mcx.x.x"
}
```
{% endcode %}
{% endtab %}

{% tab title="Modrinth Maven" %}
{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://api.modrinth.com/maven" }
}

dependencies {
    // Not recommended
    modImplementation "maven.modrinth:equator:?-mcx.x.x?"
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

{% hint style="info" %}
* `x.x.x` stands for **Minecraft** version.
  * You should always use **the full version,** for example, `1.20.2`.&#x20;
  * If the build does not exist, consider trying again **excluding the min version,** for example, use `1.20` instead of `1.20.2`.&#x20;
  * If the build still does not exist, **Equator** may not support the targeting **Minecraft** version.
* `?` stands for **Equator** version.
  * **Equivalent to the release tag,** for example, `2.6.0`.&#x20;
  * Using the latest version is recommended.
* Different **Equator** versions support different **Minecraft** versions, **please check the requirements before implementing.**
{% endhint %}

{% hint style="success" %}
**Overall, a legal version is like: `2.6.0-mc1.20`.**
{% endhint %}

{% hint style="info" %}
If you want to only include modules apart from **Equator** into your project perspectively, please follow the instruction below.
{% endhint %}

{% content-ref url="miscellaneous/module-implementation.md" %}
[module-implementation.md](miscellaneous/module-implementation.md)
{% endcontent-ref %}

2. Add the dependency to your `fabric/quilt.mod.json` file.

{% tabs %}
{% tab title="Fabric" %}
{% code overflow="wrap" %}
```json
"depends": {
    "equator": "?"
}
```
{% endcode %}
{% endtab %}

{% tab title="Quilt" %}
```json
"depends": [
    {
        "id": "equator",
        "versions": "?"
     }
]
```
{% endtab %}
{% endtabs %}

3. Re-run the gradle task.

## Getting Started

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
