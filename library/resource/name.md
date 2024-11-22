---
description: Allows you to find out the name of a script (linked to fxmanifest).
---

# name

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.resource.name(resname);
```
{% endcode %}

***

### Parameters

<table><thead><tr><th width="151" align="center">Paramètre</th><th width="79" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">resname</td><td align="center">string</td><td align="center">Name of resource</td></tr></tbody></table>

***

### Return

<table><thead><tr><th width="130" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">name</td><td align="center">string</td><td align="center">Resource name defined in fxmanifest</td></tr></tbody></table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local name = nlib.resource.name('library');

print(name); -- output: Library
```
{% endcode %}
