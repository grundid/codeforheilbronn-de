---
layout: badge
name: Projektleiter
bid: "001"
tags: [aufgaben]
image: /uploads/badge-001-projektleiter.svg
color: rgb(255, 152, 0);
published: true
---

## Voraussetzungen

Dieser Badge wird für den erfolgreichen Abschluss eines Projektes verliehen.

* Ein abgeschlossenes Projekt
* Das Projekt muss dokumentiert sein
* Am Projekt müssen mindestens 2 weitere Personen mitgearbeitet haben

## Verliehen an

{% for contributor in site.data.contributors %}
    {% for ctr_badge in contributor.badges %}
        {% if (ctr_badge.id == page.bid) %}
            {% include cfh-contributor.html contributor=contributor.nick %}
        {% endif %}
    {% endfor %}
{% endfor %}
