---
description: >-
  Used to delete a KVP.
---

# DeleteNumber

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.internal.kvp.DeleteNumber(name);
nlib.internal.kvp.DeleteInt(name);
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

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvp_test', 47);

local mykvp = nlib.kvp.internal.GetInt('kvp_test');
print(mykvp); -- output: 47

nlib.kvp.internal.DeleteInt('kvp_test');

local test2_mykvp = nlib.kvp.internal.GetInt('kvp_test');
print(test2_mykvp); -- output: 0 (it returns a vacuum since it no longer exists)
```
{% endcode %}
