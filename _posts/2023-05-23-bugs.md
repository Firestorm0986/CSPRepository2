---
toc: true
comments: true
layout: post
title: Bugs
description: bugs
categories: []
image: images/bugs.png
---

<button onclick="startAnimation()">Start Animation</button>

{% assign sprite_file = site.baseurl | append: page.image %}
{% assign bugs = site.data.bugs %}

<div class="container">
  {% for bug in bugs %}
    {% assign id = bug.id %}
    <div class="column">
      <p class="sprite" id="{{id}}">{{id}}</p>
    </div>
  {% endfor %}
</div>

<style>
  .sprite {
    background-image: url('{{ sprite_file }}');
    background-repeat: no-repeat;
    height: 100px;
    width: 100px;
    font-size: 2em;
    text-align: center;
  }

  {% for bug in bugs %}
    {% assign id = bug.id %}
    #{{id}} {
      background-position: calc({{bug.col}} * 100% * -1px) calc({{bug.row}} * 100% * -1px);
    }
  {% endfor %}
</style>

<script>
  var intervalIDs = {};

  function startAnimation() {
    {% for bug in bugs %}
      var id = "{{bug.id}}";
      var row = {{bug.row}};
      var col = {{bug.col}};
      var frames = {{bug.frames}};

      var colOffset = col * 100;

      intervalIDs[id] = setInterval(() => {
        var currentFrame = col % frames;
        var backgroundPositionX = (currentFrame * 100) - colOffset;

        document.getElementById(id).style.backgroundPosition = `${backgroundPositionX}px calc(${row * 100}% * -1)`;

        col++;
      }, 200);
    {% endfor %}
  }
</script>
