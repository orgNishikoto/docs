---
description: >-
  Permet de supprimer une KVP.
---

# DeleteNumber

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.internal.kvp.DeleteBoolean(name);
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

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvp_test', true);

local mykvp = nlib.kvp.internal.GetBoolean('kvp_test');
print(mykvp); -- output: true

nlib.kvp.internal.DeleteBoolean('kvp_test');

local test2_mykvp = nlib.kvp.internal.GetBoolean('kvp_test');
print(test2_mykvp); -- output: false (ça renvoie false vu qu'elle n'existe plus)
```
{% endcode %}