This is the most basic example and case for xss. The page works by taking the inputted query string, and (once it is determined that it cannot be found) printing it out so they user can see a message like "Sorry, no results were found for QUERY. Try again.". Turns out, the entered query text is simply combined with the already constructed output, and then printed to the webpage. This is allows for the insertion of html tags, which will be interpreted by the page when it renders.

Answer: <script>alert(1)</script>
