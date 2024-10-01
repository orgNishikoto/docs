---
description: >-
  Ce fichier contient tout les logs disponible et qui peuvent être écrit dans la console.
---

# Console

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.0**
</details>

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
      <td>...args</td>
      <td align="center">any</td>
      <td></td>
    </tr>
  </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.console.err('Your error message');
nlib.console.log('Your log message');
nlib.console.print('Basic print of lua');
nlib.console.success('Your success message');
nlib.console.warn('Your warning message');
```
{% endcode %}

![console-prints](../../assets/snippets/console-prints.png)

{% hint style="info" %}
Tips: **nlib.console** peut être remplacé par **console**
{% endhint %}