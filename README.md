A quick implementation of the RottenTomatoes developer API.

There has been very little testing, but the focus was to get something off the 
ground rapidly and go from there.

If you're in a rush, here's how to get started:

	<?php

		include("rotten_potatoes.php");

		$rp = new rotten_potatoes(array("API_KEY" => "your_api_key"));

		// contains info about search results
		$search = $rp->search("inception");

		// get the first result
		$movie = $rp->movies[$search->results[0]];

	?>

I'll try to work on more documentation soon!
