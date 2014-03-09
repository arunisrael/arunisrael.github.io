<div dir="ltr" style="text-align: left;" trbidi="on">
<span style="font-family: Arial, Helvetica, sans-serif;">I created an "angularized" wrapper around the Google Places API and posted it to Github <a href="https://github.com/arunisrael/angularjs-google-places">here</a>. The readme explains how to install, use, and customize the code.</span><br />
<span style="font-family: Arial, Helvetica, sans-serif;"><br /></span>
<span style="font-family: Arial, Helvetica, sans-serif;">The wrapper provides a simple way to do a search for nearby places and to get detailed information about a particular place and it provides responses back in JSON format.</span><br />
<span style="font-family: Arial, Helvetica, sans-serif;"><br /></span>
<span style="font-family: Arial, Helvetica, sans-serif;">You can see a demo of it in this <a href="http://embed.plnkr.co/6kKlcbafz57lS7HEPPMx/preview">plunker</a>.</span><br />
<span style="font-family: Arial, Helvetica, sans-serif;"><br /></span>
<span style="font-family: Arial, Helvetica, sans-serif;">The Google Places API is callback based. To make this work in Angular, it needs to be wrapped in a $rootScope.$apply when the data is ready. You can see what this looks like <a href="https://github.com/arunisrael/angularjs-google-places/blob/master/src/angularjs-google-places.js#L58-L68">here</a>.</span><br />
<span style="font-family: Arial, Helvetica, sans-serif;"><br /></span>
<span style="font-family: Arial, Helvetica, sans-serif;">The API also needs to be initialized with an DOM node or Google Map object which is why $window is injected to access $window.document.creatElement as seen in the code <a href="https://github.com/arunisrael/angularjs-google-places/blob/master/src/angularjs-google-places.js#L72-L78">here</a>.<br /><br />Feedback welcome!</span></div>

