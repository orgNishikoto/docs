---
description: >-
  This log is a bit special: it's only displayed if the convar
  'nishikoto:library:debug' is active (set to 'true').
---

# Debug

<details>
  <summary>Logs</summary>

  Added in **v0.1.0**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.console.debug(eLevel, message);
```
{% endcode %}

---

### Parameters

<table>
  <thead>
    <tr>
      <th align="center">Parameter</th>
      <th width="79" align="center">Type</th>
      <th align="center">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">eLevel</td>
      <td align="center">string</td>
      <td align="center">Debug error level</td>
    </tr>
    <tr>
      <td align="center">message</td>
      <td align="center">string</td>
      <td align="center">Debug message</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.console.debug(nlib.enum.eLevel.Fatal, 'Coucou');
```
{% endcode %}

<div align="left" data-full-width="false">
  <img src="../../assets/snippets/console-debug-fatal.png" alt="console-debug-fatal" width="231">
</div>
