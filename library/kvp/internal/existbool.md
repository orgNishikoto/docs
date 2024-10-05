---
description: >-
  Permet de savoir si une KVP existe.
---

# ExistBoolean

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.internal.ExistBoolean(name);
```
{% endcode %}

***

### Paramètres

<table>
    <thead>
        <tr>
            <th width="151" align="center">Paramètre</th>
            <th width="79" align="center">Type</th>
            <th align="center">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>name</td>
            <td align="center">string</td>
            <td>Nom/Clé de la KVP</td>
        </tr>
    </tbody>
</table>

***

### Retours

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
            <td>True si la KVP existe, sinon false</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvp_test', true);
local kvp_status = nlib.kvp.internal.ExistBoolean('kvp_test');
local kvp_status2 = nlib.kvp.internal.ExistBoolean('kvp_2');

print(kvp_status); -- output: true
print(kvp_status2); -- output: false
```
{% endcode %}
