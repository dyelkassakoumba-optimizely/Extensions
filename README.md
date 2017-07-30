## Universal Analytics Debugger

This analytics integration allows you to enable troubleshooting custom events to identify potential reasons for discrepencies between Optimizely and Universal analytics.

## Setup

1.	Use config.json to import this custom analytics integration.

2.	Create 3 custom events within your project using the folowing API names:
	-	step1_ga_wait_success
	-	step2_ga_ready
	-	step3_ga_tracking_success

4. Use the above custom event to define the three troubleshooting metrics within your metrics builder for the experiment you want to troubleshoot.

5. Enable this integration for the experiment you would like to troubleshoot.

## Reading the results

When enough visitors have been included in the experiment the results page will contain the following information.

% step1_ga_wait_success: Number of users for which the troubleshooting script ran.
% step2_ga_ready: Number of users for which the GA object was defined
% step3_ga_tracking_success: Number of users for which the event got sent successfully.
