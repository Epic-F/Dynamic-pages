PHP-Dynamic-pages
=================



This project helps you to include the pages dynamically, very simple to use. Just upload the files to your directory 
edit the index.inc.php files (located in app/views/<page that is requested>) and you are ready to go.

Live Demo: http://hub.gitcloud.nl/Dynamic/

How to request a page? 
When the files are on your server, go to index.php?page=home (this will load the app/views/home/index.inc.php file).


Add an extra page? 
Open the routes.inc.php file (located in app/ folder), and edit:
	
		<?php
		$pages = array('index', 'home', 'about', 'contact');
		
		?>
For example you want to add a "privacy" page, just add this: 

		<?php
		$pages = array('index', 'home', 'about', 'contact', 'privacy');
		
		?>

then go to "app/views/" and add a folder named "privacy", in the folder you need to create the file "index.inc.php", and you are done!

Have questions? Email me!
