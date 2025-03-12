# LaunchDarkly demo
The goal of this app is to demonstrate seamless feature releases and instant remediation/rollback of impacting changes using LaunchDarkly feature flags. By the end of this project, you'll also understand how to define specific audiences for your feautre release, giving you the ability to target individuals for testing purposes or groups of users based on rulesets. You can read more about instant feature flag updates in [this blog post](https://launchdarkly.com/blog/how-near-instant-feature-flag-updates-ensure-your-app/), or learn how to implement your own feature flags in [this Getting Started guide](https://app.launchdarkly.com/projects/default/get-started?env=test&selected-env=test).

**Please Note:** This demo application uses the Current weather data API from OpenWeatherMap to provide our website with various weather conditions at cities populated by our users. It also uses the LaunchDarkly SDK to add feature flag functionality to our code. As such, you will need accounts on both OpenWeatherMap and LaunchDarkly in order to complete this demo. Instructions on creating both accounts are included below. 

# Get started with this app
1. **Clone this project onto your local workstation. From a command line/terminal session:**
   * Use `mkdir lddemo` to create a new directory named "lddemo" for this project
   * Use `cd lddemo` to move into your new directory
   * Use `git clone https://github.com/joderita/launchdarkly.git .` to clone this repository into your new directory
2. **Get an API key from https://openweathermap.org.**
   * Navigate to https://openweathermap.org and create an account using your email address
   * Verify your email address (be sure to check your Spam folder!)
   * Once verified, navigate to My API Keys under your profile name
    <img width="425" alt="Screenshot 2025-03-11 at 8 45 01 AM" src="https://github.com/user-attachments/assets/b1b95ac9-aa5e-4dba-bfee-a15d9150b702" />

   * Copy your Default API key
   * Create a `.env` file in your `lddemo` directory and add `WEATHER_API_KEY=<paste your API key here>`, replacing `<paste your API key here>` with the API key value from openweathermap.org
3. **Get an SDK key from https://launchdarkly.com.**
   * Navigate to https://app.launchdarkly.com/signup and create a free trial account
   * Verify your email address (be sure to check your Spam folder!) and select "Skip setup" on the resulting page to go directly to your new organization page
   <img width="223" alt="Screenshot 2025-03-11 at 12 18 18 PM" src="https://github.com/user-attachments/assets/167ebbd8-37b0-4f45-a87a-da18008303bd" />

   * From the Projects section of your org, select the Default Project and navigate to Environments. Open the menu for Test environment and select SDK key. This will automatically copy the key to your clipboard
   <img width="413" alt="Screenshot 2025-03-11 at 12 31 05 PM" src="https://github.com/user-attachments/assets/c99dbee1-b765-43ee-a771-a0604d5b7a6f" />

   * In the `.env` file in your `lddemo` directory, add `LD_SDK_KEY=<paste your SDK key here>`, replacing `<paste your SDK key here>` with the SDK key value from your Test environment
4. **Create and configure a virtual environment to run your app locally.**
   * If you don't already have Python installed on your workstation, download it now. You can download it directly from the Python website [here](https://www.python.org/downloads/) and follow your system's installation prompts
   * Use the command below appropriate for your operating system to create and launch a virtual environment on your workstation:
     * For Mac or Linux systems: `python3 -m venv .venv && source .venv/bin/activate`
     * For Windows systems: `py -m venv .venv` and then `source .venv/Scripts/activate`
   * Use `pip install requests python-dotenv Flask launchdarkly-server-sdk` to install the necessary packages to run our application.
   * Use `pip freeze > requirements.txt` to create a file that lets our host server know what packages it needs installed.
   * 




4. **Create a new feature flag.**
   * Navigate to the Flags section of LaunchDarkly and select "Create flag"
   * Name your flag "Wind Speeds". This should cause the "Key" value to autopopulate; ensure that the value is "wind-speeds"
   * 


* create a new feature flag named "wind_speed"

In a terminal session, create .venv file
Launch virtual environment
Install Python, Flask, JavaScript?
python server.py to start app
Open browser to localhost:8000
Enter a city
Toggle feature flag, watch the magic happen

