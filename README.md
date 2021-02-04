# DetectX plugin for Watchman Monitoring

This plugin requires a scheduled run of DetectX CLI writing to /Library/Mac-MSP/Gruntwork/detectx.txt. I used the launchd example here as a model: https://github.com/munkireport/detectx#detectx-module

I should figure out a more appropriate/general place to drop the output. 

Right now the plugin only mirrors the latest output to the dashboard, no alerting or anything. 

Next steps: 
1. learn some python 
2. switch the DetectX command in the LaunchDaemon to produce .json
3. have the plugin read the json and produce some useful output
5. have the plugin check the json for a non-empty "infections" array & exit 2 or
5. exit 0

