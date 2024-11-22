---
description: Allows you to find out the version of a script (linked to fxmanifest).
---

# version

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.resource.author(resname);
```
{% endcode %}

***

### Parameters

<table><thead><tr><th width="151" align="center">Parameter</th><th width="79" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">resname</td><td align="center">string</td><td align="center">Name of resource</td></tr></tbody></table>

***

### Return

<table><thead><tr><th width="142" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">version</td><td align="center">string</td><td align="center">Resource version defined in fxmanifest</td></tr></tbody></table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local version = nlib.resource.version('library');

print(version); -- output: fork-alpha-0.1.2
```
{% endcode %}
