---
layout: page
root: ..
title: Develop
---

These pages contain information on how to develop
{{ site.software_name }}. This include accessing the source code,
development tools, test tools, how to develop components, how to
write tests, coding standards, and release process.

* [Coding standards](./CodingStandards.html)

## Technologies

ShowYourWorking leverages the following technologies to help with your work:

<img src="/assets/images/tech_stack/overview.png">

((TODO technology stack here))

<section class="tech-stack" id="tech-stack">

{% for section in site.techstack %}

<h3>{{section.title}}</h3>

{% for item in section.items %}

<div id="{{item.id}}" class="tech-stack-item">
<div class="row">
  <div class="col-xs-3"><img src="/assets/images/tech_stack/{{item.id}}.png" class="img img-responsive"></div>
  <div class="col-xs-9"><p><a href="{{item.link}}">{{item.name}}</a><br>{{item.description}}</p></div>
</div>
</div>

{% endfor %}

{% endfor %}

</section>

((TODO Any further explanation of these here))

((TODO link to the github repos or documentation of key 3rd party libs like tatsypie, angular schema form etc))

## ShowYourWorking code

Our repositories are at ((TODO list new repository locations and link to them)).

((TODO an overview of how the ShowYourWorking code integrates at a high level. Low level documentation should be within ))

Detailed technical documentation is available within the wikis for these repositories.

## ShowYourWorking testing

((TODO outline our testing mechanism - Travis, Behave etc))


