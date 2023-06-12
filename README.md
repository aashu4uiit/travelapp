Requirements before getting started with this Lab
- Install Python
- Install VS Code or any other IDE
- Launchdarkly account with Server side SDK installation for Python


Application Setup and Installation:
1. Clone repository: _git clone https://github.com/rmalik25/travel.git_
2. Go into _travel_ directory, where you cloned the repository
3. Edit server.py, and update SDK key value in row 9: _ldclient.set_config(Config(**sdk-key**))_
4. Update the name of the feature flag in row 29: _is_tier_3_enabled = client.variation(**flag-name**, user, False)_
5. Run Python and Launch server on Linux based systems: _pip install -r requirements && python server.py_
6. Run Python and Launch server on Windows based systems: _pip install -r requirements ; python server.py_
7. Open up browser and browse to http://127.0.0.1:5000/
8. Update _user.json_ with new values e.g. change country to "Australia" and refresh browser to see 3 clases of tickets
9. Update _user.json_ with new values e.g. change country to "China" and refresh browser to see 2 clases of tickets
  
Slack Integration: 
1. Create a separate workspace for Launchdarkly in your slack such as DemoWS
2. Create a channel where you would like to receive the notifications such as demo
3. Install Launchdarkly application from Slack app directory https://demowsworld.slack.com/apps/AKEEF9DTM-launchdarkly
4. Launchdarkly will request permission to access the workspace - Click Allow 
5. You shoud be able to see "Success" message
6. Now you can go back to Slack workspace and interact with Launchdarkly App
7. Send a message /launchdarkly account from your app 
8. Click on connect with Launchdarkly, which will take you to Launchdarkly authrize page
9. Once authrized you can start use /launchdarkly subscribe to get notifications

Datadog Events Integration: 

1. Datadog integration can be done for events,the dashboard widget, triggers, and Real User Monitoring (RUM)
2. We will configure Events and dashboard widget in this lab
3. we need to generate an API key from Datadog API keys page
4. Navigate to integration page https://app.launchdarkly.com/default/integrations
5. Search for  Datadog Events and click on add integration
6. In a new window we can configure - Name, Datadog API key, Policy and actions
7. We can save and validate configuration    


Datadog dashboard Integration: 

1. Install the LaunchDarkly integration from https://app.datadoghq.com/integrations
2. Navigate to an existing dashboard or create a new one in Datadog
3. Click the Add Widgets button to access the widget drawer
4. Search for LaunchDarkly in the Apps section of the widget drawer
5. Add the LaunchDarkly widget to your dashboard by clicking which opens the LaunchDarkly editor modal
6. Connect and authrize your LaunchDarkly account
7. Configure the widget options in the LaunchDarkly editor
8. Save the configuration to finalize the creation of the Datadog dashboard widget.