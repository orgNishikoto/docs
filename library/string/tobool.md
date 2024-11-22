---
description: >-
  This function simply transforms a “string” or “number” variable into a “boolean”.
  “number” variable into a ‘boolean’.
---

# tobool

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.string.tobool(variable);
tobool(variable);
```
{% endcode %}

***

### Parameters

<table><thead><tr><th width="151" align="center">Parameter</th><th width="176" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">variable</td><td align="center">string | number</td><td align="center"></td></tr></tbody></table>

***

### Return

<table><thead><tr><th width="179" align="center">Variable</th><th width="120" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">boolean</td><td align="center">boolean</td><td align="center">Variable transformed into boolean</td></tr></tbody></table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local var1 = nlib.string.tobool('true');
local var2 = tobool(0);

print(var1); -- output: true
print(var2); -- output: false
```
{% endcode %}
