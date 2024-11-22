---
description: >-
  Find out the version of a GitHub repository (public).
---

# Get

<details>
  <summary>Logs</summary>

  Added in **v0.1.0**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.version.get(username, reponame, truncate);
```
{% endcode %}

***

### Parameters

<table>
    <thead>
        <tr>
            <th width="151" align="center">Parameter</th>
            <th width="79" align="center">Type</th>
            <th align="center">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>username</td>
            <td align="center">string</td>
            <td>Name of github user or github organization</td>
        </tr>
        <tr>
            <td>reponame</td>
            <td align="center">string</td>
            <td>Name of github repository or github organization</td>
        </tr>
        <tr>
            <td>truncate</td>
            <td align="center">boolean</td>
            <td>Display full version name (fork-x.x.x) or cut version name (x.x.x)</td>
        </tr>
    </tbody>
</table>

***

### Return

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
            <td>version</td>
            <td align="center">string</td>
            <td>Version of selected GitHub repository</td>
        </tr>
    </tbody>
</table>

***

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local version_truncate = nlib.version.compare('orgNishikoto', 'library', true);
local version_notruncate = nlib.version.compare('orgNishikoto', 'library', false);

if (version_truncate and version_notruncate) then
    print(version_truncate); -- output: fork-alpha-0.1.0
    print(version_notruncate); -- output: 0.1.0
end
```
{% endcode %}

{% hint style="info" %}
**Tips**: Make sure you don't get “rate-limited” by the Github API. (Max 60 requests)
{% endhint %}