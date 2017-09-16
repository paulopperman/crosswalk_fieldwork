## a web application for logging of pedestrian crossings and sidewalks ##

### objectives ###
* log data to a human-friendly spreadsheet, rather than a database
* present choices to a user based off of existing rows from the spreadsheet
* use technologies that can run on a mobile browser
* (possibly) allow for real-time collaboration

### technologies, tutorials used ###
#### spreadsheet "backend" ####
* [access a Google spreadsheet using their API](https://www.twilio.com/blog/2017/03/google-spreadsheets-and-net-core.html)

#### web server ####
* [Python language](https://www.python.org/)
* [Flask web framework](http://flask.pocoo.org/)
* [Flask SocketIO integration library](http://flask-socketio.readthedocs.io/en/latest/)
* ["gspread" library for accessing spreadsheet](http://gspread.readthedocs.io/en/latest/)

#### web client ####
* [modern Javascript](https://javascript.info/)
* [JQuery](http://jquery.com/)
* [SocketIO](https://socket.io/)
* [Leaflet](http://leafletjs.com/)
* [Leaflet Icon.Glyph](https://github.com/Leaflet/Leaflet.Icon.Glyph)
* [Font Awesome](http://fontawesome.io/icons/)
* [Leaflet Marker-Cluster](https://github.com/Leaflet/Leaflet.markercluster)

### deployment ###

### gotchas ###
can't think of a good way to force the server to mark the backend as "dirty" and re-fetch it (i.e. if someone manually updates the spreadsheet). working thought right now is to add a script to the spreadsheet to call a "refresh" URL.
