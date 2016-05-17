---
layout: page
root: ..
title: Develop
---

These pages contain information on how to develop
{{ site.software_name }}. This include accessing the source code,
development tools, test tools, how to develop components, how to
write tests, coding standards, and release process.

---

## Docs

The main developer documentation is hosted on GitHub.

<a href="https://github.com/thesgc/chembiohub_ws/wiki">**Click Here for Developer Documentation**</a>

* <a href="#what">What is ShowYourWorking</a>
* <a href="#why">What problem does ShowYourWorking solve?</a>
* <a href="#how">How can I get ShowYourWorking?</a>
* <a href="#howuse">How do I run and use ShowYourWorking?</a>
* <a href="#trouble">My installation is not working, what should I do?</a>
* <a href="#dev">I would like to develop a new feature for ShowYourWorking</a>


###<a name="what">What is ShowYourWorking</a>

ShowYourWorking develops in-house applications and provides links to a variety of useful tools which can help chemical biologists, related scientists and support staff.

The ShowYourWorking platform is designed to accommodate a wide range of data - from chemical data (ChemiReg) to more generic collection and inventory data (InventoryReg) or any other simple tabular data format.

###<a name="why">What problem does ShowYourWorking solve?</a>

ShowYourWorking helps researchers search and manage their data including experimental data but also other data from the processes going on in labs such as keeping track of what is in stock.

###<a name="how">How can I get ShowYourWorking?</a>

ShowYourWorking is open-source software. If using the Chemical features it is under a GPL v3 license.

See [[Installation]] documentation here

###<a name="howuse">How do I run and use ShowYourWorking?</a>

To configure your installation see [[Getting started once installed]].

For information on how to back-up and similar tasks, see the [[Systems Administration]] page

End user documentation is located on our [project site](http://showyourworking.github.io/user/index.html
).


###<a name="trouble">My installation is not working, what should I do?</a>

We have gathered some common errors in our [[Troubleshooting]] page. If you still have a problem, feel free to raise a [github issue](https://github.com/thesgc/chembiohub_ws/issues) and we will try to get back to you.

###<a name="dev">I would like to develop a new feature for ShowYourWorking</a>

ShowYourWorking was developed to be extendible both in the front end and back end using a combination of AngularJS and Python Django.

The way the features work and how to set up a development environment is described in the [[Technical guide and how to extend]] page. If you have a problem using these docs, feel free to raise a [github issue](https://github.com/thesgc/chembiohub_ws/issues) and we will try to get back to you.

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

<!-- {% for section in site.techstack %}

<h3>{{section.title}}</h3>

{% for item in section.items %}

<div id="{{item.id}}" class="tech-stack-item">
<div class="row">
  <div class="col-xs-3"><img src="/assets/images/tech_stack/{{item.id}}.png" class="img img-responsive"></div>
  <div class="col-xs-9"><p><a href="{{item.link}}">{{item.name}}</a><br>{{item.description}}</p></div>
</div>
</div>

{% endfor %}

{% endfor %} -->

</section>

