---
description: Allows you to find out the author of a script (linked to fxmanifest).
---

# author

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
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

<table><thead><tr><th width="161" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">author</td><td align="center">string</td><td align="center">Author of the resource defined in fxmanifest</td></tr></tbody></table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local author = nlib.resource.author('library');

print(author); -- output: Nishikoto <https://www.nishikoto.fr>
```
{% endcode %}
