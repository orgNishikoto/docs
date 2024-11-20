---
description: >-
  Permet de bannir un identifiant.
---

# BanIdentifier

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.BanIdentifier(license, identifier);
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
      <td>license</td>
      <td align="center">string</td>
      <td>License de l'utilisateur</td>
    </tr>
    <tr>
      <td>identifier</td>
      <td align="center">string</td>
      <td>Identifiant à bannir</td>
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
      <td align="center">true | nil</td>
      <td align="center">boolean | nil</td>
      <td>Permet de savoir si l'identifiant à été banni ou non</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanIdentifier = PrincessBan.BanIdentifier('51c8d0dd60bd6056610e6af1dc39364c5b014f20', '11000013df5ec2f');

if (BanIdentifier) then
  print('Identifier has been banned.');
end
```