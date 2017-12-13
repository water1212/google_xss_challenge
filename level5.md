Level 5 is a bit odd to me, because its a more basic example, although I did manage to find another security flaw (unrelated to xss). I'll explain that one as well.

However, if you take a look at the hints section, you'll notice one talking about executing javascript from links without using the onclick event. That hint, coupled with the way the next parameter is being used in the <a> tag, allows us to execute javascript from the url using  "javascript:CODE"

Answer: next=javascript:alert(1)


BONUS: so the other security flaw I found involving this was, using the next parameter, we can force the page to redirect to some completely different page. In my case, I used espn.com, but feel free to try it with any page (malicious or benign).

Bonus Answer: next=http://www.espn.com
