---
description: >-
  New to Equator? Learn here to master this ultimate toolbox which boosts your
  render stuffs in Minecraft.
layout: landing
---

# 🪐 Landing on Equator

## How Equator Works?

**Equator** is a Powerful Modding Library for Minecraft which focuses on making rendering stuffs easier.

It may be a headache to many modders to render stuffs in Minecraft, through **Mojang's Blaze3D** renderer. **Equator** makes it much easier by wrapping the **Blaze3D** renderer and provides simple APIs for you to use.

**Equator** is aimed to be a not-too-complicated library, and humanized experience is the first priority. Throughout your way of rendering, that you can easily get the result you want is always the goal of **Equator.** Features like **immutable classes** and **chaining** are the embodiment of this goal.

## First Steps to Take

### Introduce Equator to Your Project

1. Implement **Equator** to your project through [**JitPack**](https://jitpack.io) or [**Modrinth Maven**](https://api.modrinth.com/maven)**.**

{% tabs %}
{% tab title="JitPack" %}
{% code title="build.gradle" overflow="wrap" %}
```groovy
repositories {
    maven { url "https://jitpack.io" }
}

dependencies {
    modImplementation "com.github.KrLite:Equator:xxx" // Not completed yet
}
```
{% endcode %}
{% endtab %}

{% tab title="Modrinth Maven" %}
{% code title="build.gradle" overflow="wrap" %}
```groovy
repositories {
    maven { url "https://api.modrinth.com/maven" }
}

dependencies {
    modImplementation "maven.modrinth:equator:xxx" // Not completed yet
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

2. Add the dependency to your `fabric/quilt.mod.json` file.

{% code overflow="wrap" %}
```json
"depends": {
    "equator": "*"
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
