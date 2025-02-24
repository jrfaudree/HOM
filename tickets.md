---
layout: course-page
title: Tickets
---

### Daily Materials

<div class="x-scroll">
<table class="asst-table">
<tr><th>Date</th><th>No.</th><th>Ticket</th><th>Worksheet</th></tr>
{% for c in site.data.ticket_s2025 %}
<tr valign="top">
  <td>
    {{ c.day }}
  </td>
  <td>
    {{ c.number }}
  </td>
  <td>
    <table class="inner">
      {% if c.ticket %}
      <tr>
         <td> <a href="{{ c.ticket }}">blank</a> </td>
      </tr>
      {% endif %}
      {% if c.tfilled %}
      <tr>
         <td> <a href="{{ c.tfilled }}">filled</a> </td>
      </tr>
      {% endif %}
    </table>
  </td>
  <td>
    <table class="inner">
      {% if c.worksheet %}
      <tr>
         <td> <a href="{{ c.worksheet }}">blank</a> </td>
      </tr>
      {% endif %}
      {% if c.wfilled %}
      <tr>
         <td> <a href="{{ c.wfilled }}">filled</a> </td>
      </tr>
      {% endif %}
    </table>
  </td>
</tr>
{% endfor %}
</table>
</div>
