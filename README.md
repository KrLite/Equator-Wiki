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

## First Steps to Take

### Introduce Equator to Your Project

1. Implement **Equator** to your project through [**JitPack**](https://jitpack.io) or [**Modrinth Maven.**](https://docs.modrinth.com/docs/tutorials/maven/)

{% tabs %}
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

{% tab title="Modrinth Maven" %}
{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://api.modrinth.com/maven" }
}

dependencies {
    // Not recommended
    modImplementation "maven.modrinth:equator:a.b.c-v?"
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

* `a.b.c` stands for **Minecraft** version.
  * You should always use **the full version,** for example, `1.20.1`.&#x20;
  * If the build does not exist, consider trying again **excluding the min version,** for example, use `1.20` instead of `1.20.1`.&#x20;
  * If the build still does not exist, **Equator** may not support the targeting **Minecraft** version.
* `v?` stands for **Equator** version.
  * **Equivalent to the release tag,** for example, `v2.5.1`.&#x20;
  * Using the latest version is recommended.
* Different **Equator** versions support different **Minecraft** versions, **please check the requirements before implementing.**

**Overall, a legal version is like: `1.20.1-v2.5.1`.**

{% hint style="info" %}
If you want to only include modules apart from **Equator** respectively into your mod, here's an instruction.
{% endhint %}

{% content-ref url="miscellaneous/module-implementation.md" %}
[module-implementation.md](miscellaneous/module-implementation.md)
{% endcontent-ref %}

2. Add the dependency to your `fabric/quilt.mod.json` file.

{% tabs %}
{% tab title="Fabric" %}
<pre class="language-json" data-overflow="wrap"><code class="lang-json">"depends": {
    "equator": "<a data-footnote-ref href="#user-content-fn-1">?</a>"
}
</code></pre>
{% endtab %}

{% tab title="Quilt" %}
<pre class="language-json"><code class="lang-json">"depends": [
    {
        "id": "equator",
        "versions": "<a data-footnote-ref href="#user-content-fn-2">?</a>"
     }
]
</code></pre>
{% endtab %}
{% endtabs %}

3. Re-run the gradle task.

***

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

[^1]: It is fine for you to only fill up the raw version component, such as `2.5.3`.

[^2]: It is fine for you to only fill up the raw version component, such as `2.5.3`.
