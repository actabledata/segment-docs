---
rewrite: true
---
[Xtremepush](https://xtremepush.com/?utm_source=segmentio&utm_medium=docs&utm_campaign=partners) is a complete digital engagement platform. Empowering global brands to create personalised, real-time experiences for their customers across mobile, web, email, SMS and social. Xtremepush's clients are increasing revenue through data-driven, contextually-relevant interactions. The software is flexible, reliable and quick to deploy, backed up by a team of expert strategists and technical support.

This destination is maintained by Xtremepush. For any issues with the destination, please [reach out to their team](mailto:support@xtremepush.com).

_**NOTE:** The Xtremepush Destination is currently in beta, which means that they are still actively developing the destination. This doc was last updated on April 05, 2019. If you are interested in joining their beta program or have any feedback to help improve the Xtremepush Destination and its documentation, please [let  their team know](mailto:support@xtremepush.com)!_


## Getting Started

<!-- {{>connection-modes}} -->

1. From your Segment UI's Destinations page click on "Add Destination".
2. Search for "Xtremepush" within the Destinations Catalog and confirm the Source you'd like to connect to.
3. Drop in the "API Key" into your Segment Settings UI which you can find from your Xtremepush Project under *Settings > Integrations* as described in the [user guide](https://support.xtremepush.com/hc/en-us/articles/360001351637-Generating-API-Tokens).

## Identify

If you haven't had a chance to review our spec, please take a look to understand what the [Identify method](https://segment.com/docs/spec/identify/) does. An example call would look like:

```
analytics.identify('userId123', {
  email: 'john.doe@segment.com',
  phone: '1234567890',
  firstName: 'John'
});
```

When you identify a user, we’ll pass that user’s information to Xtremepush and will try to update or create a new user based on whether a Profile exists with that `user_id`.

Some special traits will also be used as additional user identifiers:

| Segment Trait | Xtremepush User Identifier |
| ------------- | -------------------------- |
| email         | email                      |
| phone         | mobile_number              |

For any additional traits you want to save you should create [User Profile Attributes](https://support.xtremepush.com/hc/en-us/articles/360000850789-User-Profiles-Quick-Start-Guide#AddingOtherAttributestoUserProfiles) in your Xtremepush Project.

If a trait does not match a custom Xtremepush User Profile Attribute and is not recognized as a User Identifier it will be ignored.

## Track

If you haven't had a chance to review our spec, please take a look to understand what the [Track method](https://segment.com/docs/spec/track/) does. An example call would look like:

```
analytics.track('Product Purchased', {
  productName: 'Some Product'
})
```

Track calls will be sent to Xtremepush as a `event hits`, so you can use it to [trigger a campaign](https://support.xtremepush.com/hc/en-us/articles/207743999-Event-Tab) for a user.

Event properties can be used as merge tags in the message content. You can also define additional rules on where to trigger the campaign based on event properties value.

## Enabling Push and In-App Notifications
To enable Xtremepush push and in-app notifications you will also need to to install the relevant [Xtremepush SDKs](https://support.xtremepush.com/hc/en-us/categories/200812171-SDKs).