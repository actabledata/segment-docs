---
# The end name should be similar to `Slack  Destination`
title: Actable Predictive Destination
hide-boilerplate: true
hide-dossier: true
---

<!-- This template is meant for Actions-based destinations that do not have an existing Classic or non-Actions-based version. For Actions Destinations that are a new version of a classic destination, see the doc-template-update.md template. -->

{% include content/plan-grid.md name="actions" %}

<!-- Include a brief description of the destination here, along with a link to your website. -->

Actable Predictive is a standalone marketing-specific customer prediction tool. It trains models on your customer's behavioral data, and provide regular automated scoring of new data against those models. The scoring output is tailored to drive higher levels of customer engagement, lower levels of churn, and increased incidence of purchases. 

Read more at [actable.com](https://www.actable.com/).

<!-- This include describes the requirement of A.js 2.0 or higher for Actions compatibility, and is required if your destination has a web component. -->

{% include content/ajs-upgrade.md %}

<!-- In the section below, explain the value of this actions-based destination. If you don't have a classic version of the destination, remove this section. -->

## Benefits of Actable Predictive (Actions)

Actable Predictive (Actions) provides the following benefits:

- **Unlock the value of using Segment's event specification by generating powerful customer predictions.**  The Actable Segment Destination provides a low friction way to pipeline data to Actable for customer predictions. 
- **Pair the Actable Destination with the Actable Source to route customer predictions back to Segment**. Use Actable's models to create  intelligent marketing campaigns powered by ML by using Segment to send scored customer records to operational destinations. Or, pair it with Segment Personas to combine those scores with other traits, and sync audiences.  

<!-- The section below explains how to enable and configure the destination. Include any configuration steps not captured below. For example, obtaining an API key from your platform and any configuration steps required to connect to the destination. -->

## Getting started

1. From the Segment web app, click **Catalog**, then click **Destinations**.
2. Find the Destinations Actions item in the left navigation, and click it.
3. Click **Configure Actable Predictive**.
4. Configure the applicable Sources to connect to Actable Predictive (Actions). Actable requires email engagement data, web/app activity data, and purchase data to generate scores. There is a bespoke action for each data source, as well as a generic action to permit adhoc mapping of events.

<!-- The line below renders a table of connection settings (if applicable), Pre-built Mappings, and available actions. -->

{% include components/actions-fields.html %}

<!--
Additional Context

Include additional information that you think will be useful to the user here. For information that is specific to an individual mapping, please add that as a comment so that the Segment docs team can include it in the auto-generated content for that mapping.
-->