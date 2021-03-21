---
layout: page
title: About
permalink: /about/
---

**AskBob** is an easily customisable, completely federated voice assistant deployable on low-power devices with limited to no internet access that performs all speech and personal data processing offline on-device.

This is our development blog, where we'll be documenting our progress as we research, design, test and build **AskBob**.

# Team members

- Jeremy Lo Ying Ping ([jeremy.ping.19@ucl.ac.uk](mailto:jeremy.ping.19@ucl.ac.uk))
- Akhere Ihoeghinlan ([ak.ihoeghinlan.18@ucl.ac.uk](mailto:ak.ihoeghinlan.18@ucl.ac.uk))

# MoSCoW list
The following is a list of 'must have', 'should have', 'could have' and 'would have' requirements for *AskBob*:
## Must have
- **federated architecture** wherein the interpretation and processing of all speech and personal data must occur locally when **AskBob** is being operated in 'interactive mode', i.e. where users can speak to **AskBob** and hear responses to queries
    - Any personal data provided by the user (mostly related to keeping track of the conversation flow) must be stored and processed locally.
- **local operation on low-power devices** (e.g. laptops, desktops and Intel NUCs with i3 processors running locally) with little to no internet access such that it could be deployed in the community in places such as care homes, hospitals, GP clinics, etc
    - Where there is internet access, this may only be used for interfacing with external RESTful APIs containing no personally identifiable information to ensure compliancy with data protection law
- **a plugin system** allowing system administrators to install additional **AskBob** 'skills' as plugins
    - **AskBob** should primarily serve as a framework for other developers' plugins that tailor the voice assistant to their own specific use cases.
- **an accessible index of voice assistant skills** currently installed and available for use through the plugin system

## Should have
- **a configuration generator responsive web-app** that allows administrators to more easily generate plugin configuration files required for the creation of new **AskBob** skills plugins
- **the capability to interoperate with external web services via third-party plugins**
    - Third-party plugin developers should be able to write their own **AskBob** plugins adding voice assistant skills that interface with external APIs, such as the CarerCare platform and other external RESTful web APIs.
- **integration with the FISE video conferencing team** by providing support for voice queries within their FISE lounge web app via a RESTful web API (possibly over a private local area network)
- **integration with the FISE concierge team** -- who are building a RESTful web service that centralises and simplifies access to a range of different online web services -- by providing support for understanding textual queries via a RESTful web API within their Android app (possibly over a private local area network) that may retrieve data from their web service

## Could have
- **multilingual support**
- **a skills viewer web-app** to allow administrators to view the index of installed **AskBob** skills in a more visual manner
- **compatibility with other APIs over several protocols** via third-party plugins, e.g. Win32 on Windows, IFTTT in the home, any other in-home network with a centralised hub, Bluetooth, etc
- **access to open-source services** via the concierge team's web service (e.g. the ability to search for something, look up the weather, read something out loud, etc) when running locally (or perhaps in the FISE video conferencing group's 'lounge')
- **a drag-and-drop-style interface** to implement simple voice assistant skills in the configuration generator web app

## Would have
- **a plugins marketplace** whereby system administrators can download and install additional plugins (via a URL) in new **AskBob** builds
- **an advanced MIT Scratch-style draft-and-drop interface** to implement complex voice assistant skills in the configuration web app that would otherwise have to be implemented in Python code, e.g. RESTful API calls
- **support for wearable devices**, such as smart watches
