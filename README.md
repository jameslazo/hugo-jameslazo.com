# Resume CI/CD Pipeline

This project started as a fork from Eddie Webb's [Hugo Resume theme](https://github.com/eddiewebb/hugo-resume). Visit the original repo for additional background information.

## Updates

My biggest contribution to this repo was adding the .devcontainer so that Go, Hugo, Git and any required dependencies are loaded into a Docker container, allowing editing on any machine, or even in the browser with Codespaces. Also, providing Terraform code for provisioning all resources in AWS. I should note that the original repository includes Circle CI for deployment and Netlify CMS for editing and Git version control. I just prefer Terraform and GitHub Actions for my workflow.

Besides creating the content for my website based on the exampleSite in the original theme repo, I also did some housekeeping removing assets for sections I am not using and some light [CSS](themes/hugo-resume/static/css/resume.css) edits to improve image layout. The `resume-image` class was added to [projects summary](themes/hugo-resume/layouts/partials/projectsSummary.html) and [publications summary](themes/hugo-resume/layouts/partials/publicationsSummary.html). I also changed the Project submenu item "Creation" to "Deployments" in the [index.html](themes/hugo-resume/layouts/index.html) and subdirectory under /content. And there was a limited set of devicons that can be applied to tags in the Skills sections, but I prefer a uniform `</>` delimiter.

## Setup & Use

From the dev container, you just need to update the `config.toml` then open the terminal and run the commands `hugo build` and `hugo server` to get going. Edit the CSS files under the theme's `static` folder to your liking and create your markdown files under the /content directory. The cards on the home page are populated from the /data json files.

## Credits

Forked from Eddie Webb's [Hugo Resume theme](https://github.com/eddiewebb/hugo-resume).

This project ports the Start Bootstrap Resume theme by David Miller to support hugo.

### Contributions
The following users have made notable contributions:
- [Anthony Whitford](https://github.com/awhitford)
- [Kaushal Modi](https://github.com/kaushalmodi)
- [Julien Rouse](https://github.com/JulienRouse)

### Start Bootstrap Resume

Start Bootstrap is an open source library of free Bootstrap templates and themes. All of the free templates and themes on Start Bootstrap are released under the MIT license, which means you can use them for any purpose, even for commercial projects.

* https://startbootstrap.com
* https://twitter.com/SBootstrap

Start Bootstrap was created by and is maintained by **[David Miller](http://davidmiller.io/)**, Owner of [Blackrock Digital](http://blackrockdigital.io/).

* http://davidmiller.io
* https://twitter.com/davidmillerskt
* https://github.com/davidtmiller

Start Bootstrap is based on the [Bootstrap](http://getbootstrap.com/) framework created by [Mark Otto](https://twitter.com/mdo) and [Jacob Thorton](https://twitter.com/fat).

