# pda-http-playground
HTTP Playground for Dataswyft PDA APIs

## Introduction
The repository is a TLDR Level 101 demostration of Dataswyft's PDA APIs.

## Prequisites
1. I assume you are a software developer.
2. You are familiar with a programming language and have a favourite application framework. Lastly, I assume you understand REST APIs, with their `GET`, `POST`, `PUT`, `DELETE` and so on.
3. You have a Live PDS
4. You have an account on our Developers Portal.
5. You have created a Project under your Developers Portal Account.

## Live PDA and Developers Portal
You can fulfill the above requirements 3-5 by registering at our [Developers Portal](https://developers.dataswift.io).
Upon registration, you will be given
1. A Live PDS - Please keep your credentials safe.
2. the rights to create your Project
Initially, all created Projects operate in our Sandbox environment.

## Technical Requirements
1. This Github Repo - [PDA HTTP Playground](https://github.com/dataswift/pda-http-playground)
2. Visual Studio Code
3. Rest Client extension by Huachao Mao. [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=humao.rest-client). All the instructions with the .http files in this repo are executable.

## Repo Contents
This repo contains
1. README.md
2. test/rest-client/pda.http
    * the main purpose of this file is to demonstrate the creating, reading, updating and deleting of records on the PDA
3. test/rest-client/hatters.http
    * the main purpose of this file is to show how to create a PDA for your application
    * authenticate a user against his PDA
    * and to make queries about a user

## Basic Concepts
2. When you register your PDA application in the Developers Portal, you will be given an `application_id`. You'd need the application_id when authenticating the user.
3. After a successful authentication, you will receive an `application_token` with which to call the REST APIs with.
4. Every application has a `namespace` where data is stored. The `application_token` will give you access to the `namespace`

## Where to find further help
1. Join our HAT Community on Slack. Especially #developers channel
    * After you have registered on the Developers Portal, our HATLab Studio manager will send you the invitation link to the Slack workspace in a welcome email.
2. In your Developers Portal dashboard, go to `Docs`
    * it will point you to various places on [Dataswyft Docs](https://docs.dataswyft.com)
3. The full blown API set that is compatible with Postman is available on (https://api.dataswift.io/)
