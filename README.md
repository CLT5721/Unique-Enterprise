# Unique-remitone8888
Wise uses the standard OAuth 2.0 protocol for authentication and authorization.
Sandbox API location
https://api.sandbox.transferwise.tech
Production API location
https://api.transferwise.com
{
       "access_token": "01234567-89ab-cdef-0123-456789abcdef",
       "token_type": "bearer",
       "refresh_token": "01234567-89ab-cdef-0123-456789abcdef",
       "expires_in": 43199,
       "scope": "transfers",
       "created_at": "2020-01-01T12:33:33.12345Z"
     }
     curl -X POST https://api.sandbox.transferwise.tech/oauth/token \
      -U '<api-client-id>:<api-client-secret>' \
      -d '{
           "grant_type": "refresh_token",
           "refresh_token": {{refresh token}}
          }'
          If the consumer has recycled their account, previously stored tokens will fail with error code 400 and the error:
{
   "error": "invalid_grant",
   "error_description": "Invalid user credentials."
}
Then push them by linking to your existing Wise account flow.
User logs in to Wise.
User agrees to provide access permission to partner applications.
The consumer will be redirected back to the preconfigured redirect_url, including an authorization code that can be used to generate a consumer token. For example https://www.yourbank.com/transferwise-link-page/?code=[CODE]&profileID=[PROFILE_ID]
These steps are explained in more detail below.

1. Your banking application redirects users to the Wise authorization page
Your website or app opens the following URL in a user's browser - Environmental Information

2. User logs into Wise
If the user is not logged in to the browser they are using, the user is shown our usual login screen. If enabled for users, they will also be prompted to complete our two-factor authentication process.
3. The user agrees to grant access permission and we will forward it to you redirect_url
Once the user gives your application permission to connect to Wise and access their data, the user is redirected back to your redirect_url using the generated code query string value. For example

https://www.yourbank.com/transferwise-link-page/?code=[CODE]&profileID=[PROFILE_ID]

Your site or service can then use this code to obtain an access token to perform operations on behalf of the user account described in the Authorization code section for exchanging API tokens

If you build your Wise integration as a native mobile app, the redirect URL should be able to return the user to the correct location in the app using a "deep link" based on a custom URL scheme defined by the mobile app.
