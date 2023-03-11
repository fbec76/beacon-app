# Beacon - Get home safe

Beacon is an app which provides a way on how to get home safe by tracking a users location and take actions if there are complications on the way without the user having to do anything.

## Idea

Beacon is an app helping people to get home safe. It is a location based app which tracks the location of the user and takes action in case of danger.
By analyzing the location of the user, the app can detect if the user is in danger. The user has to have a constant connection to the internet during the whole trip.
It would work as follows:

1. The user sets a destination like home, a friends house, work or any other place. (Up to 5 destinations can be saved, any other place can be used directly via a selection menu)

2. The user sets it travel mode (e.g. walking, cycling, driving, public transport, etc.) With the help of google maps, the app calculates suggested ways and the estimated time of arrival. The user then is able to select the way he wants to use (like in the google maps app).

3. From now on the app tracks and analyzes the users way. If the user suddenly stops (for longer than usual) or uses a direction which does not seem to be the right one, the app will notify the user ans asks if everything is okay. If the user does not answer, the app will send a notification to previously selected contacts (e.g. family, friends, etc.) with the current location of the user and its healthcare information (e.g. allergies, blood type, etc.). The app also is able to call the emergency services (e.g. 112/110) and send the current location of the user.

4. If the user gets home safe, he can stop the tracking and the app will ask the user to send notifications to it emergency contacts that he got home safe. This can be accepted or declined.

The goal of this whole process is to help people to get home safe and feel safe while traveling alone. The app also wants to have the user make as little as possible effort to detect if the user is in danger. Needing to type in any form of "hello im in danger please help me my current location is ..." or just clicking a button should not be the way to go. The app should be able to detect if the user is in danger and take action without the user having to do anything.

## Features

The app uses an approach in which its not a "neutral app" but to be personal. The users should not feel being tracked rather than being attended by a friend. This virtual friend (assistant) will be called **Lily**.

The app will be able to:

- Track the location of the user
- Detect if the user is in danger (possibly using AI)
- Notify emergency contacts (e.g. family, friends, etc.)
- Call emergency services (e.g. 112/110)

### Optional features

The user can simulate a phone call with **Lily**. Talking everything to make others look like the user is having a real conversation. This can be used to make the user feel more safe.

## Technology stack

The app will be available to mobile phones as a standalone build app. It will be developed using React Native and Expo for the frontend.
Amazon Web Services will be used for the backend. Using serverless functions could be a problem because of the need of a constant connection to the internet. Therefore, probably a normal server will be used. The use of serverless websocket could also be an option.
For managing the infrastructure as code, terraform will be used.

The following list of links will be useful to start the development:

- [React Native](https://reactnative.dev)
- [React Native with Typescript](https://reactnative.dev/docs/typescript)
- [Expo](https://expo.io)
- [Amazon Web Services](https://aws.amazon.com)
- [Google Maps API](https://developers.google.com/maps/documentation)
- [Amplify](https://aws.amazon.com/amplify)
- [Authentication](https://docs.amplify.aws/ui/auth/authenticator/q/framework/react-native/)
- [User Information Storage](https://aws.amazon.com/blogs/mobile/build-a-user-settings-store-with-aws-appsync/)
- [Object Storage](https://aws.amazon.com/s3/)
- [React Native Websocket](https://blog.logrocket.com/how-to-implement-websockets-in-react-native/)
- [AWS Websocket](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-websocket-api.html)
- [AWS Serverless Websocket](https://aws.amazon.com/blogs/compute/building-serverless-multi-region-websocket-apis/)
- [AWS Notifications](https://docs.aws.amazon.com/sns/latest/dg/sns-mobile-phone-number-as-subscriber.html)
- [AWS Cloud Development Kit](https://aws.amazon.com/cdk/)
- [AWS Command Line Interface](https://aws.amazon.com/cli/)
- [Terraform](https://www.terraform.io)

## Design

Calling the app beacon because the user should image a beacon which is sending out a signal to help the user to get home safe. Having a light beacon at night as a symbol for the app could be a good idea.

## Other

This project is part of a Bachelor Thesis for the FOM Fachhochschule für Oekonomie & Management in Münster, Germany.
