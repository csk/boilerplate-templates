# boilerplate-templates
Provides boilerplate vulnerability explanations and templates which can easily be used in real-world reports

## How to contribute

The **boilerplate-templates** `gh-pages` branch is essentially a [Jekyll](http://jekyllrb.com/) site.

For example, you want to add a new *template*: **Testing for SSI-Injection**

1. Clone the `gh-pages` branch: `git clone -b gh-pages https://github.com/owtf/boilerplate-templates.git` .
1. Make a new folder inside the `templates` directory, namely `ssi-injection`.
1. Add the relevant template in that folder, `templates/ssi-injection`. Templates are essentially **Markdown** formatted files, `index.md`. See the examples given (`templates/<vuln>/index.md`) for how to write a template.
1. Once you added the template as `index.md` inside the `templates/ssi-injection`, add a new entry in the `_data/vulns.yml` file. This essentially makes a new index for the vulnerability on the site.
For `ssi-injection` it would be: 

  ```
  - name: "SSI Injection"
    id: 7
    url: /templates/ssi-injection
    author: "<your name>"
  ```

1. Install [Jekyll](http://jekyllrb.com/) with `gem install jekyll`
1. Try out your changes to see if it is working as expected. Serve the project using `jekyll serve --baseurl=/boilerplate-templates` 
1. All done, open a pull request!
