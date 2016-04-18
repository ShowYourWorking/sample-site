---
layout: page
root: ..
title: Develop
---

These pages contain information on how to develop
{{ site.software_name }}. This include accessing the source code,
development tools, test tools, how to develop components, how to
write tests, coding standards, and release process.

* [Technical Documentation Wiki](https://github.com/thesgc/chembiohub_ws/wiki)
* [Angular API](../docs/) (beta - under development)
* [Repositories on GitHub](http://github.com/showyourworking)

## ShowYourWorking code

Our repositories are located [on GitHub](http://github.com/showyourworking).

{{ site.software_name }} is built on Django, the Python CMS. You can find out more information on Django here. {{ site.software_name }} currently uses version 1.7 of Django, with Python version 2.7.

{{ site.software_name }} currently uses Angular v1.3 for the user interface. An API of all the code used within the app is viewable [here](../docs/)

Django is used primarily to provide a web service architecture for the applications and the user and login functionality. Django was primariliy selected for this purpose because of its open source nature, written in the Python programming language for interaction with chemically-aware software such as RDKit via ChEMBL's web service architecture and also with existing python tools for integrating with the University of Oxford's WebAuth single sign on system.

{{ site.software_name }} installation scripts preconfigure a number of backend services including Redis, PostgreSQL, Elasticsearch etc. More details can be found on the [Running the python server and database in production] page

By default, login is handled by the django login system.

We also include and example custom deployment of {{ site.software_name }} where the login credentials are checked in python against a different internal database.

As the system is built with Django, theoretically any of the login mechanisms supported by django could be integrated. Please raise a ticket if you have interest in this. We have integrated the login parts of our application with University of Oxford's WebAuth system but this is not included in the default install listed here.

Detailed technical documentation is available within the wikis for these repositories. You can access an overview of these [here](https://github.com/thesgc/chembiohub_ws/wiki)

There are a good deal of quality, well supported, open-source projects used within ShowYourWorking, as you can see from the [Technologies list](#technologies) on this page. 

* Django and PostgreSQL provides the main ORM for saving, retrieving and modifying data.

* Tastypie allows saving of non-ORM data and interaction with Elasticsearch and a more configurable web service architecture on top of Django. 

* Elasticsearch provides better searching of data through multiple indexes and flexible query language. 

* We use a system called Angular Schema form which allows definition of front end forms to be contained in JSON either on the front end or back end.

Detailed technical documentation is available within the wikis for these repositories. You can access an overview of these [here](https://github.com/thesgc/chembiohub_ws/wiki)

## ShowYourWorking testing

{{site.software_name}} utilises Behavioural Driven Development as the basis of its testing architecture. This is a semantically defined testing language which allows the creation of scenarios (to help with user story testing) and also reusable testing steps to validate end-to-end processes.

{{site.software_name}} utilises Travis continual integration platform ((TODO will there be a ShowYourWorking-specific Travis installation anywhere? Or an SGC one?))

## Technologies

{{site.software_name}} leverages the following technologies to help with your work:

<img src="/assets/images/tech_stack/overview.png">

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

