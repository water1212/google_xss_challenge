This one is very similar to level1, except that the basic <script> case has been stripped and handled. So we need to think of other ways to go about it. Using things like <b> and <i> work, so we know we're allowed to write html. Turns out, there is an html attibute you can use called 'onerror'. It fires an event when an error occurs that you can use to run javascript with.

In the case of this example, I use the <img> tag with a garbage image to force the onerror event to fire.

Answer: <img src='doesnt_exist.png' onerror=alert(1) />
