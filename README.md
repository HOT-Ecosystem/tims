# Terminology Infrastructure and Management Services Group (TIMS Group) - website
TIMS is using Jekyll and GitHub Pages for its static site: https://hot-ecosystem.github.io/tims/

## How to update the site
1. **Edit files**: [What files to edit](_docs/site.md)
2. **Depoy updates**: Push/make a commit to the `gh-pages` branch, and the update will automatmically be deployed.

## More information
<details><summary>Using on your local machine</summary>
<p>

### Using on your local machine

The Docker Compose setup should allow you to run the Jekyll server locally (in Docker), edit files, and see the results with live reload.

* Run `docker compose up` and wait until you see `Server running... press ctrl-c to stop.`
* Go to http://localhost:4000 in your browser.
* Open the page you want to edit in the browser and in your editor.
* Make changes, save, and you should see the results in your browser in a few seconds.
* The console where you ran `docker compse up` should show some logging. It might be useful if you're having issues.
* Commit your changes and push to GitHub
* Changes should be visible on the GitHub Pages side once they're built and deployed. You can watch and confirm if the build and deployment succeeded [here](https://github.com/HOT-Ecosystem/tims/actions)
* `CTRL+C` in the terminal should stop the Docker container.
  * No need to do a `docker compsoe down` unless you need to start with a clean container, which takes time to do the initial setu.
  * Running `docker compse up` the next time to continue with the live reload should be much faster the next time.

</p>
</details> 

<details><summary>Initial setup</summary>
<p>

## Initial Setup

* Jekyll based: https://jekyllrb.com/docs/
  * Server sepecific settings, which you can use in the docker-compose-yaml file, are here: https://jekyllrb.com/docs/configuration/options/#serve-command-options
  * 
* GitHub specifics: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll
* Custom theme: https://mmistakes.github.io/minimal-mistakes/

</p>
</details>

<details><summary>Jekyll static site resources</summary>
<p>

## Jekyll static site resources

Content can be added by following Jekyll's documentation and using the required markdown.
* Pages: https://jekyllrb.com/docs/pages/
* Posts: https://jekyllrb.com/docs/posts/

Jekyll uses [Kramdown](https://kramdown.gettalong.org/index.html) for markdown.

* [Quick reference](https://kramdown.gettalong.org/quickref.html)
* [Documentation](https://kramdown.gettalong.org/documentation.html)

</p>
</details>

<details><summary>Additional devops resources</summary>
<p>

### Additional devops resources
* [Deployment action logs](https://github.com/HOT-Ecosystem/tims/actions/workflows/pages/pages-build-deployment)
* [Alternate page for: Deployment action logs](https://github.com/HOT-Ecosystem/tims/deployments)
* [GitHub pages site settings](https://github.com/HOT-Ecosystem/tims/settings/pages)

</p>
</details>