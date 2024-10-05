---
description: >-
  Permet de voir la valeur de la KVP (integer ou number) de la ressource demandé.
---

# GetNumber

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.external.GetNumber(resName, kvpName);
nlib.kvp.external.GetInt(resName, kvpName); -- C'est la même chose
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
            <td>resName</td>
            <td align="center">string</td>
            <td>Nom de la resource dans laquelle la KVP est enregistré</td>
        </tr>
        <tr>
            <td>kvpName</td>
            <td align="center">string</td>
            <td>Nom de la KVP</td>
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
            <td>valeur</td>
            <td align="center">number</td>
            <td>Valeur de la KVP</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local mykvp = nlib.kvp.external.GetNumber(GetCurrentResourceName(), 'nishi_number');

print(mykvp); -- output: Renvoi la valeur ou 0 si nul
```
{% endcode %}