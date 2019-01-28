# spree_nice_admin

Adds a responsive menu the the Spree 3.7 admin, plus makes it look nicer.

## Changes to the admin html.erb files
Addes order currency to orders in list view and also adds order currency to the order details page in the summery section. Moves the order number to the first column, and truncates the emails to give a more user friendly layout. 

## Changes to the JS files
Removes the default Spree menu js that seems overkill for a simple on/off screenmenu, and then adds a toggle class for the menu onhandheld devices.

## Changes to the CSS files
Just simple styling, looks like a bit of a Shopify rip off, but hey that might change with further updates.

## Installation

1. Add this line to the bottom of your Gemfile:
  ```ruby
  gem 'spree_nice_admin', github: 'matthewkennedy/spree_nice_admin'
  ```

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Copy & run the following commands in order
  ```ruby
  bundle exec rails g spree_nice_admin:install
  ```

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_bs4/factories'
```


## Contributing

If you'd like to contribute, please take a look at the
[instructions](CONTRIBUTING.md) for installing dependencies and crafting a good
pull request.

Copyright (c) 2018 [name of extension creator], released under the New BSD License
