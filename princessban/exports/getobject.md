---
description: >-
  Permet de récuperer tout les fonctions exportable.
---

# GetObject

<details>
  <summary>Logs</summary>

  Ajoutée en **v1.0**
</details>

### Appel

{% code title="server/example.lua" %}
```lua
local PrincessBan = exports['princessban']:GetObjectPrincessBan();
```
{% endcode %}

{% hint style="warning" %}
Si vous avez renomé le nom du script, veillez à rempacé `princessban` par le nom que vous avez choisis.
{% endhint %}

{% hint style="warning" %}
Les exports fonctionne uniquement côté serveur!
{% endhint %}

---

### Retours

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
      <td>Fonctions exportable</td>
    </tr>
  </tbody>
</table>