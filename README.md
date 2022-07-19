# Hackmining Web

This is the repository containing a static website for the hackathon "Hack Mining!" registration website.

# Why?

We needed a registration website for the hackathon.

We didn't want to use the RWTH Academy service for creating a website as it is quite costly.
Moreover, websites like shopify etc. may allow fast and easy website configuration but they 
are very much tailored towards e-commerce. 

Therefore, the simplest and cheapest solution seems to be a static website hosted on some static
website hosting service such as github pages.

# Components of the website

- index.html (contains all the infos + submission form)
- thanks.html (site being called once user as sent off form)
- custom.css (containing my crude custom css)
- pico.min.css (containing the CSS framework i've used)
- .gitlab-ci.yml (containing the CI workflow)

# How to use it!

In case you ever want to re-use this static site (e.g. to use it for other AMT events),
you have to do the following things

- amend the HTML code (dates, event name, logo etc.) accordingly (mostly just index.html)
- sign up for a form submission service such as [formspark.io](https://formspark.io/) or [Paperform](https://paperform.co/)
- add the form from that submission service to the website (index.html)
- host the html and static assets on some static website provider such as github or gitlab
- to host static websites using such providers, I suggest reading their docs reading hosting static pages as this requires some configuration

