---
title: Decorators & Presenters
length: 90
tags: presenters, decorators, rails, refactoring, mvc
status: draft
---

## Learning Goals

* Understand the decorator pattern
* Practice rewriting helpers using a Draper decorator
* Understand the theory and purpose of a presenter object
* Practice creating a presenter to collect and wrap data

## Structure

* 30 - Lecture: Intro to Decorators
* 30 - Tutorial: Experimenting with Draper
* 15 - Lecture: Intro to Presenters
* 15 - Code: Creating a Dashboard Presenter

## Lecture: Intro to Decorators

First we'll discuss and experiment with decorators:

* The decorator pattern
* The idea and responsibilities of a "view model"
* Primer on Draper
* Work through an example

## Tutorial: Experimenting with Draper

Get together with your pair and [work through the tutorial](http://tutorials.jumpstartlab.com/topics/decorators.html).
If you get done with the core tutorial, then try out the bit at the end about
creating XML and JSON from your decorator.

## Lecture: Intro to Presenters

* One view, one controller, one action, one model?
* A presenter creates an abstraction across one or more models
* A presenter pretends to be a domain object
* No library needed -- just POROs!
* Example: creating a `Dashboard` presenter

## Code: Creating a Dashboard

Get back with your pair and implement a presenter for the Dashboard such
that the **only** instance variable in `views/dashboard/show.html.erb` is
`@dashboard`.

If you get that working, try creating a `DashboardDecorator`. What logic can
you pull out of the view template into the decorator?
