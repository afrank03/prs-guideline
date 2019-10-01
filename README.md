# Pull Requests Guideline
> This document is designed to be a guideline for engineers, explaining how a good PR look like, and what to do in certain situations. 

## Communication
TBC

## Mentality
Don't be afraid to **REJECT** PR.
> Straight reasons to reject:
> - Poor solution quality
> - Coding Standards are not met
> - Security issues
> - Missing **Q**uality, **U**nderstanding, **A**greement, **D**eployment, **S**ecurity. 
[What is QUADS?](https://gocomparecom.sharepoint.com/Tech-Engineering/SitePages/Pull-Request-Guide.aspx) 
> - PR is too BIG (see agreed limits bellow)
> - PR is not following this guide

If you have comitted your time for reviewing a PR, make sure you are doing it well.
> Pull the code and run the app on your local environment

### Things to remember
What PR's are **NOT**
> - PR's, are not just one way, dry opportunity to get your code to `master`
> - PR's, are not for personal arguments, as well as they are not designed to abuse you or anyone else

What PR's **ARE**
> - PR's, are opportunities to learn. This works both ways as for reviewer as well as for PR creator
> - PR's, are designed to get our code quality as close as possible to standards we follow
> - PR's, are collective effort, not single engineer

## Technical
### What is the perfect PR **size**?
> Many studies of Pull Requests, like one from "Cisco", has shown that ideal size for a single PR is **up to 400 lines** of code.
> Not only number of lines is important, but number of files is also crucial. 
Why bother?
> - It quicker & esier to review
> - It reduces chances of bugs
> - It does not block other engineers
> - It speeds up delivery
What is the real world TOP limit? Where should I hit REJECT button? 
> - If Pull Request is larger then **700** changed or new lines, don't be afraid of asking for a breakdown.
> - If it's sometihing rediculous like **30+** files chnaged, we should breakdown this PR.

