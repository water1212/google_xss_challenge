Level 4 is all about url encoding. A good resource on these can be found here: https://www.w3schools.com/tags/ref_urlencode.asp

This level is quite similar to level3, except that we have to escape some of the characters in the URL, as certain ones are not permitted (mainly ;) For saftey's sake, I went ahead and encoded all the special characters.

The solution unescaped is ?timer=');alert('Hi
The reason we do this is to close out the current javascript function that this is being passed into, and then outright just running the alert function next. 


Answer: ?timer=%27%29%3Balert%28%27Hi
