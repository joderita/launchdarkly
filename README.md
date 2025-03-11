# LaunchDarkly demo
The goal of this app is to demonstrate seamless feature releases and instant remediation/rollback of impacting changes using LaunchDarkly feature flags. By the end of this project, you'll also understand how to define specific audiences for your feautre release, giving you the ability to target specific individuals for testing purposes or groups of users based on rulesets. You can read more about instant feature flag updates in [this blog post](https://launchdarkly.com/blog/how-near-instant-feature-flag-updates-ensure-your-app/), or learn how to implement your own feature flags in [this Getting Started guide](https://app.launchdarkly.com/projects/default/get-started?env=test&selected-env=test).

**Please Note:** This demo application uses the Current weather data API from OpenWeatherMap to provide our website with various weather conditions at cities populated by our users. It also uses the LaunchDarkly SDK to add feature flag functionality to our code. As such, you will need accounts on both OpenWeatherMap and LaunchDarkly in order to complete this demo. Instructions on creating both accounts are included below. 

# How to get started with this app
1. Clone this project onto your local workstation. From a command line/terminal session:
   * Use `mkdir lddemo` to create a new directory named "lddemo" for this project
   * Use `cd lddemo` to move into your new directory
   * Use `git clone https://github.com/joderita/launchdarkly.git .` to clone this repository into your new directory
2. Get an API key from https://openweathermap.org.
   * Navigate to https://openweathermap.org and create an account using your email address
   * Verify your email address (be sure to check your Spam folder!)
   * Once verified, navigate to My API Keys under your profile name
    <img width="425" alt="Screenshot 2025-03-11 at 8 45 01 AM" src="https://github.com/user-attachments/assets/b1b95ac9-aa5e-4dba-bfee-a15d9150b702" />

   * Copy your Default API key
   * Create a `.env` file in your `lddemo` directory and add `WEATHER_API_KEY=<paste your API key here>`, replacing `<paste your API key here>` with the API key value from openweathermap.org
3. Get an SDK key from https://launchdarkly.com.
   * Navigate to https://app.launchdarkly.com/signup and create a free trial account
   * Verify your email address (be sure to check your Spam folder!) and select "Skip setup" on the resulting page to go directly to your new organization page
   <img width="223" alt="Screenshot 2025-03-11 at 12 18 18 PM" src="https://github.com/user-attachments/assets/167ebbd8-37b0-4f45-a87a-da18008303bd" />

   * From the Projects section of your org, select the Default Project and navigate to Environments. Open the menu for Test environment and select SDK key. This will automatically copy the key to your clipboard
   * In the `.env` file in your `lddemo` directory, add `LD_SDK_KEY=<paste your SDK key here>`, replacing `<paste your SDK key here>` with the SDK key value from your Test environment
4. Create a new feature flag.
   * 


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

