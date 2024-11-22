---
description: Provides the description of a script (linked to fxmanifest).
---

# description

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.resource.description(resname);
```
{% endcode %}

***

### Parameters

<table><thead><tr><th width="151" align="center">Parameter</th><th width="79" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">resname</td><td align="center">string</td><td align="center">Name of resource</td></tr></tbody></table>

***

### Return

<table><thead><tr><th width="141" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">description</td><td align="center">string</td><td align="center">Description of the resource defined in the fxmanifest</td></tr></tbody></table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local desc = nlib.resource.description('library');

print(desc); -- output: nil (since it is not defined, it returns nothing)
```
{% endcode %}
