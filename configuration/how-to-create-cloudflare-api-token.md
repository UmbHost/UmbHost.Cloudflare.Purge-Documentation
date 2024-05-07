# How to Create Cloudflare API Token

The recommended approach is to create a scoped Cloudflare API Token, you can do this by browsing to the Cloudflare User API Tokens page:

{% embed url="https://dash.cloudflare.com/profile/api-tokens" %}

On this page click the `Create Token` button and then scroll down and click `Get Started` next to `Create Custom Token`

On the following page enter the following details:

| Key            | Value                                             |
| -------------- | ------------------------------------------------- |
| Token name     | A unique name to identify the token in Cloudflare |
| Permissions    | Zone -> Cache Purge -> Purge                      |
| Zone Resources | Include -> Specific Zone -> YOURZONENAME          |

Click the `Continue to summary` and then on the summary page click `Create token` next copy the token and place it in the `Auth Key` [appsetting](./)
