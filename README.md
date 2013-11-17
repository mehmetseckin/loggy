 * Loggy
=======
 * Loggy is a basic class responsible from logging events and errors.
 * It writes down logs in a file called log.gy, and can also read the data,
 * and return a formatted version for you.
 *
 * Usage :
 * 
 * Create an instance, using the constructor. If you want to use 
 * a different filename and/or a different separator, pass them as parameters.
 * 
 *     - $loggy = new Loggy($myLogFile, $mySeparator);
 * 
 * Anywhere in your script, use the "w" method to write a new entry.
 * 
 *     - $loggy->w("This is a dummy log message", "Written by this Tag");
 * 
 * Loggy will automatically detect the IP address and pick the date and time
 * information, and add them into your log entry.
 * 
 * 
 * Exporting Loggy Entries :
 * 
 * Use the "export" method, which returns you the HTML formatted 
 * loggy data by default.
 * Export method takes a parameter that specifies what format do you want your
 * data in.
 * 
 *     - $myHTMLLogData = $loggy->export();
 *     - $myJSONLogData = $loggy->export("JSON");
 *     - $myXMLLogData  = $loggy->export("XML");

