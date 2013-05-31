
# Instructions

**NOTE**: For development, always work out of the "source" branch, never, ever touch "master".

1. Clone the repo, install the  dependencies, and start the preview server.

    ```bash
    git clone git@github.com:drawsgood/drawsgood.github.com.git
    git checkout source
    npm install
    npm run-script preview
    ```

2. Visit <http://localhost:8080/> in your browser.

3. Make changes to `./contents/some-path/index.md` and refresh the page.  You can add more pages like <http://drawsgood.github.io/some-design> by making a folder `./contents/some-design` and an `index.md` file inside of it.  Then when you run it locally, you will need to visit <http://localhost:8080/some-design/> (note the trailing forward slash for local development, Github automatically appends this).

4. You can also edit `./templates/layout.jade` for HTML changes using the [Jade][jade] template engine.

[jade]: http://jade-lang.com

5. Make CSS changes using LESS or plain CSS by editing files in the `./contents/css` folder.

6. Add images in the `./contents/img/` folder and fonts in the `./contents/font/` folder.

7. When you're ready to deploy your changes:

    ```bash
    git add .
    git commit -m 'I made some changes'
    git push origin source
    npm run-script deploy
    ```

8. This will automatically build the site, and then deploy it to the master branch.

9. Visit your website hosted with Github Pages at <http://drawsgood.github.io>.

## Support

If you run into issues please contact <niftylettuce@gmail.com>.
