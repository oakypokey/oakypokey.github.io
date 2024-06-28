# Background
In an effort to develop my architecture skills, I decided to rewrite my splitting script and turn it into a proper application. Currently, the only two people that use it are my partner and myself but I'm still designing it with the idea that multiple people would be able to use it one day!

The idea is very similar to [2up]("https://up.com.au/2up/") from Up banking where you're able to "tackle finances together". My partner and I decided we didn't want to share an account, but given that we've been living together for the past two years, we needed an easier way to split transactions between ourselves.

In comes Multiplayer, a script that uses the Pocketsmith API to split transactions between two users and makes those transactions available to those who have been split with. It does this by creating a virtual account that the transactions are all written to. This way, you can see what has been split and it also allows us to use our own rulesets to categorize transactions!

After success with the first two versions, I have come to realise that I haven't taken it far enough after reading [this]("https://www.amazon.com.au/Architecture-Patterns-Python-Domain-Driven-Microservices-ebook/dp/B085KB31X3") book. I discovered this shiny new toy (hexagonal architecture), and decided that I wanted to use this framework for my next iteration. I may want to switch from Pocketsmith one day (who knows!) and I don't want to have to reimplement everything.

The repository is still private as I'm still trying to get to my true V1 but if you're interested in having a look-- let me know!

# Current goals


# Previous goals

~~I want to get all of my core model components defined and get all their "services" working (like splitting a transaction)~~

I managed to define Transactions, Users, Splits, and Disputes! These are the basis of _my_ application but Transactions and Users are modeled off of the Pocketsmith objects (why reinvent the wheel?)

~~I want to write some unit tests and make sure that everything is working as expected~~

I definitely think I went the wrong way round and I should have completed this first. After writing the tests, I discovered some problems with my implementation but I'm glad that everything is working intended! I got to play around with [testcontainers]("https://testcontainers.com/") which has been on my bucket list for a while!

