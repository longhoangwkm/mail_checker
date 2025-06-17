# Mail Checker Documentation

## Overview
Mail Checker is a Ruby gem designed to validate and filter disposable email addresses. It helps ensure that users provide legitimate, non-temporary email addresses for your application or service.

## Features
- Detects disposable/temporary email addresses
- Easy integration with Ruby applications
- Maintains an up-to-date list of disposable email domains

## Installation
Add this line to your application's Gemfile:

```ruby
gem 'mail_checker'
```

And then execute:

```sh
bundle install
```

Or install it yourself as:

```sh
gem install mail_checker
```

## Usage

```ruby
require 'mail_checker'

MailChecker.valid?('user@example.com') # => true
MailChecker.valid?('user@mailinator.com') # => false
```

## Updating Disposable Domains
To update the list of disposable domains, run:

```sh
rake update
```

## Contributing
Bug reports and pull requests are welcome on GitHub at https://github.com/longhoangwkm/mail_checker.

## License
This project is licensed under the MIT License. See LICENSE.txt for details.