# Configuration

Running the site locally with `bundle exec jekyll serve` there was an error `bundler: failed to load command: jekyll`. Quick research led me to [this page](https://stackoverflow.com/questions/69890412/bundler-failed-to-load-command-jekyll), which says that we need to install `webrick` manually on Mac, and that worked, install with

```
bundle add webrick
```
