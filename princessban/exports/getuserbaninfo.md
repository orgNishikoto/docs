---
description: >-
  Permet de connaitre le ban actuel d'un utilisateur.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.GetUserBanInfo(license);
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
      <td>License de l'utilsateur à verifier</td>
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
      <td align="center">table | nil</td>
      <td align="center">table</td>
      <td>Retourne une table qui contient toute les infos de bannissement de l'utilsateur</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local userInfo = PrincessBan.GetUserBanInfo('51c8d0dd60bd6056610e6af1dc39364c5b014f20');

print(userInfo.license);
print(userInfo.steam);
print(userInfo.fivem);
print(userInfo.live)
print(userInfo.xbox);
print(userInfo.ip);
print(userInfo.date);
print(userInfo.id);
print(userInfo.author);
print(userInfo.reason);
print(userInfo.discord);

-- output:
--   51c8d0dd60bd6056610e6af1dc39364c5b014f20
--   11000013df5ec2f
--   1424420
--   2535408403030711
--   844425085682829
--   127.0.0.1
--   20/11/2024 13:47:34
--   1
--   Nishikoto
--   Cheat
--   644585596022423553
```
{% endcode %}