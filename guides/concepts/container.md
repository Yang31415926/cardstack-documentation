I was going to say that the Cardstack backend uses something very similar to the Ember container but after having a quick look in the @cardstack/di package you can see that the Cardstack Container and Registry actually extend the Glimmer Container and Registry 😂 This means that if you have a type defined in the system you can get access to it using something like `env.lookup('hub:searchers')` which would get all the `searchers` registered in the system.