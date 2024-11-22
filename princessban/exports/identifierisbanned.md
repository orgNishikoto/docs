---
description: >-
  Find out if an identifier has been banned.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.IdentifierIsBanned(identifier);
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
      <td>identifier</td>
      <td align="center">string</td>
      <td>Identifier to be verified</td>
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
      <td>Returns whether the identifier is banned or not</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local IdentifierIsBanned = PrincessBan.IdentifierIsBanned('11000013df5ec2f');

if (IdentifierIsBanned) then
  print('Identifier is banned.');
end
```
{% endcode %}