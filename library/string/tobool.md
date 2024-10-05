---
description: >-
  Cette fonction permet simplement de transformer une variable "string" ou "number" en "boolean".
---

# Tobool

<detail>
  <summary>Logs</summary>

  Ajoutée en **v0.1.2**
</detail>

### Appel

{% code title="example.lua" %}
```lua
nlib.string.tobool(variable);
tobool(variable);
```
{% endcode %}

***

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
      <td>variable</td>
      <td align="center">string | number</td>
      <td></td>
    </tr>
  </tbody>
</table>

***

### Retours

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
            <td>boolean</td>
            <td align="center">boolean</td>
            <td>Variable transformé en boolean</td>
        </tr>
    </tbody>
</table>

***

### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local var1 = nlib.string.tobool('true');
local var2 = tobool(0);

print(var1); -- output: true
print(var2); -- output: false
```
{% endcode %}