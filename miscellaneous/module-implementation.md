---
description: Include modules perspectively into your mod.
---

# 💾 Module Implementation

**Equator** should not be included into your mod as it has many independent functions. However, this instruction shows you how to include **Equator** as modules.

First of all, add **JitPack** to your repositories.

{% code title="build.gradle" overflow="wrap" %}
```gradle
repositories {
    maven { url "https://jitpack.io" }
}
```
{% endcode %}

> Module implementation is only due to the support of [**JitPack.**](https://jitpack.io/#KrLite/Equator-v2)****

## Including Modules

{% tabs %}
{% tab title="Animation" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("maven.modrinth.equator:Animation:v?")
}
```
{% endcode %}

Module **Animation** contains classes including **Animation, Interpolation** and **Slices.**
{% endtab %}

{% tab title="Math" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("maven.modrinth.equator:Math:v?")
}
```
{% endcode %}

Module **Math** contains classes including **Vector, Box, Theory** and **FrameInfo.**
{% endtab %}

{% tab title="Visual" %}
{% code overflow="wrap" %}
```gradle
dependencies {
    modImplementation include("maven.modrinth.equator:Visual:v?")
}
```
{% endcode %}

Module **Visual** contains classes including **AccurateColor** and **Palette.**
{% endtab %}
{% endtabs %}

* Not all versions support all Minecraft versions, **please check the requirements before implementing.**
* `v?` stands for **Equator**'s version, which is **equivalent to the release tag,** for example, `v2.0.0`. Using the latest version is recommended.

> All modules' methods and classes are strictly in line with **Equator**'s, which enables you switching to **Equator** at any time.

{% content-ref url="../" %}
[..](../)
{% endcontent-ref %}
