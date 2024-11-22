---
description: >-
  Enables a user to be unbanned.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.UnbanUser(license, author);
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
      <td>license</td>
      <td align="center">string</td>
      <td>User license to be debugged</td>
    </tr>
    <tr>
      <td>author</td>
      <td align="center">string</td>
      <td>Name of author of troubleshooting</td>
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
      <td align="center">true | nil</td>
      <td align="center">boolean | nil</td>
      <td>Indicates whether the player has been debriefed or not</td>
    </tr>
  </tbody>
</table>

---

### Event

The event will be triggered as soon as a player is unannounced.

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

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanPlayer = PrincessBan.UnbanUser('51c8d0dd60bd6056610e6af1dc39364c5b014f20', 'Nishikoto');

if (BanPlayer) then
  print('User has been unbanned.');
end
```
{% endcode %}