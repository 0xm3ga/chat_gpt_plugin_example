# ChatGPT Plugin Documentation

ChatGPT Plugins is an exciting new feature offerd by OpenAI that allows developers to integrate ChatGPT with third-party applications, opening the door to a world of possibilitie, empowering it to fetch real-time data, mine information from knowledge bases, assist in a wide range of tasks, and much more.

## Introduction

ChatGPT Plugins function by leveraging one or more API endpoints, defined within a **manifest file** and an **OpenAPI specification**. The AI model utilizes these specifications to function as an adept API caller, facilitating dynamic interactions with user queries. For example, a user question about a codebase could trigger the model to call an associated plugin API, fetching relevant code snippets. These snippets are then utilized by ChatGPT to contextually address the query.

## Developing a ChatGPT Plugin: A Step-by-Step Guide

Here's the process for creating a ChatGPT plugin:

1. **Craft a manifest file**: Host this file at `yourdomain.com/.well-known/ai-plugin.json`. This file needs to include metadata about your plugin, information on necessary authentication, and an OpenAPI specification for your desired endpoints.

2. **Register your plugin**: This is done via the ChatGPT UI. As part of the authentication process, you'll need to provide either an OAuth 2 `client_id` and `client_secret` or an API key.

3. **User engagement with your plugin**: Users will need to manually activate your plugin through the ChatGPT UI. Once OAuth is set up, users will be redirected to your plugin for signing in.

4. **Initiation of user conversation**: ChatGPT introduces a succinct description of your plugin into the conversation, which remains hidden from the end users. If a user poses a relevant question, the model may initiate an API call to your plugin. The results from this API call are then amalgamated into the model's response, providing a seamless user experience.
