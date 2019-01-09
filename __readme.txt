# To test locally on Ubuntu 18.04, install the following:
sudo apt install ruby-all-dev
sudo apt install python-dev build-essential dos2unix
sudo apt install zlib1g-dev

# To test locally once dependencies are meet, run the following:
git clone https://aiaa-istc.github.io/aiaa-istc.github.io.git
cd aiaa-istc.github.io
bundle install
bundle exec jekyll serve
# and then in a separate window, run:
firefox &
# and browse to: localhost:4000
# in order to see the page
# use Ctrl-C in the jekyll server window to stop

# References:
# https://help.github.com/articles/adding-a-jekyll-theme-to-your-github-pages-site/
# https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#requirements
# https://github.com/pages-themes/architect
# https://github.com/mmistakes/jekyll-theme-basically-basic#installation

# --eof--
