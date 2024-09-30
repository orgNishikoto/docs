# Installation


## Dépendance

La bibliothèque [lib](https://github.com/JustGodWork/lib/releases/latest) est obligatoire pour faire fonctionner Library.
- Cliquez [ici](https://github.com/JustGodWork/lib/blob/main/README.md#getting-started) pour suivre les étapes d'installation de la bibliothèque lib

## Installation
{% tabs %}

{% tab title="Manuellement" %}
- Téléchargez la dernière [release](https://github.com/orgNishikoto/library/releases/latest)
- Ajoutez `ensure library` dans votre fichier `server.cfg` ou `resource.cfg`

{% hint style="info" %}
Tips: Démarrez la resource **library** avant vos resources personnel
{% endhint %}

{% hint style="info" %}
La suite est une intégration uiquement pour vos resource personnel, dans mes scripts la bibliothèque est déjà appelé.
{% endhint %}

{% code title="fxmanifest.lua" overflow="" lineNumbers="true" %}
```lua
shared_scripts {
    '@lib/imports.lua',
    '@library/imports.lua'
} 
```
{% endcode %}
{% endtab %}

{% tab title="Git" %}
{% code title="" overflow="" lineNumbers="false" %}
```
git clone https://github.com/orgNishikoto/library.git
```
{% endcode %}
{% endtab %}

{% endtabs %}