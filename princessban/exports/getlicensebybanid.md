---
description: >-
  Permet de connaître la license d'un utilisateur banni via un banId.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.GetLicenseByBanId(id);
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
      <td>id</td>
      <td align="center">number</td>
      <td>BanID de l'utilisateur</td>
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
      <td align="center">license</td>
      <td align="center">string</td>
      <td></td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local License = PrincessBan.GetLicenseByBanId(1);

print(License);

-- output: 51c8d0dd60bd6056610e6af1dc39364c5b014f20
```