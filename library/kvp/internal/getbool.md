---
description: >-
  Retrieves a kvp recorded by your script
---

# GetBoolean

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.kvp.internal.GetBoolean(name);
```
{% endcode %}

***

### Parameters

<table>
    <thead>
        <tr>
            <th width="151" align="center">Parameter</th>
            <th width="79" align="center">Type</th>
            <th align="center">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>name</td>
            <td align="center">string</td>
            <td>KVP name</td>
        </tr>
    </tbody>
</table>

***

### Return

<table>
    <thead>
        <tr>
            <th width="254" align="center">Variable</th>
            <th width="82" align="center">Type</th>
            <th align="center">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>kvp</td>
            <td align="center">boolean</td>
            <td>KVP value</td>
        </tr>
    </tbody>
</table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvpbool', true);
local kvp_value = nlib.kvp.internal.GetBoolean('kvpbool');

print(kvp_value, nlib.string.type(kvp_value)); -- output: true, boolean 
```
{% endcode %}
