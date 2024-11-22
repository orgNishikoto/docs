---
icon: down-to-bracket
---

# Installation

## Dependency

[Lib](https://github.com/JustGodWork/lib/releases/latest) is required to run Library.

* Click [here](https://github.com/JustGodWork/lib/blob/main/README.md#getting-started) to follow the steps for installing the library.

## Installation

{% tabs %}
{% tab title="Manually" %}
* Download the latest [release](https://github.com/orgNishikoto/library/releases/latest)
* Add `ensure library` in your `server.cfg` or `resource.cfg` file
* Copy the contents of the `convars.cfg` file (included in the library) into your `server.cfg` or `resource.cfg` file

{% hint style="info" %}
Tips: Start the **library** resource before your personal resources
{% endhint %}

{% hint style="info" %}
The rest is an integration for your personal resources only, in my scripts the library is already called.
{% endhint %}

{% code title="fxmanifest.lua" lineNumbers="true" %}
```lua
shared_scripts {
    '@lib/imports.lua',
    '@library/imports.lua'
} 
```
{% endcode %}
{% endtab %}

{% tab title="By git" %}
{% code title="" lineNumbers="true" %}
```
git clone https://github.com/orgNishikoto/library.git
```
{% endcode %}
{% endtab %}
{% endtabs %}
