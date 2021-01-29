# GingerPandaViewTool

> Various view specific methods for applications I use

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ginger_panda_view_tool'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install ginger_panda_view_tool

## Usage
> This tool/command takes to two string arguments(name , and a message)
> It will prepend a copyright html symbol
> Add this method to application_helper.rb

```ruby
def copyright_generator
  GingerPandaViewTool::Renderer.copyright 'Insert your company name', 'All rights reserved'
end
```

> In rails you would have to render this helper in your view i.e. application.html.erb in the footer

```text
<%= copyright_generator %>
```

## Example
> This Should display
© 2021 | CompanyName All rights reserved


## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/ginger_panda_view_tool. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/[USERNAME]/ginger_panda_view_tool/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the GingerPandaViewTool project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/ginger_panda_view_tool/blob/master/CODE_OF_CONDUCT.md).
