---
description: >-
  Permet de connaître la version d'un dépôt GitHub (publique).
---

# Get

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.0**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.version.get(username, reponame, truncate);
```
{% endcode %}

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
            <td>username</td>
            <td align="center">string</td>
            <td>Nom de l'utilisateur github ou de l'organisation github</td>
        </tr>
        <tr>
            <td>reponame</td>
            <td align="center">string</td>
            <td>Nom du dépôt github ou de l'organisation github</td>
        </tr>
        <tr>
            <td>truncate</td>
            <td align="center">boolean</td>
            <td>Permet d'avoir le nom de la version complète (fork-x.x.x) ou coupé (x.x.x)</td>
        </tr>
    </tbody>
</table>

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
            <td>version</td>
            <td align="center">string</td>
            <td>Version du dépôt GitHub séléctionné</td>
        </tr>
    </tbody>
</table>

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local version_truncate = nlib.version.compare('orgNishikoto', 'library', true);
local version_notruncate = nlib.version.compare('orgNishikoto', 'library', false);

print(version_truncate); -- output: fork-alpha-0.1.0
print(version_notruncate); -- output: 0.1.0
```
{% endcode %}



test.lua