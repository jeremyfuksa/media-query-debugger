# media-query-debugger
===================

A quick, lightweight jQuery plugin used for keeping track of the responsive breakpoints you're working with.

## USAGE
===================

1. Link to css/media-query-debugger.css or copy/paste the .mq-debug class into your master stylesheet.
2. Place an empty <div> right after the <body> tag and give it a unique ID.
3. Include js/jquery.media-query-debugger.js just before the </body> tag.
4. Place the following function right after the linked plugin (where "#debugger" is replaced by your unique ID):

	<script>
		$(document).ready(function(){
			$('#debugger').mqDebug();
			$(window).resize(function(){
				$('#debugger').mqDebug();
			});
		});
	</script>

You should now have a small badge that floats above your entire design that displays your current breakpoint every time it is resized.