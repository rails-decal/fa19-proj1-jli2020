# Q0: Why are these two errors being thrown?
The first error is thrown because the pending migrations exist, and the database schema is not up to date. The second error is thrown because the Pokemon model hasn't been created yet. 
# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
The random Pokemon appear from the rails db:seed command, which populates the database with pokemon in the seeds file.  
# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
It creates a button that prompts the user to throw a pokeball and capture it. It then grabs the current pokemon object and reads in its id, and directs it to the capture path, which in turn directs it to the capture method in the Pokemon controller. 
# Question 3: What would you name your own Pokemon?
Shannon
# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed in request.referrer. It is okay not to have a path because you are just refreshing to the previous page/URL, which is the desired trainer profile page.
# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.

# Give us feedback on the project and decal below!

# Extra credit: Link your Heroku deployed app
