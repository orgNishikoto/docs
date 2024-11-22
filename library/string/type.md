---
description: Identifies the type of a variable.
---

# type

{% hint style="warning" %}
Warning: I'm only adding the fact that I can see the 'float' type of a number, so yes, it's possible to see other types with this function.

That's why I haven't replaced lua's native `type()` function.
{% endhint %}

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.string.type(variable);
```
{% endcode %}

***

### Parameters

<table><thead><tr><th width="151" align="center">Parameter</th><th width="96" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">variable</td><td align="center">any</td><td align="center"></td></tr></tbody></table>

***

#### Return

<table><thead><tr><th width="190" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">type</td><td align="center">string</td><td align="center">The type of variable sent</td></tr></tbody></table>

***

#### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local whatismynumber = 8.9;
local typeof = nlib.string.type(whatismynumber);

print(typeof); -- output: float
```
{% endcode %}
