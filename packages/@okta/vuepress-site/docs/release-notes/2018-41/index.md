---
title: Okta API Products Release Notes
---

## 2018.41

| Change                                                                                                               | Expected in Preview Orgs | Rollout to Production Orgs Expected to Start |
| -------------------------------------------------------------------------------------------------------------------- | ------------------------ | -------------------------------------------- |
| [Rate Limit Notifications for One App and Enterprise](#rate-limit-notifications-for-one-app-and-enterprise)                            | October 10, 2018       | October 15, 2018                             |
| [OIDC Clients Can Initiate Logout with Expired Token](#oidc-clients-can-initiate-logout-with-expired-token)                            | October 10, 2018       | October 15, 2018                             |
| [Change to User Link Editing Permissions](#change-to-user-link-editing-permissions)                            | October 10, 2018       | October 15, 2018                             |
| [Bugs Fixed in 2018.41](#bugs-fixed-in-2018-41)                                                                       | October 10, 2018         | October 15, 2018                             |
| [Previously Released Early Access Features 2018.41 Update](#previously-released-early-access-features-2018-41-update) | Available Now            | Available Now                                |

### Rate Limit Notifications for One App and Enterprise

When an org reaches its [rate limit](/docs/reference/rate-limits/), the admin console will display a banner and the admin(s) will receive an email notification. These notifications will only appear on One App and Enterprise organizations. <!--OKTA-185719-->

### OIDC Clients Can Initiate Logout with Expired Token

Client-initiated [logout](/docs/reference/api/oidc/#logout) now succeeds even when the ID token is no longer valid. <!--OKTA-131652-->

### Change to User Link Editing Permissions

Editing the [link](/docs/reference/api/users/#links-object) between users now requires edit permissions for all users involved. <!--OKTA-186702-->

### Bugs Fixed in 2018.41

* Queries to the `/logs` [endpoint](/docs/reference/api/system-log/#list-events) with values for `since` and `until` that did not specify the time to milliseconds would sometimes return events outside of the specified time range. (OKTA-191533)
* Responses from the `/events` [endpoint](/docs/reference/api/events/#list-events) would sometimes omit milliseconds from the `published` field. (OKTA-192568)

### Previously Released Early Access Features 2018.41 Update

The following features have already been released as Early Access. To enable them, contact [Support](https://support.okta.com/help/open_case).

| Early Access Features Available Now
| :------------------------------------------------- |
| [Custom URL Domains](#custom-url-domains-are-in-early-access)|
| [Custom Okta-hosted Sign-In Page](#custom-okta-hosted-sign-in-page-is-in-early-access)|
| [Custom Error Page](#custom-error-page-is-in-early-access)|
| [Linked Objects API](#linked-objects-api-in-early-access-ea) |
| [Token Management API](#token-management-api-is-in-early-access-ea) |
| [User Consent for OAuth 2.0 and OpenID Connect Flows](#user-consent-for-oauth-20-and-openid-connect-flows-in-early-availability-ea) |
