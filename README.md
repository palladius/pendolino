pendolino
=========

this is a ruby/python project to generate RoR, Django, GAE application right from the data model.
It will have ruby-like generators to create scaffold for different languages.

Ideally you should have something like this:


# appmodels.yml
  posts:
    title: string
    description: text
    active:
      type: bool
      default: true
  comments:
    body: text
    post_id: string

  $ pendolino -f appmodels.yml --out-type rails
  $ pendolino -f appmodels.yml --out-type appengine


Thanks
======

Again, my mum for my great ideas.
