---
description: >-
  Find out if a user has been banned.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.UserIsBanned(license);
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
      <td>User license to be verified</td>
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
      <td>Returns whether the user is banned or not</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local UserIsBanned = PrincessBan.UserIsBanned('51c8d0dd60bd6056610e6af1dc39364c5b014f20');

if (UserIsBanned) then
  print('User is banned.');
end
```
{% endcode %}