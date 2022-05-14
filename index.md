---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Portfolio
class: portfolio
permalink: /
---

<div class="wrapper">
    <h1 class="post-title">{{ page.title | escape }}</h1>
</div>

<div class="portfolio-content">


<div class="grid">
  <div class="grid-sizer"></div>
  <div class="grid-item">{% include image.html url="/assets/images/portfolio/Rembrandt.png" description="Personal Work; Rembrandt Master Study" %}</div>
  <div class="grid-item">{% include image.html url="/assets/images/portfolio/AB_Team.png" description="Personal Work; Poster of a DnD Campaign" %}</div>
  <div class="grid-item">{% include image.html url="/assets/images/portfolio/Doom.png" description="Personal Work; Esad Ribic Master Study" %}</div>
  <div class="grid-item">{% include image.html url="/assets/images/portfolio/awaken.png" description="Personal Work" %}</div>
  <div class="grid-item">{% include image.html url="/assets/images/portfolio/Nervous_System.png" description="Personal Work" %}</div>
<div class="grid-item">{% include image.html url="/assets/images/portfolio/Reichenbach.png" description="Commission; Illustration of a Reichenbach experiment" %}</div>
  <div class="grid-item grid-item--width2">{% include image.html url="/assets/images/portfolio/skatedeck001.png" description="Personal Work; Design for a skateboard deck" %}</div>
</div>

</div>

<script
  src="https://code.jquery.com/jquery-3.6.0.slim.min.js"
  integrity="sha256-u7e5khyithlIdTpu22PHhENmPcRdFiHRjhAuHcs05RI="
  crossorigin="anonymous"></script>
<script src="{{ "/assets/js/masonry.pkgd.min.js" | relative_url }}"></script>
<script src="{{ "/assets/js/imagesloaded.pkgd.min.js" | relative_url }}"></script>

<script>
var $grid = $('.grid').imagesLoaded( function() {
  // init Masonry after all images have loaded
    $('.grid').masonry({
        // set itemSelector so .grid-sizer is not used in layout
        itemSelector: '.grid-item',
        // use element for option
        columnWidth: '.grid-sizer',
        percentPosition: true
    });
});
</script>
