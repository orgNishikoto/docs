---
description: >-
  Compares the version of your script with the version of the latest
  release of a (public) GitHub repository.
---

# Comparaison

<details>
  <summary>Logs</summary>

  Added in **v0.1.0**
</details>

### Call

{% code title="example.lua" %}
```lua
nlib.version.compare(username, reponame, version);
```
{% endcode %}

---

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
      <td>Name of github repository</td>
    </tr>
    <tr>
      <td>version</td>
      <td align="center">string</td>
      <td>Version of your script</td>
    </tr>
  </tbody>
</table>

---

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
      <td align="center">lower | upper | equal | error</td>
      <td align="center">string</td>
      <td>Comparison status</td>
    </tr>
  </tbody>
</table>

---

### Use

{% code title="example.lua" lineNumbers="true" %}
```lua
local status = nlib.version.compare('orgNishikoto', 'library', '0.1.0');

if (status) then 
    print(status); -- output: equal
end
```
{% endcode %}

{% hint style="info" %}
**Tips**: Make sure you don't get “rate-limited” by the Github API. (Max 60 requests)
{% endhint %}