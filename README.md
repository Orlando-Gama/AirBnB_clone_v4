0x06. AirBnB clone - Web dynamic

Tasks
0. Last clone!
mandatory
A new codebase again? Yes!

For this project you will fork this codebase:

Update the repository name to AirBnB_clone_v4
Update the README.md:
Add yourself as an author of the project
Add new information about your new contribution
Make it better!
If you’re the owner of this codebase, create a new repository called AirBnB_clone_v4 and copy over all files from AirBnB_clone_v3
If you didn’t install Flasgger from the previous project, it’s time! sudo pip3 install flasgger
1. Cash only
mandatory
Write a script that starts a Flask web application:

Based on web_flask, copy: web_flask/static, web_flask/templates/100-hbnb.html, web_flask/__init__.py and web_flask/100-hbnb.py into the web_dynamic folder
Rename 100-hbnb.py to 0-hbnb.py
Rename 100-hbnb.html to 0-hbnb.html
Update 0-hbnb.py to replace the existing route to /0-hbnb/
2. Select some Amenities to be comfortable!
mandatory
For the moment the filters section is static, let’s make it dynamic!

Replace the route 0-hbnb with 1-hbnb in the file 1-hbnb.py (based on 0-hbnb.py)

Create a new template 1-hbnb.html (based on 0-hbnb.html) and update it:
3. API status
mandatory
Before requesting the HBNB API, it’s better to know the status of this one.

Update the API entry point (api/v1/app.py) by replacing the current CORS CORS(app, origins="0.0.0.0") by CORS(app, resources={r"/api/v1/*": {"origins": "*"}}).

Change the route 1-hbnb to 2-hbnb in the file 2-hbnb.py (based on 1-hbnb.py)

Create a new template 2-hbnb.html (based on 1-hbnb.html) and update it:
4. Fetch places
mandatory
Replace the route 2-hbnb with 3-hbnb in the file 3-hbnb.py (based on 2-hbnb.py)

Create a new template 3-hbnb.html (based on 2-hbnb.html) and update it:

Import the JavaScript static/scripts/3-hbnb.js
5. Filter places by Amenity
mandatory
Replace the route 3-hbnb with 4-hbnb in the file 4-hbnb.py (based on 3-hbnb.py)

Create a new template 4-hbnb.html (based on 3-hbnb.html) and update it:

Import the JavaScript
6. States and Cities
#advanced
Now, reproduce the same steps with the State and City filter:

Replace the route 4-hbnb to 100-hbnb in the file 100-hbnb.py (based on 4-hbnb.py)

Create a new template 100-hbnb.html (based on 4-hbnb.html) and update it:

Import the JavaScript static/scripts/100-hbnb.js in the <head> tag (instead of 4-hbnb.js)
Add to all li tags of each state a new tag: <input type="checkbox">
Add to all li tags of each cities a new tag: <input type="checkbox">
The new checkbox must be at 10px on the left of the State or City name
Add to all input tags of each states (<li> tag) the attribute data-id=":state_id"
Add to all input tags of each states (<li> tag) the attribute data-name=":state_name"
Add to all input tags of each cities (<li> tag) the attribute data-id=":city_id"
Add to all input tags of each cities (<li> tag) the attribute data-name=":city_name"
Write a JavaScript script (static/scripts/100-hbnb.js):

Based on 4-hbnb.js
Listen to changes on each input checkbox tag:
if the checkbox is checked, you must store the State or City ID in a variable (dictionary or list)
if the checkbox is unchecked, you must remove the State or City ID from the variable
update the h4 tag inside the div Locations with the list of States or Cities checked
When the button tag is clicked, a new POST request to places_search should be made with the list of Amenities, Cities and States checked
7. Reviews
#advanced
Let’s add a new feature: show and hide reviews!

Replace the route 100-hbnb to 101-hbnb in the file 101-hbnb.py (based on 100-hbnb.py)

Create a new template 101-hbnb.html (based on 100-hbnb.html) and update it:

Import the JavaScript static/scripts/101-hbnb.js in the <head> tag (instead of 101-hbnb.js)
Design the list of reviews from this task
Add a span element at the right of the H2 “Reviews” with value “show” (add all necessary attributes to do this feature)
Write a JavaScript script (static/scripts/101-hbnb.js):

Based on 100-hbnb.js
When the span next to the Reviews h2 is clicked by the user:
Fetch, parse, display reviews and change the text to “hide”
If the text is “hide”: remove all Review elements from the DOM
This button should work like a toggle to fetch/display and hide reviews

