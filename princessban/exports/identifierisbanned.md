---
description: >-
  Permet de savoir si un identifier est banni.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.IdentifierIsBanned(identifier);
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
      <td>identifier</td>
      <td align="center">string</td>
      <td>Identifier à vérifier</td>
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
      <td align="center">true | false</td>
      <td align="center">boolean</td>
      <td>Retourne si l'identifiant est banni ou non</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local IdentifierIsBanned = PrincessBan.IdentifierIsBanned('11000013df5ec2f');

if (IdentifierIsBanned) then
  print('Identifier is banned.');
end
```
{% endcode %}