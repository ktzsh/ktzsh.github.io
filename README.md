Personal Webpage
=========================

Powered by Jekyll

Local Build Steps (Arch OS - Similar on other variants)
```
sudo pacman -S ruby2.7 # Latest is 3 but is not compatible with github-pages gem

export GEM_HOME="$(ruby-2.7 -e 'puts Gem.user_dir')"
export PATH="$PATH:$GEM_HOME/bin"

bundler-2.7 init

add <gem "github-pages"> in Gemfile

bundle-2.7 update
bundle-2.7 install
bundle-2.7 exec jekyll serve
```