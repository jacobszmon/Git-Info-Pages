# just-the-docs-template

This is a *bare-minimum* template to create a [Jekyll] site that:

- uses the [Just the Docs] theme;
- can be built and published on [GitHub Pages] using a [GitHub Actions workflow];
- can be built and previewed locally, and published on other platforms.

You can see [a deployed version of this template here].

To get started with creating a site, just fork this repository.

After forking the repository, update it as needed:

## Invite Others to Collaborate with you on this Project

Only one team member needs to clone the repository. They can then give their team members access under the repo's `Settings => Collaborators` page.

The team should then collaboratively work on building out this site according to the assignment instructions.

## Replace the Content of the Template Pages

Update the following files to your own content:

- `index.md` (your new home page)
- `README.md` (information for those who access your site repo on GitHub)
- `docs\first-doc.md` (Sample nested page. All pages other than home should go in `docs`.)

Remember that you will be using [Markdown Syntax] rather than raw HTML to format the content of your pages.

## Publish your site on GitHub Pages

The following should be done by the team member who owns the repo.

1.  If your created repositor is `YOUR-USERNAME/YOUR-REPO-NAME`, update `_config.yml` to:

    ```yaml
    title: YOUR TITLE
    description: YOUR DESCRIPTION
    theme: just-the-docs

    url: https://YOUR-USERNAME.github.io/YOUR-REPO-NAME

    aux_links: # remove if you don't want this link to appear on your pages
      Template Repository: https://github.com/YOUR-USERNAME/YOUR-REPO-NAME
    ```

2.  Push your updated `_config.yml` to your site on GitHub.

3.  In your newly forked version of this repo on GitHub:
    - go to the `Actions` tab and enable the repository actions.
    - go to the `Settings` tab -> `Pages` -> `Build and deployment`, then select `Source`: `GitHub Actions`.
    - if there were any failed Actions, go to the `Actions` tab and click on `Re-run jobs`.

## Customization

You're free to customize sites that you create with this template, however you like!

[Browse the Just the Docs documentation][Just the Docs] to learn more about how to use this theme.

## Licensing and Attribution

This repository is licensed under the [MIT License]. You are generally free to reuse or extend upon this code as you see fit; just include the original copy of the license (which is preserved when you fork this repo). While it's not necessary, we'd love to hear from you if you do use this template, and how we can improve it for future use!

The deployment GitHub Actions workflow is heavily based on GitHub's mixed-party [starter workflows]. A copy of their MIT License is available in [actions/starter-workflows].

----

[Jekyll]: https://jekyllrb.com
[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[GitHub Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[a deployed version of this template here]: https://stungeye-rrc.github.io/Just-The-Docs-Template/
[Markdown Syntax]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
[MIT License]: https://en.wikipedia.org/wiki/MIT_License
[starter workflows]: https://github.com/actions/starter-workflows/blob/main/pages/jekyll.yml
[actions/starter-workflows]: https://github.com/actions/starter-workflows/blob/main/LICENSE
