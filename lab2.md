
# Lab 2 

## Platform
PortSwigger Web Security Academy

## Vulnerability Type
Stored XSS

## Target
Comment Box

## Injection Point
Comment Box

## Payload Used
<script>alert(1)</script>

## How It Worked
I entered a random text you are hacked in the comment box with name and email address and submitted.After submission i came to find that the message i had posted there remains on the page which means it is stored xss.Then i used the payload <script>alert(1)</script> in the comment box which worked.




