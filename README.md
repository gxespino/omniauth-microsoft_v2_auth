# Omniauth::MicrosoftV2Auth

*** Note: The original repo disappeared for this gem, so we've published it here and updated the gemspec. ***

Microsoft V2 OAuth2 Strategy for OmniAuth.
Can be used to authenticate with Microsoft Services and get a token for the Microsoft Graph Api.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-microsoft_v2_auth', :git => 'git://github.com/pairshaped/omniauth-microsoft_v2_auth.git'
```

And then execute:

    $ bundle

## Usage

```ruby
Rails.application.config.middleware.use OmniAuth::Builder do
  provider :microsoft_v2_auth, ENV['AZURE_APPLICATION_CLIENT_ID'], ENV['AZURE_APPLICATION_CLIENT_SECRET']
end
```
