---
title: Overview of API support in Azure Static Web Apps
description: Learn what API features Azure Static Web Apps supports
services: static-web-apps
author: craigshoemaker
ms.service: static-web-apps
ms.topic:  conceptual
ms.date: 06/14/2022
ms.author: cshoe
---

# Overview of API support in Azure Static Web Apps

Front end web applications often call back end APIs for data and services. Azure Static Web Apps provides built-in serverless API endpoints via integration with Azure services.

Key features of Azure Static Web Apps APIs include:

- **Integrated security** with direct access to user [authentication and role-based authorization](user-information.md) data.

- **Seamless routing** that makes the `/api` route available to the front-end web app without requiring custom CORS rules.

## API options

The following Azure services can be integrated with Azure Static Web Apps:

| Service | Managed | Bring your own |
| --- | --- |
| [Azure Functions](apis-functions.md) | ✔ | ✔ |
| [Azure API Management](apis-api-management.md) |  | ✔ |
| [Azure App Service](apis-app-service.md) |  | ✔ |
| [Azure Container Apps](apis-container-apps.md) |  | ✔ |

- **Managed APIs**: By default, Azure Static Web Apps automatically integrates with Azure Functions as an API backend. You deploy an API with your static web app without managing a separate Azure Functions resource.
- **Bring your own APIs**: You can integrate your static web app with existing APIs hosted in Azure Functions, API Management, App Service, or Container Apps. You manage and deploy the API resources yourself.

Each static web app environment can only be configured with one type of backend API at a time.

> [!NOTE]
> Bring your own APIs is only available in the Azure Static Web Apps Standard plan. Built-in, managed Azure Functions APIs are available in all Azure Static Web Apps plans.

## Next steps

> [!div class="nextstepaction"]
> [Add an API](add-api.md)
