# Jekyll-mermaid

A [Jekyll](http://jekyllrb.com/) plugin to simplify the creation of [mermaid](https://github.com/knsv/mermaid) diagrams and flowcharts in your posts and pages.


## Installation

1. add this on your gemfile:
  ```
  gem 'jekyll-mermaid-forked', '1.0.0.1', git: 'https://github.com/RobbiNespu/jekyll-mermaid-forked', branch:'master', ref: '2627b41'
  ```

2. Add the gem to your Jekyll `_config.yml`:
  ```ruby
  plugins:
   - jekyll-mermaid-forked
  ```

Please see the [Jekyll documentation](http://jekyllrb.com/docs/plugins/#installing-a-plugin) for more installation options.


## Config

You'll need to update your `_config.yml` with the location of the [mermaid](https://github.com/knsv/mermaid) source javascript file you want to use.

```ruby
mermaid:
 src: 'https://cdnjs.cloudflare.com/ajax/libs/mermaid/8.5.0/mermaid.js'
```


## Usage

Simply include the [jekyll-mermaid](https://github.com/jasonbellamy/jekyll-mermaid) block helper in any of your templates.

```liquid
{% mermaid %}
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
{% endmermaid %}
```

Please see the [mermaid documentation](https://github.com/knsv/mermaid/wiki) for more examples.


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality.


## License
Copyright (c) 2014 [Jason Bellamy ](http://jasonbellamy.com)
Licensed under the MIT license.
