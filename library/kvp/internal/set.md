---
description: >-
  Permet de créer une kvp (en liaison avec le nom de votre script).
---
# Set
<detail>
  <summary>Logs</summary>
  Ajoutée en **v0.1.2**
</detail>
### Appel
{% code title="example.lua" %}
```lua
nlib.kvp.internal.Set(name, value);
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
            <td>Nom de la kvp</td>
        </tr>
        <tr>
            <td>value</td>
            <td align="center">any</td>
            <td>Valeur de la kvp</td>
        </tr>
    </tbody>
</table>
***
### Utilisation
{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('mykvp_str', 'Hoj Guys');
-- If you want to get the KVP value, then it will return that: Hoj Guys
```
{% endcode %}
