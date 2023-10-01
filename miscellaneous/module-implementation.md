---
description: Include modules from Equator into your project perspectively.
---

# 💾 Module Implementation

**Equator** should not be included into your mod as it has many independent functions. However, this instruction shows you how to include **Equator** as modules.

Note well that all the modules **work as mods,** and depend on Fabric because the usage of certain functions. However, they are safe to be included in your project.

First of all, add [**JitPack**](https://jitpack.io/#KrLite/Equator-v2) to your repositories.

{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://jitpack.io" }
}
```
{% endcode %}

## Choosing Modules

{% tabs %}
{% tab title="Animation" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("com.github.KrLite.Equator-v2:Animation:?-mcx.x.x")
}
```
{% endcode %}

Module **Animation** contains classes including **Animation, Interpolation** and **Slice.**
{% endtab %}

{% tab title="Math" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("com.github.KrLite.Equator-v2:Math:?-mcx.x.x")
}
```
{% endcode %}

Module **Math** contains classes including **Vector, Box, Theory** and **FrameInfo.**
{% endtab %}

{% tab title="Visual" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("com.github.KrLite.Equator-v2:Visual:a.b.c-v?")
}
```
{% endcode %}

Module **Visual** contains classes including **AccurateColor** and **Palette.**
{% endtab %}
{% endtabs %}

{% hint style="info" %}
* `a.b.c` stands for **Minecraft** version.
  * You should always use **the full version,** for example, `1.20.1`.&#x20;
  * If the build does not exist, consider trying again **excluding the min version,** for example, use `1.20` instead of `1.20.1`.&#x20;
  * If the build still does not exist, **Equator** may not support the targeting **Minecraft** version.
* `v?` stands for **Equator** version.
  * **Equivalent to the release tag,** for example, `v2.5.1`.&#x20;
  * Using the latest version is recommended.
* Different **Equator** versions support different **Minecraft** versions, **please check the requirements before implementing.**
{% endhint %}

{% hint style="success" %}
**Overall, a legal version is like: `1.20.1-v2.5.1`.**
{% endhint %}

> All modules' methods and classes are strictly in line with **Equator**'s, which enables you switching to use **Equator** freely and without any worries.

{% content-ref url="../" %}
[..](../)
{% endcontent-ref %}
