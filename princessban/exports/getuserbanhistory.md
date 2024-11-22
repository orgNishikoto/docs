---
description: >-
  Allows you to view a user's banning history.
---

# BanUser

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
PrincessBan.GetUserBanHistory(license);
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
      <td align="center">table</td>
      <td align="center">table</td>
      <td>List of user information</td>
    </tr>
  </tbody>
</table>

---

### Use

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
{% endcode %}