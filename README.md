# landlab.github.io
Repository for Landlab's website http://landlab.github.io

## To develop locally

- clone the repo locally<br>
`git clone <link-to-repo> <name-of-new-directory>`
- cd into your new directory<br>
`cd <name-of-new-directory>`
- make a new branch<br>
  `git checkout -b <name-of-new-branch>`

## Edit files

The repository has four main folders:

- **assets**, which contains image files

- **scripts**, which contains JavaScript files

- **stylesheets**, which contains styles in CSS (and SCSS) files

- **views**, which contains HTML files, one for each page of the website

At the root of the project is the `index.html` file that contains the framework (header, logo, footer, meta data, and links to scripts and styles) for every page on the site.

Most likely, you will want to edit the `home.html` file in the `views` directory. It contains the majority of the landing page's content. Open it in your favorite text editor.

HTML is a markup language that is structured using tags in angle brackets. For example, a paragraph is noted by the content inside of an opening `<p>` and a closing `</p>` tag:
```
<p>I am the content of a paragraph</p>
```
The content inside the tags is plain text and easy to edit.

If you need to add an image, add the image file to the assets folder and, in the HTML, reference the path to it in the `src` attribute of an `<img />` tag.

```
<img src="../assets/Landlab-logo.png" alt="Landlab logo">
```

## To run locally and see your changes
From the root directory (the directory with the `index.html` file), run an HTTP server. Some options for servers which you might already have installed include a simple Python server and a simple node HTTP server.

### Simple Python server 2.x

run<br>
`
python -m SimpleHTTPServer 8000
`

see the results of your local code in a browser window at:<br>
`http://127.0.0.1:8000`

### Simple Python server 3.x

run<br>
`
python -m http.server 1337
`

see the results of your local code in a browser window at:<br>
`http://127.0.0.1:1337`

### Simple HTTP server (Node)

if you have Node installed, install http-server<br>
`npm install http-server -g`

run<br>
`
http-server -o
`

see the results of your local code in a browser window at:<br>
`http://127.0.0.1:8080`

## Push your changes to production

When you are happy with the results, `git add` and `git commit` your changes. Then push your branch up to the remote repository on GitHub<br>
`git push origin <your-branch-name>`

From the repository on GitHub, make a Pull Request to master. Once your changes are merged into master, they will be live on `https://landlab.github.io`.
