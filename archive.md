---
layout: default
title: Archive
---

# Blog Archive
Novels

<li><a href="http://tornbranches.blogspot.co.nz/search/label/sci%20fi%20book%20review" target="_blank">Roadside Picnic by Arkady and Boris Strugatsky</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/a-canticle-for-leibowitz-by-walter-m.html" target="_blank">A Canticle for Leibowitz by Walter M Miller</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/05/where-to-for-star-trek-beyond.html" target="_blank">The Final Reflection by John M. Ford</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/09/why-i-hated-horus-rising-by-dan-abnett.html" target="_blank">Why I hated Horus Rising by Dan Abnett (some spoilers)</a></li>

Short stories and collections

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/book-review-three-moments-of-explosion.html" target="_blank">Three moments of an explosion by China Mieville&nbsp;</a></li>

Movies and Television

<li><a href="http://tornbranches.blogspot.co.nz/2016/07/jackrabbit-movie-review.html" target="_blank">Jackrabbit</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/05/captain-america-civil-war-review.html" target="_blank">Captain America: Civil War</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/05/film-review-shuen-by-philippe-mckie.html" target="_blank">Shuen by Philippe McKie</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/07/jackrabbit-movie-review.html" target="_blank">JackRabbit</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/think-new-zealand-genre-films-are-just.html" target="_blank">The&nbsp;Quiet Earth</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/psycho-pass-is-gripping-homage-to.html" target="_blank">Psycho Pass</a></li>

Ghost in the Shell - Let's watch

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/ghost-in-shell-stand-alone-complex-e01.html" target="_blank">Ghost in the Shell: Stand Alone Complex E01 Section 9</a></li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/06/ghost-in-shell-stand-alone-complex-e02.html" target="_blank">Ghost in the Shell: Stand Alone Complex E02 Runaway Evidence</a></li>
<li><a href="http://tornbranches.blogspot.co.nz/2016/06/ghost-in-shell-stand-alone-complex-e03.html" target="_blank">Ghost in the Shell: Stand Alone Complex E03 Android and I</a></li>
<li><a href="http://tornbranches.blogspot.co.nz/2016/07/ghost-in-shell-stand-alone-complex-e04.html" target="_blank">Ghost in the Shell: Stand Alone Complex E04 Interceptor</a></li>
<li><span id="goog_1218098820"></span><a href="https://tornbranches.blogspot.com/2016/08/ghost-in-shell-stand-alone-complex-e05.html" target="_blank">Ghost in the Shell: Stand Alone Complex E05 Decoy</a>&nbsp;<span id="goog_847014170"></span><a href="https://www.blogger.com/"></a><span id="goog_847014171"></span></li>
<li>Ghost in the Shell: Stand Alone Complex E06 Meme</li>

<li><a href="http://tornbranches.blogspot.co.nz/2016/08/ghost-in-shell-stand-alone-complex-e07.html" target="_blank">Ghost in the Shell: Stand Alone Complex E07 Idolator</a></li>
<li><a href="http://tornbranches.blogspot.co.nz/2016/09/ghost-in-shell-stand-alone-complex-e08.html" target="_blank">Ghost in the Shell: Stand Alone Complex E08 Missing Hearts</a></li>
<li><a href="http://tornbranches.blogspot.co.nz/2016/10/ghost-in-shell-stand-alone-complex-e09.html" target="_blank">Ghost in the Shell: Stand Alone Complex E09 CHAT! CHAT! CHAT!</a></li>
<li><a href="http://tornbranches.blogspot.co.nz/2016/10/ghost-in-shell-stand-alone-complex-e10.html" target="_blank">Ghost in the Shell: Stand alone complex E10 Jungle Cruise</a></li>

{% assign posts_by_year = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}

{% for year_group in posts_by_year %}
  <h2>{{ year_group.name }}</h2>
  <ul>
    {% for post in year_group.items %}
      <li>
        <span class="post-meta">{{ post.date | date: "%B %d" }}</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}
