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

{{site.software_name}} leverages the following technologies to help with your work:

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





## {{site.software_name}} code

Our repositories are at ((TODO list new repository locations and link to them)).

((TODO an overview of how the {{site.software_name}} code integrates at a high level. Low level documentation should be within ))

<section>

((TODO link to the github repos or documentation of key 3rd party libs like tatsypie, angular schema form etc))

We have a good deal of quality, well supported, open-source projects which are used within ShowYourWorking, as you can see.

Django and PostgreSQL provides the main ORM for saving, retrieving and modifying data.

Tastypie allows saving of non-ORM data and interaction with Elasticsearch and a more configurable web service architecture on top of Django.

Elasticsearch provides better searching of data through multiple indexes and flexible query language.

We use a system called Angular Schema form which allows definition of front end forms to be contained in JSON either on the front end or back end.





</section>

Detailed technical documentation is available within the wikis for these repositories. You can access an overview of these [here](https://github.com/thesgc/chembiohub_ws/wiki)

## {{site.software_name}} testing

((TODO outline our testing mechanism - Travis, Behave etc))

{{site.software_name}} utilises Behavioural Driven Development as the basis of its testing architecture. This is a semantically defined testing language which allows the creation of scenarios (to help with user story testing) and also reusable testing steps to validate end-to-end processes.

