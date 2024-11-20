---
description: >-
  Permet de débannir un utilisateur.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.UnbanUser(license, author);
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
      <td>License de l'utilisateur à débannir</td>
    </tr>
    <tr>
      <td>author</td>
      <td align="center">string</td>
      <td>Nom de l'auteur du débannissement</td>
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
      <td>Permet de savoir si le joueur à été débanni ou non</td>
    </tr>
  </tbody>
</table>

---

### Event

L'event sera déclencher dés qu'un joueur se fera débannir.

{% code title="server/example.lua" %}
```lua
AddEventHandler('PrincessBan:UserUnbanned', function(data)
    print('UserUnbanned');
    print(('License [%s]'):format(data.license));
    print(('Author [%s]'):format(data.author));
    print(('On [%s]'):format(data.date));
end);

-- output:
--   License [51c8d0dd60bd6056610e6af1dc39364c5b014f20]
--   Author [Nishikoto]
--   On [21/12/2024 00:17:34]
```
{% endcode %}

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanPlayer = PrincessBan.UnbanUser('51c8d0dd60bd6056610e6af1dc39364c5b014f20', 'Nishikoto);

if (BanPlayer) then
  print('User has been unbanned.');
end
```
{% endcode %}