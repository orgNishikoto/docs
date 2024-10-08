---
description: >-
  Permet de récupérer une kvp enregistrer par votre script
---

# GetTable

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.internal.GetTable(name);
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
            <td align="center">table</td>
            <td>Valeur de la KVP</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

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
**Important**: Pour le moment il n'est pas possible de retourner une table, dés que je trouve la solution elle sera mise en place, sinon vous pouvez toujours contribuer au développement de la bibliothèque.
{% endhint %}

{% hint style="info" %}
La dernière version de la fonction est disponible sur la branche "main" du dépôt Github.
{% endhint %}
