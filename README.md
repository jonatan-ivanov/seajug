# SeaJUG
Static page demo for SeaJUG

# Setting Up Dev Environment

## Installing [Ruby](https://www.ruby-lang.org/)

There are multiple ways, check the [Downloads](https://www.ruby-lang.org/en/downloads/) page.  
Example with rbenv:

```
brew update && brew install rbenv
rbenv init #follow the instructions
rbenv install --verbose <version> #freshly compiled and slow
rbenv global <version>
rbenv rehash
```

## Installing [bundler](https://github.com/bundler/bundler), [jekyll](https://github.com/jekyll/jekyll) and [octopress](https://github.com/octopress/octopress)

```
gem update --system
gem install bundler
rbenv rehash #if you use rbenv
bundle
rbenv rehash #if you use rbenv
```

If the bundle command fails because it is not able to install Nokogiri, try  
`gem install nokogiri --version '<version>' -- --use-system-libraries`
then run `bundle` again

## Starting local dev server

```
bundle exec jekyll serve
```
