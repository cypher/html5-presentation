!SLIDE

# Local Storage #

!SLIDE

	@@@ javascript
	sessionStorage.username = "John";
	console.log(sessionStorage.username);

!SLIDE

	@@@ javascript
	var database = openDatabase("DB Name",
	                            "DB Version");

	database.executeSql("SELECT * FROM test",
	  function(result1) {
	    // do something with the results
	    database.executeSql("DROP TABLE test",
	      function(result2) {
	        // do some more stuff
	        console.log("done!");
	   });
	});