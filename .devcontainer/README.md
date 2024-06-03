# Installation
- First login to docker
- `docker login -u hm-<username> gitlab.lrz.de:5005` -> ENTER
- Put in your password from gitlab

1. Just copy the `.devcontainer` Folder to your Workspace.
2. Install the DevContainer Extension from Microsoft `ms-vscode-remote.remote-containers`
3. In VS-Code Click on _Reopen in Container_ in the Popupmessage on the right bottom corner
   If ther is no Message Press Strg+Shift+P and Type `Rebuild and Reopen the Container` or something like this
4. get into your main Latex file and click on the left site on `LATEX` there should be a `Run` button on the top where you can build your Latex paper


# Further instructions
- If you want to build your paper just press Strg+S this not only saves the document but also builds it.
- If you want to build it automaticly (and also save it automaticly) just press Strg+Shift+P and Type `Auto Save` and toggel it.