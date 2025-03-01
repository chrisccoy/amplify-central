---
title: Integrate with Amplify
linkTitle: Integrate with Amplify
weight: 300
---
Amplify is built using the API-first pattern, then CLI, and lastly UI. Because of this, you can use Amplify APIs to build your own integration patterns.

## Amplify Central APIs definition and usage

Amplify APIs are described in the OAS 3.0 specification:

* (US region) <https://apicentral.axway.com/apis/docs>
* (EU region) <https://central.eu-fr.axway.com/apis/docs>

The APIs can be used either programmatically or using the [Axway Central CLI](/docs/integrate_with_central/cli_central/).

All APIs are secured using a JSON Web Token (JWT).

* When using the APIs, you must use the following url / parameters to get your token:

    * Auth URL: <https://login.axway.com/auth/realms/Broker/protocol/openid-connect/auth>
    * Grant Type: Implicit
    * Client ID: apicentral
    * Enter your username / password to validate your credentials

* When using the Axway Central CLI, this token is automatically retrieved when connected to Amplify using the `axway auth login` command.

Once you get your token, you can start manipulating the Amplify resources.

When using APIs programmatically, the following headers are required:

* **X-Axway-Tenant-Id**: contains your organization identifier. Go to <https://platform.axway.com> and navigate to the **Organization** tile to find the Organization ID.
* **authentication**: contains your JWT token obtained previously.

## What can you do once you integrate with Amplify

It all depends on what you want to accomplish with the platform:

* If you want to manipulate Amplify resources, the APIs or [Axway Central CLI](/docs/integrate_with_central/cli_central/cli_command_reference/) can be used to add/update/remove resources.

* If you want to trigger a flow when specific events happen in Amplify, you will need a [webhook integration](/docs/integrate_with_central/webhook/).
