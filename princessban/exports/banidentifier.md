---
description: >-
  Allows you to ban an identifier.
---

# BanIdentifier

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.BanIdentifier(license, identifier);
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
      <td>User license</td>
    </tr>
    <tr>
      <td>identifier</td>
      <td align="center">string</td>
      <td>Ban username</td>
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
      <td>Finds out whether the user has been banned or not</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local BanIdentifier = PrincessBan.BanIdentifier('51c8d0dd60bd6056610e6af1dc39364c5b014f20', '11000013df5ec2f');

if (BanIdentifier) then
  print('Identifier has been banned.');
end
```
{% endcode %}