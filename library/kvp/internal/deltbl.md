---
description: >-
  Permet de supprimer une KVP.
---

# DeleteNumber

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.internal.kvp.DeleteTable(name);
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
nlib.kvp.internal.Set('kvp_test', { foo = 'bar' });

local mykvp = nlib.kvp.internal.GetTable('kvp_test');
print(mykvp); -- output: { foo = 'bar' }

nlib.kvp.internal.DeleteTable('kvp_test');

local test2_mykvp = nlib.kvp.internal.GetTable('kvp_test');
print(test2_mykvp); -- output: {} (it returns a vacuum since it no longer exists)
```
{% endcode %}
