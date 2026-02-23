Lab 4

Platform
PortSwigger Web Security Academy

Vulnerability Type
DOM-Based XSS

Target
Search box

Injection Point
Comment Box

Payload Used

">
How It Worked

I entered a random text in the search box and came ot find that the input is taken but shows and errorbut the input is shown on the page- that means injection is possible.I moved to inspect element and find my input landing in the and " ",where it lies under An Html tag and attributes respectively. Then i thought to break out of the quotes and can i add a new attributes and finally can i inject any suitable ee=vent handler for this. then i tried firstly closing the tags "><onload=alert(1)> payload which didnt worked.

The input was reflected inside the src attribute of an tag. By injecting ">, I broke out of the attribute context and closed the tag. My initial attempt to inject onload directly failed because it was not attached to a valid HTML element. I then injected an element with an onload event handler, which successfully executed JavaScript when the page rendered the stored comment.
