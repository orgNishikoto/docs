---
description: Creates a kvp (linked to your script name).
---

# Set

<details>

<summary>Logs</summary>

Ajoutée en **v0.1.2**

</details>

#### Call

{% code title="example.lua" %}
```lua
nlib.kvp.internal.Set(name, value);
```
{% endcode %}

***

#### Parameters

<table><thead><tr><th width="151" align="center">Parameter</th><th width="79" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">name</td><td align="center">string</td><td align="center">Name of kvp</td></tr><tr><td align="center">value</td><td align="center">any</td><td align="center">kvp value</td></tr></tbody></table>

***

#### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('mykvp_str', 'Hoj Guys');
-- If you want to get the KVP value, then it will return that: Hoj Guys
```
{% endcode %}
