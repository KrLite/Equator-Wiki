---
description: >-
  New to Equator? Learn here to master this ultimate toolbox which boosts your
  render stuffs in Minecraft.
layout: landing
---

# 🪐 Landing on Equator

## How Comes Equator?

**Equator** is a Powerful Modding Library for Minecraft which focuses on making rendering stuffs easier.

It may be a headache to many modders to render stuffs in Minecraft, through **Mojang's Blaze3D** renderer. **Equator** makes it much easier by wrapping the **Blaze3D** renderer and provides simple APIs for you to use.

**Equator** is aimed to be a not-too-complicated library, and humanized experience is the first priority. Throughout your way of rendering, that you can easily get the result you want is always the goal of **Equator.** Features like **immutable classes** and **chaining** are the embodiment of this goal.

## First Steps to Take

### Introduce Equator to Your Project

1. Implement **Equator** to your project through [**JitPack**](https://jitpack.io) or [**Modrinth Maven.**](https://docs.modrinth.com/docs/tutorials/maven/)

{% tabs %}
{% tab title="Modrinth Maven" %}
{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://api.modrinth.com/maven" }
}

dependencies {
    modImplementation "maven.modrinth:equator:a.b.c-v?"
}
```
{% endcode %}
{% endtab %}

{% tab title="JitPack" %}
{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://jitpack.io" }
}

dependencies {
    modImplementation "com.github.KrLite.Equator-v2:build:a.b.c-v?"
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

* `a.b.c` stands for **Minecraft** version, you should always use **the full version,** for example, `1.19.4`. If the version does not exist, consider trying again **excluding the min version,** for example, use `1.19` instead of `1.19.4`. If the version still does not exist, **Equator** may not supporting the target **Minecraft** version.
* `v?` stands for **Equator** version, which is **equivalent to the release tag,** for example, `v2.4.0`. Using the latest version is recommended.
* Not all versions support all **Minecraft** versions, **please check the requirements before implementing.**

**Overall, a legal version is like: `1.19.4-v2.4.0`.**

If you want to only include modules apart from **Equator** respectively into your mod, here's an instruction.

{% content-ref url="miscellaneous/module-implementation.md" %}
[module-implementation.md](miscellaneous/module-implementation.md)
{% endcontent-ref %}

2. Add the dependency to your `fabric/quilt.mod.json` file.

{% code overflow="wrap" %}
```json
"depends": {
    "equator": "a.b.c-v?"
}
```
{% endcode %}

3. Re-run the gradle task.

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
