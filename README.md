SpreePickup
=============

SpreePickup is an extension and one stop solution to integrate pickup functionality in a spree application.

* This extension allows to add pickup location to your orders. The user can choose from the list of pickup locations.

* When a user chosses pickup as the mode of delivery then the shipping address of the order is pickup location itself.

* This extension adds new states `ready_for_pickup` and `shipped_for_pickup`. An order is in `read_for_pickup` when the order has arrived at pickup location while order is in `shipped_for_pickup` state when the order has been shipped from warehouse/store to the pickup location.

Demo
----
Try Spree Pickup for Spree master with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-pickup-master)

Try Spree Pickup for Spree 3-4 with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-pickup-3-4)

## Installation

1. Just add this line to your `Gemfile`:
  ```ruby
  gem 'spree_pickup', github: 'vinsol/spree_pickup'
  ```

2. Execute the following commands in respective order:

   ```ruby
    bundle install
    ```

   ```ruby
    bundle exec rails g spree_pickup:install
    ```

## See It In Action

<a href="http://www.youtube.com/watch?feature=player_embedded&v=FEtDsCeDRhs
" target="_blank"><img src="http://img.youtube.com/vi/FEtDsCeDRhs/0.jpg" 
alt="Youtube Video Tutorial" /></a>

Contributing
------------

1. Fork the repo.
2. Clone your repo.
3. Run `bundle install`.
4. Run `bundle exec rake test_app` to create the test application in `spec/test_app`.
5. Make your changes.
6. Ensure specs pass by running `bundle exec rspec spec`.
7. Submit your pull request.

Testing
-------

Be sure to bundle your dependencies and then create a dummy test app for the specs to run against.

```shell
bundle
bundle exec rake test_app
bundle exec rspec spec
```

Credits
-------

[![vinsol.com: Ruby on Rails, iOS and Android developers](http://vinsol.com/vin_logo.png "Ruby on Rails, iOS and Android developers")](http://vinsol.com)

Copyright (c) 2017 [vinsol.com](http://vinsol.com "Ruby on Rails, iOS and Android developers"), released under the New MIT License

