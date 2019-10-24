# Pull Requests Guideline

> This document is designed to be a guideline for engineers, explaining how a good PR look like, and what to do in certain situations.

## Communication

> PR comment dialogue must be courteous and professional at all times.
> Disagreement is perfectly acceptable (and healthy), as long as it doesn't become personal e.g. straying into openly questioning others' standards.
> If you have specific concerns, make your point in private to the individual as constructively as you can.

### As PR owner

> - Be kind, descriptive and open minded. Protect your code with respect to others and accept valid feedback as given knowledge. (No one on your PR is here to critique you personally)
> - Directly @mention people if you want their input.
> - If you need support for your point or you have got a question which you think other person might have and answer, tag them in your comment.
> - Be explicit about specific areas where you may want a more thoughtful review:
>
>   - What are people's thoughts on this and that.
>   - Do we want to apply this design pattern here?
>   - Not 100% happy with that bit, anyone knows better approach?
>   - etc.
>
> - Communicate if the work is ongoing, For example you can use tags from bellow, like [WIP] if it’s not ready to review
>   - Ex. `[WIP][FEATURE] Add button component`
> - You can put your initial comment on PR to explain, that feature is not ready yet but you want early feedback, to avoid big changes in the end.
> - Comment on your own code if you spot something.

### As PR reviewer

> - Be kind, descriptive and open minded.
> - Make sure you understand the context of the pull request, before you put any feedback.
> - Cite your reasoning.
> - Explain your concern well, with example and details. Ideally you would provide an example of what should better solution be.
> - Make sure you are not making it personal. For example you can use indirect appeal. Ex.
> - Instead of saying `-"You need to change this to ..."` you can say `-"We use this approach to solve simillar problem ..."`

## Mentality

Don't be afraid to **REJECT** PR.

> **Straight reasons to reject:**
>
> - Poor solution quality
> - Coding Standards are not met
> - Security issues
> - Missing **Q**uality, **U**nderstanding, **A**greement, **D**eployment, **S**ecurity.
>   [What is QUADS?](pr_quads.md)
> - PR is too BIG (see agreed limits bellow)
> - PR is not following this guide

If you have committed your time for reviewing a PR, make sure you are doing it well.

> - If it's appropriate, pull the code from PR's branch and run the app on your local environment
>   - Examples of what appropriate PR means:
>     - It's not simple text change
>     - PR is decent size
>     - There is some business logic going on
> - Review code as if it's last chance to save the world.
> - Do not skim it. If you started it, put some effort into it.
> - Keep checks of whitespaces and missing commas for linters and automations.
> - If PR is opened in TFS, toggle `Wait for author` option.
>   - So that people can see, that you are reviewing it.
>   - To prevent completion while you are reviewing PR

If you are opening PR.

> Make sure, you have checked everything before you ask for a review.

### Things to keep in mind

What PR's are **NOT**

> - PR's, are not just one way, dry opportunity to get your code to `master`
> - PR's, are not for personal arguments, as well as they are not designed to abuse you or anyone else

What PR's **ARE**

> - PR's, are **opportunities to learn**. This works both ways as for reviewer as well as for PR creator
> - PR's, are designed to get our code quality as close as possible to standards we follow
> - PR's, are collective effort, not single engineer

## Technical

### What is the perfect PR **size**?

> Many studies of Pull Requests, like one from "Cisco", has shown that ideal size for a single PR is **up to 400 lines** of code.
> Not only number of lines is important, but number of files is also crucial.
> Why bother?
>
> - It quicker & easier to review
> - It reduces chances of bugs
> - It does not block other engineers
> - It speeds up delivery

What is the real world TOP limit? Where should I hit REJECT button?

> - If Pull Request is larger then **700** changed or new lines, don't be afraid of asking for a breakdown.
> - If it's something ridiculous like **30+** files changed, we should breakdown this PR.

What if there is no way to avoid **HUGE PR**

> - Request a group review session (ideally with at least one representative from a different team)
> - Walk through your PR

### How to format PR description and title?

Every PR Title must follow agreed structure. Be descriptive. Use tags.

**TAGs:**

> ```
> [FEATURE]  # New feature
> [BUG]      # Bug fix
> [REFACTOR] # Refactored legacy / resolved tech debt
> [SETUP]    # Configuration / new app / plugin setup
> [WIP]      # Work In Progress
> [DNM]      # Do Not Merge
> ```

> **Example:**
>
> ```
> [FEATURE] New Login POST endpoint for MyGoCo
> [BUG] Fixed broken login validation
> [REFACTOR] Implemented factory pattern
> ```

You can combine TAGs if needed.

> **Example:** > `[WIP][FEATURE] Adding new comment component`
