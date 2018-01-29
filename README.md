# kriti2108.github.io
my portfolio
library(twitteR)
library(ROAuth)

consumer_key <-"mom5978jc4SkBdpSo2AS4i20V"
consumer_secret <-"njv9uJ2aDtjNXEsHA6ZRHjMiOO1BjBjIlqnowyAWUGk4F5nTOE"
access_token <-"2995566692-Ww0YbP9p8yovywRNpFjmLQVYERj9gUsX4b5Z81H"
access_secret <- "7GBqgDJgaqFKKnZczUxdFIAEme4fK6Uko7k1lmOBIQXiJ
"

setup_twitter_oauth(consumer_key,consumer_secret,access_token,access_secret)

cred <- OAuthFactory$new(consumerKey = consumer_key,
        consumerSecret = consumer_secret,
	  requestURL='https://api.twitter.com/oauth/request_token',
	  accessURL='https://api.twitter.com/oauth/access_token',
	  authURL='https://api.twitter.com/oauth/authorize')

cred$handshake(cainfo="cacert.pem")

