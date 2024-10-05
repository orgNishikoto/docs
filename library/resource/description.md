---
description: >-
  Permet de connaître la description d'un script (lié au fxmanifest).
---

# Description

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.resource.description(resname);
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
            <td>resname</td>
            <td align="center">string</td>
            <td>Nom de la resource</td>
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
            <td>description</td>
            <td align="center">string</td>
            <td>Description de la resource défini dans le fxmanifest</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local desc = nlib.resource.description('library');

print(desc); -- output: nil (vu quel n'est pas défini elle ne renvoie rien)
```
{% endcode %}