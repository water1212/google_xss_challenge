So this attack is all about reading the code. If you look, the number of the image is what drives this site, and is also reflected in the webpage's output. 

The key line to pay attention to is line 17, which contains:
<img src='/static/level3/cloud" + num + ".jpg' />;

As you can see, the string concatenation here is the main cause for concern.By closing the preceeding ' mark early and then using the onerror trick as in the last exercise, we can make headway.

Unfortunately, by doing this, the <img> tag would look something like:
<img src='/static/level3/cloud'onerror=alert(1).jpg'/>

The issue is the last ' after the .jpg. In order to bypass that, we can just simply close the <img> tag with a > and be done

Answer: 'onerror=alert(1)>
