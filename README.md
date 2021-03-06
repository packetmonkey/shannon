# Shannon

A little Gem to calculate Shannon entropy (base 2).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'shannon'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install shannon

## Usage

```ruby
require "shannon"

Shannon::entropy ""               #=> 0
Shannon::entropy "aaaa"           #=> 0
Shannon::entropy("abcde").round 4 #=> 2.3219
```

It uses base 2 for the log by default, so `Shannon::entropy "abcde"` and `Shannon::entropy "abcde", 2` will give the same answer.

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/shannon. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.
