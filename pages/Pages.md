---
title: Gestion des pages / Pages management
subject: La page actuellement affichée !
author: Plume WebMaster
tags: 
---

{% if user %}

Le  contenu  des  pages  est intégralement  accessible  sur  le  dépôt
[`{{  site.repository  }}`][plume-pages]  de  [GitHub][].  Chacun  est
invité  à  contribuer  pour  réparer  une erreur,  une  typo  ou  plus
généralement améliorer et enrichir nos pages.

La  syntaxe  retenue pour  les  éditer  est [Markdown][],  qui  permet
d'écrire facilement  des documents enrichis. Ce  format particulier de
syntaxe  `WikiWiki` présente  pour avantage  premier d'être  largement
répandu  (il a  aussi convaincu  les fondateurs  de `GitHub`  !). Mais
l'intérêt  principal, corollaire  immédiat de  sa popularité,  est son
inter-opérabilité.

Le source  de ces  pages est  accessible à  tous. Pour  contribuer, il
suffit de  s'incrire (gratuitement)  sur `GitHub`.  On peut  pour cela
utiliser  un des  multiples accès  proposés par  `OpenId`. Notre  site
utilise les  services de  [`{{ site.proseurl }}`][Prose].  Cela permet
d'oublier complètement toute la mécanique `Git` sous-jacente.

Retenez qu'un  nombre très limité (Patrick,  Colin, Filippo, Philippe)
sont  *collaborateurs*,  et à  ce  titre  opèrent directement  sur  le
contenu édité. Pour les autres  membres de l'équipe, leur contribution
sera *proposée* via `Prose` pour être intégrée au dépôt.

<div class="container-narrow">
  <div class="row-fluid">
    <div class="span10 offset1">
      <div class="news-head">/News</div>
  {% for page in routes %}
          <article class="post">
            <header>
              <h1><a href="/{{ site.url }}{{ page.url }}">{{ page.url }} - {{ page.title }}</a></h1>
              <div class="postmeta">
                <span class="date">{{ page.modified }}</span>
                <div class="clear"></div>
              </div>
            </header>
            <section class="content">
              {{ page.subject }}
            </section>
            <li class="post">
              <div class="row">
                <div class="col-sm-9">
                  <a class="revision-history" href="{{ page.history }}" target="_blank">historique</a>
                </div>
                <div class="col-sm-3 date">
                  <a class="btn btn-primary btn-small" href="{{ page.edit }}">éditer</a>
                </div>
              </div>
            </li>
          </article>
  {% endfor %}
    </div>
  </div>
</div>

{% else %}

Pages servies par ce site :

<div class="container-narrow">
  <div class="row-fluid">
    <div class="span10 offset1">
      <div class="news-head"></div>
          <ul>
  {% for page in routes %}
    {% if !page.reserved %}
            <li class="post">
              <div class="row">
                <div class="col-sm-9">
                  <a href="/{{ site.url }}{{ page.url }}">{{ page.url }} - {{ page.title }}</a>
                </div>
                <div class="col-sm-3 date">
                  {{ page.date | relative_datetime }}
                </div>
              </div>
            </li>
    {% endif %}
  {% endfor %}
          </ul>
    </div>
  </div>
</div>
{% endif %}

[plume-pages]: https://github.com/{{ site.repository }} (Contenu du site de l'équpe)
[GitHub]: https://github.com (Programmation et édition structurée, basé sur Git)
[Markdown]: http://fr.wikipedia.org/wiki/Markdown (Synthèse sur Markdown de WikiPedia)
[Prose]: http://prose.io (Édition, fingers in the nose, de contenu GitHub)
