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
nlib.internal.kvp.DeleteNumber(name);
nlib.internal.kvp.DeleteInt(name);
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
nlib.kvp.internal.Set('kvp_test', 47);

local mykvp = nlib.kvp.internal.GetInt('kvp_test');
print(mykvp); -- output: 47

nlib.kvp.internal.DeleteInt('kvp_test');

local test2_mykvp = nlib.kvp.internal.GetInt('kvp_test');
print(test2_mykvp); -- output: 0 (ça renvoie 0 vu qu'elle n'existe plus)
```
{% endcode %}
