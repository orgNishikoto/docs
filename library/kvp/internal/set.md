---
description: Permet de créer une kvp (en liaison avec le nom de votre script).
---

# Set

<details>

<summary>Logs</summary>

Ajoutée en **v0.1.2**

</details>

#### Appel

{% code title="example.lua" %}
```lua
nlib.kvp.internal.Set(name, value);
```
{% endcode %}

***

#### Paramètres

<table><thead><tr><th width="151" align="center">Paramètre</th><th width="79" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">name</td><td align="center">string</td><td align="center">Nom de la kvp</td></tr><tr><td align="center">value</td><td align="center">any</td><td align="center">Valeur de la kvp</td></tr></tbody></table>

***

#### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
nlib.kvp.internal.Set('mykvp_str', 'Hoj Guys');
-- If you want to get the KVP value, then it will return that: Hoj Guys
```
{% endcode %}
