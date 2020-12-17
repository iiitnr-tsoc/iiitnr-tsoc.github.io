---
title: Leaderboard
icon: fas fa-trophy
order: 5

# The About page
# v2.0
# https://github.com/cotes2020/jekyll-theme-chirpy
# © 2017-2019 Cotes Chung
# MIT License
---


<table>
  <thead>
    <tr>
      <th><strong>Name</strong></th>
      <th><strong>Karma</strong></th>
    </tr>
  </thead>
  <tbody>
  {% for row in site.data.leaderboard %}
    {% tablerow pair in row %}
    {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
  </tbody>
</table>
