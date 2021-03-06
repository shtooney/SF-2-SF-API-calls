# SF-2-SF-API-calls
##### Enjoy openness of the Platform by having 2 different Salesforce orgs talk to each other!

1. **Step 1:** Sign up for 2 different Developer orgs (so do it twice): https://developer.salesforce.com/signup
2. **Step 2:** Set up Connected App in Org 1
    * Callback URL: https://login.salesforce.com/services/oauth2/callback (different if custom domain)
    * Rights: Full access (full), Access your basic information (id, profile, email, address, phone), Access and manage your data (api), Perform requests on your behalf at any time (refresh_token, offline_access)
    * If you haven't set it up before: Go to Create >> Apps >> Click New under Connected Apps at the bottom. Put in your Connected App Name, API Name, Enable OAuth settings, Callback URL above, and select security parameters mentioned above 
3. **Step 3:** Optional to play it safe: Set Remote Site Settings for each org of the org's URL - i.e., https://na34.salesforce.com	or your custom domains. If you haven't set it up before: Go to Security Controls >> Remote Site Settings >> and do New Remote Site
4. **Step 4:** Review and provide code (with comments):
    * _Code Applicable for Org 1:_
       * ExampleManager class
    * _Code Applicable for Org 2:_ 
       * Integrate class (with OAuth2 wrapper class)
       * TestShow page
