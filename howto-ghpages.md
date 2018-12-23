git checkout -b gh-pages
git push --set-upstream origin gh-pages
git clone git@github.com:davidearn/math3a.git gh-pages

This URL now works nicely: https://davidearn.github.io/math3a/

git checkout master
cd gh-pages
git checkout gh-pages
git branch
cd ..

The gh-pages directory contains the gh-pages branch and is always
checking out that branch, so you can copy stuff there and then git add
and push to make it appear on the web page.

To get the theme:

- go the repo on github
- settings --> github pages --> choose a theme

See also:

https://help.github.com/categories/github-pages-basics/

to learn about creating an index file rather than just letting the README be used by default.
