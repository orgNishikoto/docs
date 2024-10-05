---
description: Permet de connaître le type d'une variable.
---

# type

{% hint style="warning" %}
Attention: J'ajoute' uniquement le fait voir le type 'float' d'un nombre, donc oui il est possible de voir les autres type avec cette fonction.

C'est pour cela que je n'ai pas remplacé la fonction native `type()` de lua.
{% endhint %}

## Get

<details>

<summary>Logs</summary>

Ajoutée en **v0.1.2**

</details>

#### Appel

{% code title="example.lua" %}
```lua
nlib.string.type(variable);
```
{% endcode %}

***

#### Paramètres

\=

<table><thead><tr><th width="151" align="center">Paramètre</th><th width="96" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">variable</td><td align="center">any</td><td align="center"></td></tr></tbody></table>

***

#### Retours

<table><thead><tr><th width="190" align="center">Variable</th><th width="82" align="center">Type</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">type</td><td align="center">string</td><td align="center">Le type de la variable envoyé.</td></tr></tbody></table>

***

#### Utilisation

{% code title="example.lua" lineNumbers="true" %}
```lua
local whatismynumber = 8.9;
local typeof = nlib.string.type(whatismynumber);

print(typeof); -- output: float
```
{% endcode %}
