---
description: >-
  Permet de bannir un utilisateur.
---

# BanUser

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
PrincessBan.BanUser(source, author, reason, time);
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
      <td>source</td>
      <td align="center">number</td>
      <td>ID de l'utilisateur à bannir</td>
    </tr>
    <tr>
      <td>author</td>
      <td align="center">string</td>
      <td>Nom de l'utilisateur qui banni</td>
    </tr>
    <tr>
      <td>reason</td>
      <td align="center">string</td>
      <td>Raison du bannissement</td>
    </tr>
    <tr>
      <td>time</td>
      <td align="center">table</td>
      <td>Temps de bannissement</td>
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
      <td>Permet de savoir si le joueur à été banni ou non</td>
    </tr>
  </tbody>
</table>

---

### Event

L'event sera déclencher dés qu'un joueur se fera bannir.

{% code title="server/example.lua" %}
```lua
AddEventHandler('PrincessBan:UserBanned', function(data)
    print('UserBanned');
    print(('License [%s]'):format(data.license));
    print(('Reason [%s]'):format(data.reason));
    print(('Author [%s]'):format(data.author));
    print(('Until [%s]'):format(data.date));
end);

-- output:
--   License [51c8d0dd60bd6056610e6af1dc39364c5b014f20]
--   Reason [Cheat]
--   Author [Nishikoto]
--   Until [21/12/2024 00:17:34]
```
{% endcode %}

---

### Utilisation

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanPlayer = PrincessBan.BanUser(1, 'Nishikoto', 'Cheat', {
  type = 'month', -- year | month | day | week | hour | minute
  time = 1 -- Mettre 0 ici, bannira l'utilisateur définitivement
});

if (BanPlayer) then
  print('User has been banned.');
end
```
{% endcode %}