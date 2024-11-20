---
description: >-
  Permet de connaître l'historique de bannissement d'un utilisateur.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.GetUserBanHistory(license);
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
      <td>License de l'utilisateur à vérifier</td>
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
      <td align="center">table</td>
      <td align="center">table</td>
      <td>Liste des informations de l'utilsateur</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local UserHistory = PrincessBan.GetUserBanHistory('51c8d0dd60bd6056610e6af1dc39364c5b014f20');

for _,userinfo in pairs(UserHistory) do
    print('---')
        print(('License: %s'):format(userinfo.license));
        print(('Reason: %s'):format(userinfo.reason));
        print(('Author: %s'):format(userinfo.author));
        print(('On: %s'):format(userinfo.bannedOn));
        print(('Until: %s'):format(userinfo.bannedUntil));
    print('---')
end

-- output:
--    License: 51c8d0dd60bd6056610e6af1dc39364c5b014f20
--    Reason: Cheat
--    Author: Nishikoto
--    On: 21/12/2024 00:17:34
--    Until: 20/11/2024 13:47:34
```