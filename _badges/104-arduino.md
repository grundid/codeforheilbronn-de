---
layout: badge
name: Projektleiter
bid: "104"
tags: [aufgaben]
image: /uploads/badge-104-arduino.svg
color: rgb(96, 125, 139);
published: true
---

## Voraussetzungen

Dieser Badge wird für ein abgeschlossenes und dokumentiertes Arduino-Projekt verliehen.

* Das Projekt muss die Arduino-Library nutzen und einen kompatiblen Microcontroller.
* Das Projekt muss abgeschlossen (Projektziel erfüllt) sein.
* Das Projekt muss auf codeforheilbronn.de dokumentiert sein.
* Der Quellcode muss auf Github veröffentlicht werden.

## Verliehen an

{% for contributor in site.data.contributors %}
    {% for ctr_badge in contributor.badges %}
        {% if (ctr_badge.id == page.bid) %}
            {% include cfh-contributor.html contributor=contributor.nick %}
        {% endif %}
    {% endfor %}
{% endfor %}
