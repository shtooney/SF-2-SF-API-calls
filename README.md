# SF-2-SF-API-calls
Great to show the openness of the Salesforce Platform by having 2 different Salesforce orgs talk to each other

**Step 1: ** Sign up for 2 different Developer orgs (so do it twice): https://developer.salesforce.com/signup

**Step 2: ** Set up Connected App in Org 1
--- Callback URL: https://login.salesforce.com/services/oauth2/callback (different if custom domain)
--- Rights: Full access (full), Access your basic information (id, profile, email, address, phone), Access and manage your data (api), Perform requests on your behalf at any time (refresh_token, offline_access)

**Step 3: ** Optional to play it safe: Set Remote Site Settings for each org of the org's URL - i.e., https://na34.salesforce.com	or your custom domains

**Step 4: ** Review and provide code (with comments):
Code Applicable for Org 1:
--- ExampleManager class
Code Applicable for Org 2: 
--- Integrate class (with OAuth2 helper class)
--- TestShow page
