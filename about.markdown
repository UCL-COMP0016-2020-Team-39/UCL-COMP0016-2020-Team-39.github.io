---
layout: page
title: About
permalink: /about/
---

_AskBob_ is an easily customisable, completely federated and rapidly deployable voice assistant operable on low-power devices with limited to no internet access.

This is our development blog, where we'll be documenting our progress as we research, design, test and build _AskBob_.

# Team members

- Jeremy Lo Ying Ping ([jeremy.ping.19@ucl.ac.uk](mailto:jeremy.ping.19@ucl.ac.uk))
- Akhere Ihoeghinlan ([ak.ihoeghinlan.18@ucl.ac.uk](mailto:ak.ihoeghinlan.18@ucl.ac.uk))

# MoSCoW list
The following is a list of 'must have', 'should have', 'could have' and 'would have' requirements for *AskBob*:
## Must have
- **completely federated**: the interpretation and processing of all speech must occur locally
- **operable on low-power devices** (e.g. laptops, Intel NUCs with atom processors, tablets, browsers - anything anywhere!) with little to no internet access (where there is internet access, this may only be used for sending JSON requests to RESTful APIs containing no personally identifiable information to ensure GDPR compliancy)
- **rapidly deployable** in places such as care homes, hospitals, GP clinics, etc
- **local storage of all personal data**: a local database storing all personal data will be processed locally by the different services supported by our voice assistant
- **a flatfile index of all services and services** with which the voice assistant is interoperable (similar to Alexa skills) and which are easily enablable by system administrators

## Should have
- **configurability via a responsive web-app** interfacing with the aforementioned local database (or perhaps a web API) that allows administrators to examine the local database and add new ‘skills’ to the voice assistant, including multilingual capabilities
- **interoperability with the existing CarerCare platform and other services** : it should be relatively simple to interface with external APIs.

## Could have
- **multilingual support**
- **drag-and-drop-style interface** to implement new voice assistant skills
- **compatibility with many devices over several protocols**, e.g. IFTTT in the home, any other in-home network with a centralised hub, Bluetooth (like Philips hue lightbulbs), etc.
- **features based on open-source services**, e.g. the ability to search for something, look up the weather, purchase something, read something out loud, etc.

## Would have
- **full chatbot functionality** wherein users could maintain a long conversation with the voice assistant
