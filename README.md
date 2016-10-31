# Ayanami

A Telegram Bot API for Ruby that focuses on simplicity. Ayanami is meant to be a simple interface to Telegram's Bot API. 
The Goal of Ayanami is to keeping it simple and barebone so other people can use it for their own needs.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'Ayanami'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ayanami

## Usage

You can start by creating a Bot object.

```ruby
	b = Ayanami::Bot.new('YOUR_BOT_TOKEN_GOES_HERE')
```

To confirm the connection, You can invoke the `get_me` function to see your bot identity.

```ruby
	puts b.get_me
```

To get received messages or other updates, You can invoke the `get_updates` function to receive updates.

```ruby
	puts b.get_updates()
```

You can also send a simple message to a group/user by invoking the `send_message` function.

```ruby
	puts b.send_message(chat_id: USER_OR_CHAT_ID_GOES_HERE, text: 'Hello :)')
```

For more information about the included functions, Please consult [Telegram's Bot API documentation](https://core.telegram.org/bots/api)

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/patiOne/Ayanami.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

