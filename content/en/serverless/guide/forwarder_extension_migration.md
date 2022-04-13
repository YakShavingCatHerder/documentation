---
title: Migrating from the Datadog Forwarder to the Datadog Lambda Extension
kind: guide
---
## Overview

<div class="alert alert-warning">Datadog recommends migrating your dev and staging applications first and migrating production applications one by one.</div>

This guide explains how to migrate from the [Datadog Forwarder][1] to the [Datadog Lambda Extension][2]. See [why should you migrate][3] if you are unsure.

## Migrate

To migrate, follow the instructions below for the installation method you use. For additional details, you can compare the [installation instructions using the Datadog Lambda Extension][4] against the [instructions using the Datadog Forwarder][5].

TODO: Update the instructions below

{{< tabs >}}
{{% tab "Serverless Framework" %}}

Remove the resource name of the Forwarder from your `serverless.yml` file.

{{% /tab %}}
{{% tab "AWS SAM" %}}

Remove the resource name of the Forwarder from your `template.yml` file.

{{% /tab %}}
{{% tab "AWS CDK" %}}

Remove the resource name of the Forwarder from your CDK stack.

{{% /tab %}}
{{% tab "Zappa" %}}

Manually remove the subscription from the AWS console.

{{% /tab %}}
{{% tab "Chalice" %}}

Manually remove the subscription from the AWS console.

{{% /tab %}}
{{% tab "Datadog CLI" %}}

Manually remove the subscription from the AWS console.

{{% /tab %}}
{{% tab "Container Image" %}}

Manually remove the subscription from the AWS console.

{{% /tab %}}
{{% tab "Custom" %}}

Manually remove the subscription from the AWS console.

{{% /tab %}}
{{< /tabs >}}

[1]: /serverless/libraries_integrations/forwarder/
[2]: /serverless/libraries_integrations/extension/
[3]: /serverless/guide/extension_motivation/
[4]: /serverless/installation/
[5]: /serverless/guide#install-using-the-datadog-forwarder
