---
description: >-
  Retrieves all exportable functions.
---

# GetObject

<details>
  <summary>Logs</summary>

  Added in **v1.0**
</details>

### Call

{% code title="server/example.lua" %}
```lua
local PrincessBan = exports['princessban']:GetObjectPrincessBan();
```
{% endcode %}

{% hint style="warning" %}
If you've renamed the script name, be sure to replace `princessban` with the name you've chosen.
{% endhint %}

{% hint style="warning" %}
Exports only work on the server side!
{% endhint %}

---

### Return

<table>
  <thead>
    <tr>
      <th width="82" align="center">Type</th>
      <th align="center">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">table</td>
      <td>Exportable functions</td>
    </tr>
  </tbody>
</table>