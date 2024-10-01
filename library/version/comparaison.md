---
description: >-
  Permet de comparé la version de votre script avec la version de la dernière
  release d'un dépôt GitHub (publique).
---

# Comparaison

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.0**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.version.compare(username, reponame, version);
```
{% endcode %}

---

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
      <td>Nom du dépôt github</td>
    </tr>
    <tr>
      <td>version</td>
      <td align="center">string</td>
      <td>Version de votre script</td>
    </tr>
  </tbody>
</table>

---

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
      <td align="center">lower | upper | equal | error</td>
      <td align="center">string</td>
      <td>Status de la comparaison</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local status = nlib.version.compare('orgNishikoto', 'library', '0.1.0');

print(status); -- output: equal
```
{% endcode %}
