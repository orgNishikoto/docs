---
description: >-
  Determines whether a KVP exists.
---

# ExistNumber

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.kvp.internal.ExistNumber(name);
nlib.kvp.internal.ExistInt(name);
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
            <td>status</td>
            <td align="center">boolean</td>
            <td>True if the KVP exists, or false</td>
        </tr>
    </tbody>
</table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvp_test', 45);
local kvp_status = nlib.kvp.internal.ExistInt('kvp_test');
local kvp_status2 = nlib.kvp.internal.ExistInt('kvp_2');

print(kvp_status); -- output: true
print(kvp_status2); -- output: false
```
{% endcode %}
