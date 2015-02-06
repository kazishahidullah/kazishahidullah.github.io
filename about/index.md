---
layout: page
title: <i class="fa fa-info-circle"></i>
subtitle: This page contains meta informations about me
permalink: /about/
#published: false
date: 2015-02-02 13:11
lastmodified: 2015-02-02 13:11
---

{% comment %}
<ul class="timeline-left">

  {% for year in site.data.timeline  %}
    <li><div class="timeline-badge success">{{year[0]}}</div></li>
    {% for item in year[1] %}
    <li>
      <div class="timeline-panel">
        <div class="timeline-heading">
          <h4 class="timeline-title">{{item.title}}</h4>
          <h6><i class="fa fa-clock-o"></i><time> {{item.date}} </time></h6>
        </div>
        <div class="timeline-body">{{item.desc | markdownify }}</div>
      </div>
    </li>
    {% endfor %}
  {% endfor %}

</ul>
{%endcomment%}



<div class="row">
  <div class="col-md-6">
    <div class="panel panel-primary ">
          <div class="panel-heading">
            <h3 class="panel-title">Contact Links</h3>
          </div>
          <div class="panel-body">
            {% for socialButton in site.data.personal.social %}
            <div class="col-xs-6 col-md-6 col-lg-6 social-btn-holder">
              <a class="btn btn-social btn-block {{ socialButton[1].btnClass }}" target="_BLANK" href="{{ socialButton[1].url }}">
                <i class="fa {{socialButton[1].logo}}"></i> {{ socialButton[1].text}} </a>
              </div>
              {% endfor %}
            </div>
          </div>
  </div>
  <div class="col-md-6">
    <div class="panel panel-primary">
          <div class="panel-heading">
            <h3 class="panel-title">About this site</h3>
          </div>
          <div class="panel-body">
              This site is built with:
              <ul class="">
                <li><a href="http://jekyllrb.com/"></a>Jekyll</li>
                <li>A <a target="_BLANK" href="https://github.com/itsrifat/rifyll">simple custom theme</a> built with Twitter Bootstrap by me</li>
              </ul>
          </div>
        </div>



  </div>
</div>
<div class="row">
  <div class="col-md-6">
    <div class="panel panel-primary">
      <div class="panel-heading">
        <h3 class="panel-title">To know a man is to know his playlist they say !</h3>
      </div>
      <div class="alert">
        Some of my favourites in random order as a spotify playlist
      </div>
      <div class="panel-body">

        <iframe src="https://embed.spotify.com/?uri=spotify:user:1297536437:playlist:2gR92avjtEB8uGmspofj6u"
        frameborder="0" allowtransparency="true" width="100%" height="400"></iframe>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="panel panel-primary">
      <div class="panel-heading">
        <h3 class="panel-title"> My attempt to cover few of my favourites </h3>
      </div>
      <div class="alert">
        Wanted to be a muscian when I was young, but failed miserably! These are the ashes left behind !
      </div>
      <div class="panel-body">

        <iframe width="100%" height="400" scrolling="no" frameborder="no" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/73338243%3Fsecret_token%3Ds-TLD7a&amp;color=ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false"></iframe>
      </div>
    </div>
  </div>
</div>
