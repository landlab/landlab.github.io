# landlab.github.io
Repository for Landlab's website http://landlab.github.io

## To develop locally

- clone the repo locally<br>
`git clone <link-to-repo> <name-of-new-directory>`
- cd into your new directory<br>
`cd <name-of-new-directory>`
- make a new branch<br>
  `git checkout -b <name-of-new-branch>`
- edit files, most likely `views/home.html`, in a text editor

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
