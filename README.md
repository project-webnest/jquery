[jQuery](http://www.jquery.com) Version Control
======================================================

This project contains every version of jQuery (from 1.2.6 and up) with version control implemented on it.


How to use jQuery with these modifications
------------------------------------------
The global jQuery object is now just an object instead of a function, with key value pairs mapping each version number
to it's jQuery function. For anonymous workspaces, code setup should be like below.

	(function( $ ) {
		// $ now references the jQuery-1.4.2 object
	})( jQuery['1.4.2'] )

Or to use it directly for document ready workspaces -

	jQuery['1.4.2'](function( $ ) {
		// $ now references the jQuery-1.4.2 object
	});
