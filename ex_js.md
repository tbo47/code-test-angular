https://jsfiddle.net/tbo47/qsuy92ht/

On the link above, there is an html part, a css part, a javascript part.
The rectangle at the bottom right is the final rendering.
You have to press the play button at the top left to refresh the part at the bottom right.

The `openstreetmapGetPOIs` function takes 2 arguments.
The first is a gps coordinate rectangle, the second is the type of point of interest that we want to list.
As you can see, the first argument (on line 6) is hardcoded.
I would like it to be dynamic and come from the javascript call `navigator.geolocation.getCurrentPosition`.
That is to say, we add or subtract `0.1` to the latitude/longitude to create a value to give as the first argument to the `openstreetmapGetPOIs` function

Ideally, the candidate will write readable and asynchronous code.

The result could be a jsfiddle, a github project or email.