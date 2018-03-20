# Q0: Why is this error being thrown?
This error is being thrown because there is an uninitialized constant in the the Home Controller, specifically "Pokemon." The Pokemon controller has not been created yet.
# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
They were created from the seed file, which contained data on them, and appear based on the Home Controller creating a sample of trainerless_pokemon. They all appear to not have a trainer and are the starter Pokemon that the main characters of the show own, like Pikachu and Squirtle and the like.  

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
The following line creates a form which is a single button that goes to the capture method of the pokemon via the capture path, via a Patch type route.

# Question 3: What would you name your own Pokemon?
Snorsnack

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed in trainer_path in, which requires an id parameter. I passed in the id of the current trainer, which came from the button_to call in damage.

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
If the Create Pokemon fails, then the code will show the error thrown from validation and flash it as a sentence in my form.
# Give us feedback on the project and decal below!
This was a pretty difficult project, especially with the routes needing to be ordered a certain way to function properly and bcrypt bugs. However, I don't think I was able to learn the Week 4 and 5 materials too well because I was sick, and once I got the project working things seemed more clear. Potentially a check-in of some sort would have been helpful, as my pacing was poor due to sickness.  

# Extra credit: Link your Heroku deployed app
