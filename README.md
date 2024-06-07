## Overview

The purpose of this project is to create a backend service that collects data from an MQ-2 smoke sensor. The service uses a REST API to call the ThingSpeak API at a fixed rate of every 40 seconds to fetch the latest sensor values and update them accordingly.

## Features

- Fetches smoke sensor data from ThingSpeak API.
- Updates data every 40 seconds.
- Built with Spring Boot for easy deployment and management.

## Prerequisites

Before you begin, ensure you have met the following requirements:
- Java Development Kit (JDK) 17 or higher
- Maven
- Access to the ThingSpeak API and your channel's Read API Key

## Configuration

1. Open the `src/main/resources/application.properties` file.

2. Add your ThingSpeak API configuration:
    
    thingspeak.api.url=https://api.thingspeak.com/channels/{channel_id}/fields/{field_id}.json
    thingspeak.api.key=YOUR_READ_API_KEY

- For any queries contact [animity0407@gmail.com]
