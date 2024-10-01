---
icon: down-to-bracket
---

# Installation

## Dépendance

La bibliothèque [lib](https://github.com/JustGodWork/lib/releases/latest) est obligatoire pour faire fonctionner Library.

* Cliquez [ici](https://github.com/JustGodWork/lib/blob/main/README.md#getting-started) pour suivre les étapes d'installation de la bibliothèque lib

## Installation

{% tabs %}
{% tab title="Manuellement" %}
* Téléchargez la dernière [release](https://github.com/orgNishikoto/library/releases/latest)
* Ajoutez `ensure library` dans votre fichier `server.cfg` ou `resource.cfg`
* Copiez le contenu du fichier `convars.cfg` (inclu dans la bibliothèque) dans votre fichier `server.cfg` ou `resource.cfg`

{% hint style="info" %}
Tips: Démarrez la resource **library** avant vos resources personnelle
{% endhint %}

{% hint style="info" %}
La suite est une intégration uniquement pour vos resources personnelle, dans mes scripts la bibliothèque est déjà appelée.
{% endhint %}

{% code title="fxmanifest.lua" lineNumbers="true" %}
```lua
shared_scripts {
    '@lib/imports.lua',
    '@library/imports.lua'
} 
```
{% endcode %}
{% endtab %}

{% tab title="Git" %}
{% code title="" lineNumbers="true" %}
```
git clone https://github.com/orgNishikoto/library.git
```
{% endcode %}
{% endtab %}
{% endtabs %}
