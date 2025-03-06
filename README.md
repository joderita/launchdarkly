# LaunchDarkly demo
The goal of this app is to demonstrate LaunchDarkly's feature flags, highlighting their capabilities to instantly release a new feature, remediate/rollback changes in the event of customer impact, and target/limit visibility of a feature to specific audiences. You can read more about instant feature flag updates in [this blog post](https://launchdarkly.com/blog/how-near-instant-feature-flag-updates-ensure-your-app/), or learn how to implement your own feature flags in [this Getting Started guide](https://app.launchdarkly.com/projects/default/get-started?env=test&selected-env=test).

# Get started with this app
Clone this repository

Create an openweathermap.org account:
* verify your email address
* grab API key, save it in .env as "WEATHER_API_KEY".

Create a LaunchDarkly account:
* grab client API key, save it in .env as "LD_API_KEY"
* create a new feature flag named "wind_speed"

In a terminal session, create .venv file
Launch virtual environment
Install Python, Flask, JavaScript?
python server.py to start app
Open browser to localhost:8000
Enter a city
Toggle feature flag, watch the magic happen
