sofort-rails-client-api
=======================

client for newest sofort api

it's only example module for sofort(using gem 'httparty')
=======================
example of use:

pay example:

@sofort = Sofort::API.new
result = @sofort.pay(12.0, "Sebastian Skopp", 'http://return.url', 'reason', 'EUR', 'DE')

details example: 
details = Sofort::API.new.details("sofort_token")

read sofort documentation
https://www.sofort.com/integrationCenter-eng-DE/content/view/full/2513#h1

