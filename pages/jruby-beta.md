# Getting Started with JRuby

## Before starting

  * Do note that this is in a very early stage of development. See below for known issues.
  * Your application should use Bundler 1.0.10 or later to manage gems.
  * Gemfile must include trinidad.

## Preparing an existing Rails app

- Setup Your Gemfile

An example snippet of a Gemfile:

<pre>
    source :rubygems
    group 'production' do
      gem 'rails', '3.0.7'
      gem 'sqlite3'
      gem 'trinidad', :platforms => :jruby
    end
</pre>

- Then run these commands to update your Gemfile.lock:

<pre>
    rvm install jruby
    rvm jruby
    bundle install
    
    git checkout -b jruby
    git commit -a -m "Gemfile updated for jruby/trinidad"
    git push origin jruby
</pre>

- If you are not using RVM, do this in `$RAILS_ROOT` to update `Gemfile`:

**Assumes you have pre-installed [jruby](http://www.jruby.org/download).**

<pre>
    jruby -S bundle bundle install
    git checkout -b jruby
    git commit -a -m "Gemfile updated for jruby/trinidad"
    git push origin jruby
</pre>


- Follow the Getting Started instructions to setup a new
  Environment. But select Trinidad as your **Application Server Stack** and
  **JRuby 1.6.1** as your Ruby Runtime.
  
## Known Issues

  - `engingeyard` gem is not fully supported under JRuby. YMMV.
  - Selecting Trinidad, does not auto-select JRuby as your runtime.
