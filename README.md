How to Update this Site
===

Follow the instructions below to update our site. You will need the following software installed:

- Hugo
- Git

This repo is using a submodule to push the Hugo html site (public folder) to github.io.

```
mlug-hugo ✓ $ git remote -v
origin	https://github.com/mississaugalug/mlug-hugo.git (fetch)
origin	https://github.com/mississaugalug/mlug-hugo.git (push)


mlug-hugo/public ✓ $ git remote -v
origin	https://github.com/mississaugalug/mississaugalug.github.io.git (fetch)
origin	https://github.com/mississaugalug/mississaugalug.github.io.git (push)
```

Cloning the repo
---

Make sure to clone the submodule:

```
git clone --recursive -j8 https://github.com/mississaugalug/mlug-hugo.git
```

Installing Hugo
---

#### Arch

```
pac install hugo-strata-theme
```

#### Debian based

```
sudo apt-get install hugo
```

Updating
---

a. Make the changes

b. Build after change by running `hugo`

```
cd mlug-hugo
hugo
```

c. Add files

```
git add .
```

d. Commit

```
git commit -m "[my commit message]"
```

e. Push

```
git push -u origin master
```

f. Repeat steps c-e on the public folder

* * *

**Reference:**
* https://github.com/whipperstacker/blog/blob/master/content/post/deploying-a-hugo-site-to-github-pages.md
