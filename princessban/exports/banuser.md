---
description: >-
  Allows you to ban a user.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.BanUser(source, author, reason, time);
```
{% endcode %}

---

### Parameters

<table>
  <thead>
    <tr>
      <th width="151" align="center">Parameter</th>
      <th width="79" align="center">Type</th>
      <th align="center">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>source</td>
      <td align="center">number</td>
      <td>ID of the user to be banned</td>
    </tr>
    <tr>
      <td>author</td>
      <td align="center">string</td>
      <td>Name of banning user</td>
    </tr>
    <tr>
      <td>reason</td>
      <td align="center">string</td>
      <td>Reason for ban</td>
    </tr>
    <tr>
      <td>time</td>
      <td align="center">table</td>
      <td>Banning time</td>
    </tr>
  </tbody>
</table>

---

### Return

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
      <td>Find out if the player has been banned or not</td>
    </tr>
  </tbody>
</table>

---

### Event

The event will be triggered as soon as a player is banned.

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

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanPlayer = PrincessBan.BanUser(1, 'Nishikoto', 'Cheat', {
  type = 'month', -- year | month | day | week | hour | minute
  time = 1 -- Setting 0 here will ban the user permanently
});

if (BanPlayer) then
  print('User has been banned.');
end
```
{% endcode %}