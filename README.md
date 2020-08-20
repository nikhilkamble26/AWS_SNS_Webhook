# AWS_SNS_Webhook
There are many services out there that will let you programmatically send SMS messages. One of the more popular is Twilio, and they have a great API and a python client that's easy to use. There's an interesting quora thread with several other suggestions as well.

Another option is to use Amazon's Simple Notification Service (SNS), which also supports sending SMS messages. I recently incorporated this into a project, and thought I'd share.
Step 1: API key + boto3

If you're already using AWS, you've probably jumped through these hoops. I'm not going to walk you through them, but just realize you need to figure out how to sign up for an AWS account and get some api keys.

The second part of this is boto3, amazon's python sdk.

pip install boto3

Boto's quickstart guide should help, and it also includes some info on getting boto configured.
Step 2: Send your message

At the bare minimum, you can just send a message directly to a single phone number. 
