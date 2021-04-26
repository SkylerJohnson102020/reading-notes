# What is OAuth? 

https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

- SSO - single sign-on

- 2FA - two-factor authentication

- MFA - multi-factor authentication

- OAuth - an open-standard authorization framework allowing unrelated servers to connect and securely allow authenticated access to assests without exposing or leaking vital information. 

- This was started by Twitter and Google. Released in 2010 as an open standard. Amazon, Facebook, Instagram, and several others use this.

- Example - using google to log into multiple different websites. Or sending cloud stored files through your email. Two or more services being used for one transaction.

- OAuth is basically at least two sites that are unrelated working together with a user to achieve one result. **OAuth is about authorization, NOT authentication.** One source authenticates, the other that the user is trying to access is authorizing. The authorizer only has temporary access to this information.

- OpenID - an OAuth authentication layer

- SAML - Security Assertion Markup Language - more used for Saleforce.

- TLS - Transport Layer Security

# Authenication and Authorization Flows

https://auth0.com/docs/flows

- Auth0 - uses the OIDC(OpenID Connect) protocol in addition to the OAuth 2.0 version framework.

- Authentication = Verification

- Authorization = Verifies who gets in., second server

- Authorization Code Flows - the exchange of an authorization code in exchange for an access token.

- PKCE - Proof Key for Code Exchange - an additional layer for mobile apps, mainly single page apps.

- Implicit flow - intended for public clients. sites unable to store client secrets

- Hybrid flow - combines implicit and code flow with form post.

- Client credentials flow - (M2M) - machine to machine. This authorizes an app instead of the user.

- Device Flow - Authentication through devices. Gives you a temp code to authorize another device.

- Resource Owner Password Flow - sharing information. Recommended only for re-direct flows.

[code301 Reading Notes](/301/code301Table.md)