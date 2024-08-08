# Technical Portfolio

This repository hosts a technical portfolio built using [TechFolio](http://techfolios.github.io). 

See the quick start guide for instructions on how to tailor the template to your own needs.

## local development

Refer to the [Techfolio doc](https://techfolios.github.io/docs/user-guide/local-development), but here is what worked for me on my Mac

```brew install chruby ruby-install xz```

```ruby-install ruby 3.1.3```

You should now be running ruby 3.1.3

```ruby -v```

If your versions are mismatched you may need to run these commands to get a ruby version manager

```brew install rbenv```

```rbenv install 3.1.3```

```rbenv global 3.1.3```

I then had to install sass-embedded

```gem uninstall sass-embedded```

```gem install sass-embedded```

You should now be able to run 

```bundle install```

then run the app with

```bundle exec jekyll serve```
