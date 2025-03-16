# website
Based on L1nkr template.

## COnfiguration

- Modify `config/_default/hugo.yaml` and `config/_default/params.yaml` according to your needs. Find more info on the theme [wiki](https://github.com/chrede88/L1nkr/wiki/Configuration).
- Build a local version of your site by executing `hugo server` at the root of the repository. You can see the site by navigating to `http://localhost:1313/website/` (actual URL will be outputted in the CLI) in a browser.
- The theme version used to build the site is defined in `go.mod` file.
The best practice is to update to released and tested versions. To update to a specific version execute the following command in a terminal/commandline (at the root path of your site repo):
```shell
  hugo mod get github.com/chrede88/L1nkr@vX.Y.Z
```
Replace X,Y & Z with the corresponding version numbers. You can find the releases [here](https://github.com/chrede88/L1nkr/releases). Please check if any breaking changes are listed under the release you want to update to, before proceeding.

---

## Deploy on Github Pages
Action workflow that will build and deploy your site to Github Pages automatically:+1:
`.github/workflows/buildDeploy.yml`. 
Last step: Go to Settings -> Pages -> Build and deployment -> Set the Source to "Github Actions".
Next time you publish a release this workflow will build and deploy your site :tada:
Your site will be published to the following URL:
`https://alexKazarin.github.io/website`