sofort-rails-client-api
=======================

Rails client for newest sofort api

it's only example module for sofort(using gem 'httparty')

important variables:
=======================

@base_uri = 'https://api.sofort.com/api/xml'
APP_CONFIG['sofort']['user_id'] = 123455 # it should be your account user id
APP_CONFIG['sofort']['api_key'] = asd134ufb91b7972fbbv9 # your api key, remember to generate key for !!sofort banking gateway!!
APP_CONFIG['sofort']['base_url'] = 'https://api.sofort.com/api/xml'

pay example:
=======================

@sofort = Sofort::API.new
result = @sofort.pay(12.0, "Sebastian Skopp", 'http://return.url', 'reason', 'EUR', 'DE')

details example: 
=======================
details = Sofort::API.new.details("sofort_token")

read sofort documentation:
=======================
https://www.sofort.com/integrationCenter-eng-DE/content/view/full/2513#h1

