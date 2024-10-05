---
description: >-
  Permet de récupérer une kvp enregistrer par votre script
---

# GetBoolean

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.internal.GetBoolean(name);
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
            <td>kvp</td>
            <td align="center">boolean</td>
            <td>Valeur de la KVP</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('kvpbool', true);
local kvp_value = nlib.kvp.internal.GetBoolean('kvpbool');

print(kvp_value, nlib.string.type(kvp_value)); -- output: true, boolean 
```
{% endcode %}
