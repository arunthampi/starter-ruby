# Welcome to the Ruby Guild!

As members of the Ruby guild, you will be working through the challenges of TwilioQuest using the Ruby programming language.  This project is pre-configured to do some interesting Twilio stuff using Ruby and the light-weight Sinatra web framework.

## Setting Up

We assume that before you begin, you will have [Ruby](http://www.ruby-lang.org/en/) and [RubyGems](http://rubygems.org/) installed on your system.  If you are on OS X, this should already be done for you.  On Windows, [you will need to do some work](https://forwardhq.com/support/installing-ruby-windows).

Before you can run this project, you will need to set three system environment variables.  These are:

* `TWILIO_ACCOUNT_SID` : Your Twilio "account SID" - it's like your username for the Twilio API.  This and the auth token (below) can be found [on your account dashboard](https://www.twilio.com/user/account).
* `TWILIO_AUTH_TOKEN` : Your Twilio "auth token" - it's your password for the Twilio API.  This and the account SID (above) can be found [on your account dashboard](https://www.twilio.com/user/account).
* `TWILIO_NUMBER` : A Twilio number that you own, that can be used for making calls and sending messages.  You can find a list of phone numbers you control (and buy another one, if necessary) [in the account portal](https://www.twilio.com/user/account/phone-numbers/incoming).

For Mac and Linux, environment variables can be set by opening a terminal window and typing the following three commands - replace all the characters after the `=` with values from your Twilio account:

    export TWILIO_ACCOUNT_SID=ACXXXXXXXXX
    export TWILIO_AUTH_TOKEN=XXXXXXXXX
    export TWILIO_NUMBER=+16518675309

To make these changes persist for every new terminal (on OS X), you can edit the file `~/.bash_profile` to contain the three commands above.  This will set these environment variables for every subsequent session. Once you have edited the file to contain these commands, run `source ~/.bash_profile` in the terminal to set up these variables.

On Windows, the easiest way to set permanent environment variables (as of Windows 8) is using the `setx` command.  Note that there is no `=`, just the key and value separated by a space:

    setx TWILIO_ACCOUNT_SID ACXXXXXXXXX
    setx TWILIO_AUTH_TOKEN XXXXXXXXX
    setx TWILIO_NUMBER +16518675309

## Developing on Nitrous.IO

Start hacking on this app on [Nitrous.IO](https://www.nitrous.io/?utm_source=github.com&utm_campaign=twilio-starter-ruby&utm_medium=hackonnitrous) in seconds:

[![Hack twilio/starter-ruby on
Nitrous.IO](https://d3o0mnbgv6k92a.cloudfront.net/assets/hack-l-v1-3cc067e71372f6045e1949af9d96095b.png)](https://www.nitrous.io/hack_button?source=embed&runtime=rails&repo=twilio%2Fstarter-ruby&file_to_open=README.nitrous.md)

## Running the application

[Download the project source code directly](https://github.com/twilio/starter-ruby/archive/master.zip) or [clone the repository on GitHub](https://github.com/twilio/starter-ruby).  Navigate to the folder with the source code on your machine in a terminal window.

You will first need to install the application's dependencies.  You can do this manually using RubyGems, or you can install them using [Bundler](http://bundler.io/) and the include gem file.  To install via bundler, type:

    bundle install

To install the gems manually (if you don't know what bundler is and/or don't have it installed), type the following commands:

    gem install twilio-ruby
    gem install sinatra

Now, you should be able to launch the application.  From your terminal, run `ruby app.rb`.  This should launch your sinatra application on port 4567 - [visit that URL on your local host](http://localhost:4567/).  Enter your mobile number in the fields provided, and test both SMS text messages and phone calls being sent to the mobile number you provide.


## Begin Questing!
This is but your first step into a larger world.  [Return to TwilioQuest](http://quest.twilio.com) to continue your adventure.  Huzzah!
