
# Lab 1 – Reflected XSS

## Platform
PortSwigger Web Security Academy

## Vulnerability Type
Reflected XSS

## Target
Search Parameter

## Injection Point
Search Box

## Payload Used
<script>alert(1)</script>

## How It Worked
I broke out of the attribute using " and closed the attribute bu using >  and injected an <script> tag




