UnifiedPayment
================

Provides the necessary library through UnifiedPayment::Client to interact with UnifiedPayment Gateway to

1. Initiate a payment
2. Get payment status
3. Reverse a completed payment

Also provides with MVC structure which can be extended according to the application.

Set Up
================

Add To Gemfile:

For Rails 3 

```ruby
gem 'unified_payment', '1.0.1'
```

For Rails 4
```ruby
gem 'unified_payment', '1.1.0'
```

And run below command
```ruby
bundle

bundle exec rails g unified_payment:install

bundle exec rake db:migrate
```
Also add your configurations in a yml file. For example, here is

```ruby
config/unified_payment.yml
```

```ruby
merchant_name: 'Your Merchant name at gateway'
base_uri: "http://127.0.0.1:5555" #same as stunnel's accept port.
```
To Run Specs
================
```ruby
bundle

cd spec/dummy

bundle exec rake test_unified_payment

```
Credits
================

[![vinsol.com: Ruby on Rails, iOS and Android developers](http://vinsol.com/vin_logo.png "Ruby on Rails, iOS and Android developers")](http://vinsol.com)

Copyright (c) 2014 [vinsol.com](http://vinsol.com "Ruby on Rails, iOS and Android developers")
