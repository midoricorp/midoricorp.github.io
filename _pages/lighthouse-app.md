---
layout: inner
title: Helping refugees in distress share their location.
permalink: /lighthouse-app/
lead_text:
featured_video_id:
featured_image: /img/lighthouse.png
---

## The Problem

The migrant crisis is a worldwide issue and is especially more pressing in the Greek coasts. Every day, there are hundreds of shipwrecked boats filled with refugees that wash up on the shore - dramatic scenarios. While discussing with reporters covering the story in Lesbos, I asked what could the tech community be doing? Their answer was that the camp organizers over there are overwhelmed:

> "There are so many boats that we can’t keep track of which ones need help. We would need a way to get alerts for passengers that are in distress."

They assured us that due to the small strip of sea separating Turkey and Lesbos migrants travelling have access to cellular network and often a smartphone along the journey and roam all the way through.

So came the idea for Lighthouse!


## The Solution

Lighthouse is a combination of a mobile app for migrants navigating and a cloud dashboard for the rescue teams on shore.

When a boat is in distress, anyone with the application downloaded on their phone can launch it a press an alert button that will send their coordinates to the closest shore station.

![lighthouse](/img/lighthouse.gif)

This station has access to a Lighthouse dashboard that monitors alerts in the filtered area. When rescue teams receive that alert, they can choose to acknowledge it - which will send a message to the migrant's mobile phone letting them know someone's coming (so they don't lose hope). With this real-time communication link the rescue teams can also send images and tips on first aid.

## How It's Built

*   The mobile app is developed with Ionic and AngularJS to provide a universal app for iOS, Android, Windows phone, and web access.

*   The dashboard is an AngularJS application that uses the Google Maps API to place the alerts on the map along with a filter zone (to avoid spamming)

*   All the alerts and rescue messages are sent and received using Firebase to provide a real-time communication system.

*   Built with lots of love

## What's Next

The Lighthouse alert system is in its primitive form. Here are some of the improvements we would like to make before implementation:

*   **Alert button:** The alert button will send audio recording of the situation to a remote server fro Natural Language Processing to pick up on key words and provide better contextual imformation back to the migrant's applicaiton (eg. first aid tutorials)

*   **Status & Acknowledgements:** The acknoweldgment button will be improved to allow the resuce teams to initiate a chat session with the person in distress along with sending pictures an material.

*   **Integration with Firechat:** [Firechat](http://opengarden.com/firechat/) is an applicaiton that allows people that don't have internet access to send out messages via hopping through earby hosts until the host has cellular network. This will allow Lighthouse to work even if the people in distress do not have access to the internet.

*   **Integrate SMS Functionality:** This will allow people without smartphones to send an alert anyway.

*   **Implementation & Testing:** We will be shipping out to Lesbos the summer of 2016 to implement the solution and test it thoroughly.

## Help out!

[The code is now hosted on Github](https://github.com/codersontheroad) and we welcome all contributions
