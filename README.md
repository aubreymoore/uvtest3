# uvtest3

## Technical Notes

### Clone reveal.js
It appears that the ```reveal.js``` needs to be cloned into the top level directory of a GitHub repo to render HTML using GitHub pages, so the local repo is initiated using:
```
cd ~/Desktop
git clone ????? uvtest3
cd uvtest
rm -rf .git
```
To host reveal.js presentations on GitHub pages, create a new ```uvtest3``` repo in Gitub, and push the local ```uvtest3```. Enable GitHub pages from the GH settings menu and you should be able to browse to <https://aubreymoore.github.io/uvtest3/> or something similar.

### The ```code``` directory is a ```uv``` project

The ```code``` directory is the root of a ```uv``` project created using:
```
cv uvtest3
uv init --python 3.10 code
cd code
uv venv
source .venv/bin/activate
uv add ipykernel notebook

```
Now, add ```code/.venv/``` to ```.gitignore```.

