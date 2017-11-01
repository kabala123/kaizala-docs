---
title: Kaizala APIs
description: List of APIs that Kaizala exposes to allow integration with 3rd party systems
topic: Reference
author: nitinjms
---

# Kaizala API Documentation

Before you get started, please refer to [Setup for using the Kaizala Connectors](setup.md)

## Root Domain

The root domain for invoking the Kaizala APIs is:

    {endpoint-url}
    
|            	| Parameter         	| Type   	| Optional? 	| Description |
| :---: | :---: | :---: | :---:	| :--- |
| Endpoint url 	| `endpoint-url`     	| String 	| No        	| After successful authentication during the generation of access tokens, you get an endpoint url is to use as an api-base-url for making subsequent API calls	|

> [!NOTE]
> While querying any Kaizala API if you can get **HTTP status code:308** indicating that the user's endpoint-url is changed, review the Response header field which contains the new endpoint-url.

### API End-points

The Kaizala API runs on the secure Microsoft Azure cloud, and interacts with the Kaizala platform to perform various actions for end users.
The API works with the following Kaizala resources:

*   [/groups](groups.md)
*   [/subGroups](subGroups.md)
*   [/members](members.md)
*   [/messages](messages.md)
*   [/media](media.md)
*   [/actions](actions.md)
*   [/subscribers](subscribers.md)

### WebHooks

The Microsoft Kaizala API also provides a way for developers to register for specific events within the Kaizala platform via WebHooks.

*   [/webhook](webHooks.md)

### Postman Collection

In order to test our APIs, as well as understand Kaizala API schema, you can import postman collection containing samples and schema for all the Microsoft Kaizala APIs:


[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/f68a8abec784cc00b0b9#?env%5BKaizala-APIs-environment%5D=W3siZW5hYmxlZCI6dHJ1ZSwia2V5IjoibW9iaWxlLW51bWJlciIsInZhbHVlIjoiKzkxOTkxMDg3MDAwNSIsInR5cGUiOiJ0ZXh0In0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJhY2Nlc3MtdG9rZW4iLCJ2YWx1ZSI6IiIsInR5cGUiOiJ0ZXh0In0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJ0ZXN0LWdyb3VwLWlkIiwidmFsdWUiOiIiLCJ0eXBlIjoidGV4dCJ9LHsiZW5hYmxlZCI6dHJ1ZSwia2V5IjoibW9iaWxlLW51bWJlci0yIiwidmFsdWUiOiIrOTExMTk5OTk5OTk5IiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6ImFwaS1yb290IiwidmFsdWUiOiJodHRwczovL2FwaS5rYWl6YS5sYSIsInR5cGUiOiJ0ZXh0In0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJhcHBsaWNhdGlvbi1pZCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6ImFwcGxpY2F0aW9uLXNlY3JldCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6ImVuZHBvaW50LXVybCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6InJlZnJlc2gtdG9rZW4iLCJ2YWx1ZSI6IiIsInR5cGUiOiJ0ZXh0In0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJ0ZXN0LXB1YmxpYy1ncm91cC1pZCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6InRlc3Qtc3ViLWdyb3VwLWlkIiwidmFsdWUiOiIiLCJ0eXBlIjoidGV4dCJ9LHsiZW5hYmxlZCI6dHJ1ZSwia2V5IjoibW9iaWxlLW51bWJlci0zIiwidmFsdWUiOiIrOTExMDk5OTk5OTkiLCJ0eXBlIjoidGV4dCJ9LHsiZW5hYmxlZCI6dHJ1ZSwia2V5IjoidGVzdC1hY3Rpb24taWQiLCJ2YWx1ZSI6IiIsInR5cGUiOiJ0ZXh0In0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJ0ZXN0LXN1cnZleS1pZCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifSx7ImVuYWJsZWQiOnRydWUsImtleSI6InRlc3Qtd2ViaG9vay1pZCIsInZhbHVlIjoiIiwidHlwZSI6InRleHQifV0=)

Set following environment variables in **Kaizala-APIs-environment** before running the postman project:
* mobile-number : Your mobile number which is used for invoking APIs
* application-id : ID associated with the Connector
* application-secret : Secret associated with the Connector

Other enviroment variables is auto-populated while trying the APIs in sequence mentioned in the Postman Project. 
