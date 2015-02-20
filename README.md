# MVC-Data-Handler
Data validater &amp; manager across MVC tool to setup working with simple objects and relations

			[[Client]]
View
	HTML & Javascript
		Validate input from text boxes
		Specify how values should be displayed
		Specify links between objects

			[[Server]]
Modal
	PHP || Other
		Validate and sanatize all input from client
		Encode & Decode html syntax
		Easily perform CRUD operations
		Ensure data is processed before saving into DB

			[[Data]]
Controller
	MySQL || Other DB
		Easily create objects that are relateable
		and conform to db normalization
		
[[Overall]]
	What we want is a simple syncronized way of working with simple objects and relations
	The object will be considered to be of the following form
		An Object has
			A id {integer} 1
			A Name {String} 1
			A Description {String} 1
			Properties {Array} *
				Properties are
					Columns in a table
					Array within the second layer of an associative array in PHP
					An associative array within the JSON object in JS 
			Relationships {Object_ids} *
		An Object is a
			Table within the DB
			Array within the first layer of an associative array in PHP
			An JSON object with an associative name in JS
	The database will normally be in 2nd NF
