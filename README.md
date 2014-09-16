Rails Submodules
================

#### Notes

[Source Code](https://github.com/lscott3software/rails-submodules)

**Add a submodule to your project**
```
$ git submodule add gitlink vendor/twbs
```

**application.rb**

```
class Application < Rails::Application
  config.assets.paths << Rails.root.join(‘vendor’, ’twbs')
end
```

**application.css**

```
# for minified source
*= require dist/css/bootstrap.min
```
**application.js**

```
# for minified source
//= require dist/js/bootstrap.min
```
