---
description: >-
  Retrieves a kvp recorded by your script
---

# GetTable

<details>
  <summary>Logs</summary>

  Added in **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.internal.GetTable(name);
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
            <td>KVP key</td>
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
            <td align="center">table</td>
            <td>KVP value</td>
        </tr>
    </tbody>
</table>

***

### Call

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvptbl', {
    foo = 'bar',
    myname = 'isjames'
});
local kvp_value = nlib.kvp.internal.GetTable('kvptbl');

print(kvp_value, nlib.string.type(kvp_value)); -- output: {"foo"="bar", "myname"="isjames"}, string 
```
{% endcode %}

{% hint style="danger" %}
**Important**: For the moment, it's not possible to return a table, but as soon as I find a solution, it will be implemented. If not, you can always contribute to the development of the library.
{% endhint %}

{% hint style="info" %}
The latest version of the function is available on the “main” branch of the Github repository.
{% endhint %}
