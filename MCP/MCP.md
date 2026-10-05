# Connect to Essbase through MCP

## Introduction

In this optional lab, you will connect an approved AI client to the Essbase MCP server with read-only access. You will discover the available tools and ask the client to list the Essbase applications available to your user, including the PeakGear application imported in Lab 3.

Estimated Time: 20 minutes

### About Essbase MCP

The Essbase MCP server exposes Essbase tools to compatible AI clients. The `viewer` access profile exposes read-only tools. Your Essbase permissions still determine which applications you can see.

### Objectives

In this lab, you will:

- Verify the Essbase MCP endpoint for your environment.
- Connect an approved AI client with the `viewer` profile.
- List the Essbase applications available to your user.

### Prerequisites

This lab assumes you have:

- Access to the PeakGear application imported in Lab 3.
- An approved MCP-compatible AI client.
- The Essbase MCP endpoint and approved authentication details for your environment.
- Confirmation from your workshop administrator that the embedded Essbase environment exposes the MCP service.

## Task 1: Verify the Essbase MCP Endpoint

1. Obtain the Essbase MCP base URL and authentication instructions from your workshop administrator.

2. Confirm that the endpoint is available in your environment. The standard Essbase endpoint has the form `https://<essbase-server>/essbase/rest/v1/ess-mcp`.

3. Add `?profile=viewer` to the endpoint URL for this lab.

    > **Note:** Use the endpoint confirmed for your embedded environment. Do not assume that the standard URL is enabled in every Lakehouse.

## Task 2: Connect an Approved AI Client

1. In your approved AI client, add an MCP connection using the endpoint with `?profile=viewer`.

2. Complete the authentication flow supplied for your client and environment.

3. Refresh the connection and confirm that the Essbase MCP tools are available.

    > **Note:** Keep client secrets and access tokens out of the LiveLab, screenshots, and source files.

## Task 3: List the Available Essbase Applications

1. Ask the client: **List the Essbase applications available to me.**

2. Confirm that the response includes the PeakGear application imported in Lab 3.

3. If the application is missing, verify the signed-in user and the user's Essbase application permissions.

You have connected an AI client to Essbase with read-only access and confirmed that the PeakGear application is visible.

## Learn More

- [Introducing Essbase MCP Server](https://docs.oracle.com/en/database/other-databases/essbase/26/esmcp/introducing-essbase-mcp-server.html)
- [Choose an Access Profile](https://docs.oracle.com/en/database/other-databases/essbase/26/esmcp/mcp-access-profiles.html)
- [Connect an AI Client](https://docs.oracle.com/en/database/other-databases/essbase/26/esmcp/connect-ai-client.html)

## Acknowledgements

* **Author** - Ty Wolber, Cloud Engineer
* **Last Updated By/Date** - Ty Wolber, October 2026
