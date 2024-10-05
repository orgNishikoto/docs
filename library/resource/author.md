---
description: >-
  Permet de connaître l'auteur d'un script (lié au fxmanifest).
---

# Description

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.resource.author(resname);
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
            <td>author</td>
            <td align="center">string</td>
            <td>Auteur de la resource défini dans le fxmanifest</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local author = nlib.resource.author('library');

print(author); -- output: Nishikoto <https://www.nishikoto.fr>
```
{% endcode %}