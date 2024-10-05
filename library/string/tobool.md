---
description: >-
  Cette fonction permet simplement de transformer une variable "string" ou
  "number" en "boolean".
---

# tobool

Logs

Ajoutée en **v0.1.2**

#### Appel

{% code title="example.lua" %}
```lua
nlib.string.tobool(variable);
tobool(variable);
```
{% endcode %}

***

#### Paramètres

<table><thead><tr><th width="151" align="center">Paramètre</th><th width="176" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">variable</td><td align="center">string | number</td><td align="center"></td></tr></tbody></table>

***

#### Retours

<table><thead><tr><th width="179" align="center">Variable</th><th width="120" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">boolean</td><td align="center">boolean</td><td align="center">Variable transformé en boolean</td></tr></tbody></table>

***

#### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local var1 = nlib.string.tobool('true');
local var2 = tobool(0);

print(var1); -- output: true
print(var2); -- output: false
```
{% endcode %}
