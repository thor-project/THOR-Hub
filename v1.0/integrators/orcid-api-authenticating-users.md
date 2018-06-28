---
title: "Authenticating using ORCID"
excerpt: ""
---
ORCID uses the OAuth2 protocol for authentication and authorisation.  This is a user centric authentication mechanism that allows users fine grained control over what third parties can and cannot do with their ORCID record. Actions that require user authorisation use the three-legged approach, as does authenticating users.  It works like this:

- Your website directs the user to ORCID using a specially crafted request containing details of the permissions you would like the user to grant you.  E.g. read or update
- The user authenticates to ORCID, if not already signed in
- The user grants (or denies!) permission to your application
- ORCID redirects the user back to your website with an *authorization code*
- You exchange the authorisation code for an *access token* using the ORCID OAuth API
- You include the access token in any subsequent requests you make

Implementing this in code is easier than it sounds.  
[block:api-header]
{
  "type": "basic",
  "title": "External documentation"
}
[/block]
More details can be found in the [ORCID OAuth documentation](https://members.orcid.org/api/oauth2).