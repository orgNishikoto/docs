---
description: >-
  Ce log est un peu particulier, il s'affiche uniquemnt si la convar 'nishikoto:library:debug' est active (sur 'true').
---

# Debug

<details>
  <summary>Logs</summary>

  Ajoutée en **v0.1.0**
</details>

### Appel

{% code title="example.lua" %}
```lua
nlib.console.debug(eLevel, message);
```
{% endcode %}

---

### Paramètres

<table>
  <thead>
    <tr>
      <th wigth="151" align="center">Paramètre</th>
      <th width="79" align="center">Type</th>
      <th align="center">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>eLevel</td>
      <td align="center">string</td>
      <td>Level d'erreur du debug</td>
    </tr>
    <tr>
      <td>message</td>
      <td align="center">string</td>
      <td>Message de debug</td>
    </tr>
  </tbody>
</table>

---

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.console.debug(nlib.enum.eLevel.Fatal, 'Coucou');
```
{% endcode %}

![console-debug-fatal](../../assets/snippets/console-debug-fatal.png)