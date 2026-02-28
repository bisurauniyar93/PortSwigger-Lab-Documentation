🔥 Simple Mental Rule For You (Very Important)

Whenever you see:

location.search
location.hash
document.URL
window.location

Inside JavaScript…

🚨 Immediately suspect URL-based injection.

✅ So We Concluded

✔ Injection point = URL hash
✔ Because code reads location.hash
✔ And uses it without filtering
