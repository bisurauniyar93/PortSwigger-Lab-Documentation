Lab 5

Platform
PortSwigger Web Security Academy

Vulnerability Type
DOM-Based XSS

Target
Search box

Injection Point
Search Box

Payload Used
<svg onload=alert(1)>

How It Worked
I entered a random text in the search box and and then i came to find that the input gets stored in the span tag which is an html tags.Then i tried to insert <script> tag but came to find that the script tag is escaped.

Then i anayzed that my Input is stored as a test in HTML Tags and my input is reflected inside html context ;attributes breakout is possible and eventhandlers can be used.
then used svg onload event handler with my input and it worked.
