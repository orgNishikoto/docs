---
description: >-
  Used to unban an identifier.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.UnbanIdentifierByLicense(license);
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
      <td>License of the banned user</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="server/example.lua" lineNumbers="true" %}
```lua
local UnbanIdentifier = PrincessBan.UnbanIdentifierByLicense('51c8d0dd60bd6056610e6af1dc39364c5b014f20');

if (UnbanIdentifier) then
  print('Identifier has been unbanned.');
end
```
{% endcode %}