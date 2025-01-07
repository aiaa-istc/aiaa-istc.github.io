# To test locally on Ubuntu 22.04, install the following:
sudo apt install ruby-all-dev
sudo apt install python3-is-python-dev build-essential dos2unix
sudo apt install zlib1g-dev
sudo apt install ruby-bundler
sudo apt install libyaml-dev # required for psych gem to install without errors (needed for architect gem)

# no addtl install needed for architect
# install for jekyll-theme-dinky without gem name given properly?:
#sudo gem install jekyll-theme-dinky
# no addtl install needed for minima
# install for jekyll-theme-cayman without gem name given properly?:
#sudo gem install jekyll-theme-cayman

# To test locally on Ubuntu 24.04, additionally install the following:
sudo gem install bundler
# this forcibly updates bundler, if it has issues with dependencies, see: https://stackoverflow.com/questions/60572233/bundler-error-cannot-find-rake-13-0-1-even-though-it-is-installed
sudo gem install rake
# architect seems to require rake now, via architect -> coffee-rails -> railities -> rake
# you may also need to change the config path for bundler if you run into issues with 'bundle install' complaining about write access, a la something like:
#mkdir ~/Documents/bundleconfig
#bundle config set --local path '~/Documents/bundleconfig'

# To test locally once dependencies are meet, run the following:
git clone https://github.com/aiaa-istc/aiaa-istc.github.io.git
cd aiaa-istc.github.io
# may need/want to use the following instead of giving sudo password during bundle install step
#bundle config set --local path 'vendor/bundle' # installs ./vendor/bundle
bundle install
bundle exec jekyll serve
# and then in a separate window, run:
firefox &
# and browse to: localhost:4000
# in order to see the page
# could do it as:
#firefox https://localhost:4000 &
# use Ctrl-C in the jekyll server window to stop

# note that if you delete the original git clone pulldown of the repo,
# that you have to run 'bundle install' in the new directory before running 'bundle exec jekyll serve' on it

# References:
# https://help.github.com/articles/adding-a-jekyll-theme-to-your-github-pages-site/
# https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#requirements
# https://github.com/pages-themes/architect
# https://github.com/mmistakes/jekyll-theme-basically-basic#installation

# https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll
# https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll


#
# basic git commands:
#

# creating and swapping branches
git branch --list # list branches and shows current branch
git checkout master # swaps over to a branch that currently exists
git checkout -b new_branch # creates and swaps over to a new branch called new_branch

# --eof--
