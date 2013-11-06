# TacoFancy API

Making an API for https://github.com/sinker/tacofancy

### Get a random taco

Go here: http://taco-randomizer.herokuapp.com/random/ to get a random Base Layer,
Mixin and (whenever someone adds some) a Shell. To get condiments or seasonings 
as well, append them as querystrings:

http://taco-randomizer.herokuapp.com/random/?condiments=true&seasonings=true

To just get a random full taco recipe, call it thusly:

http://taco-randomizer.herokuapp.com/random/?full-taco=true

### What’s next

Actually put some routes in the app that generate JSON and make this sucker 
queryable. 

### Want to help?

This whole this is a relatively rudimentary Flask setup. After you ``pip install``
the requirements, you should be able to run the ``prime_db.py`` and get a DB
together. The Flask app is looking for an environmental variable ``TACO_CONN`` to
tell it how to connect to the database. I developed this with sqlite but it should
work with anything that SQLAlchemy supports.

### TODO: Write more docs.
