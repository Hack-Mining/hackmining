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
- thanks.html (site being called once user has sent off form)
- custom.css (containing my crude custom css, don't judge)
- pico.min.css (containing the CSS framework we've used)

# Developing (Quick Guide)

In case you ever want to re-use this static site (e.g. to use it for other AMT events),
you have to do the following things

- Amend the HTML code (dates, event name, logos, tags etc.) accordingly (mostly just in index.html)
- Sign up for a form submission service such as [formspark.io](https://formspark.io/) or [Paperform](https://paperform.co/)
- In the past i've used [formspark.io](https://formspark.io/) as they offered 250 free form submissions
- Add the form from that submission service to the website (in index.html)
- Host the html and static assets on some static website provider such as github or gitlab
- We've chosen github here as the RWTH gitlab had some weird permission settings which didn't allow the page to be viewed publicly

# Developing (Detailed Guide)
*Tipp:* Read the code! Check the commit history as well!

## HTML

- There's two .html-files: index.html and thanks.html
- The current index.html already contains all important bits such as meta-info for search engines, css imports, page layout & contents
- So if you want to change anything (e.g. for the next hackathon) you must only amend the page contents
- This likely includes replacing some images and tests
- The images can be found in the ./images folder
- We're currently redircting to the AMT imprint and data & privacy declations. By Prof Clausen, this was fine.

## Style (CSS)

- We're using the [Pico](https://picocss.com/)-CSS-Framework which is a minimal and easy-to-use CSS Framework
- The page layout is according to the layouts provided by Pico [Pico Docs](https://picocss.com/docs/)
- We've picked the main color as #98fb98 (light green) because &#129409;
- We've written some custom CSS (e.g. for those tags) which can be found in custom.css

## Submission Forms

- Importantly, static web hosting doesn't allow to have a back-end
- In order for participants to submit their registration, we've included an external form (see index.html)
- We've chosen [formspark.io](https://formspark.io/) as they offer 250 free submissions
- So create an account there and embed the form in the website
- This has to be done for all future hackathons as the 250 free submission get used up by test submissions + real submission quite quickly
- TEST the form submission before publicly advertising the website
- After submission I made it so that the registered user is redirected to thanks.html

## Static Web Hosting

- Most prominently, static web hosting doesn't allow for back-ends to exist
- This is also true for Github static pages
- Read the Github static pages docs -> [Docs](https://pages.github.com/) !
- If you commit to this repository, the corresponding github static page will update ~10 minutes later
- You don't have to commit to view changes you made, you can check out the changes using your local browser and the file:/// path as there is no back-end