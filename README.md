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
      post_id: int          # this will be auto-inferred as a link to post model

  $ pendolino -f appmodels.yml --out-type rails
  $ pendolino -f appmodels.yml --out-type appengine

This should create a scaffolded app taking models from the yaml.
Like in rails doing something like:

    rails generate scaffold post title:string description:text active:boolean
    rails generate scaffold comment body:text post_id:int

Thanks
======

Again, my mum for my great ideas.
And DHH for starting this first.