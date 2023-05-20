# Beacon - Get Home Safe

Beacon is an innovative mobile application that focuses on ensuring your safety as you travel. This location-based tool combines real-time tracking with intuitive risk detection to provide you with a secure route from your current location to your desired destination.

Designed with a proactive approach, Beacon analyzes your path, detecting any deviations or long stops that might imply potential danger. Its intelligent algorithms operate behind the scenes, eliminating the need for constant user engagement and allowing you to concentrate on your journey.

To effectively respond to risks, Beacon maintains an active internet connection, allowing for seamless location updates and emergency alert dispatches when required. Your privacy is paramount, and Beacon restricts tracking only to the duration of your travel and adheres to stringent data privacy standards.

Beacon's core functionality extends beyond risk detection. It provides a platform where you can save frequent destinations, choose your mode of transport, and get route suggestions based on real-time traffic data. This practical, user-oriented approach places Beacon as an invaluable tool in ensuring your safe travels.

## Concept
Beacon is not just an app; it's a personal security assistant that constantly monitors your location to keep you safe. The primary aim of Beacon is to make users feel secure while traveling alone by minimizing their interaction with the app, enabling them to focus on their journey.

To make your trip safer, the Beacon app tracks your travel route, predicts possible hazards, and alerts your preselected contacts if any potential danger arises. The user maintains an active internet connection throughout the journey, and the process unfolds as follows:

1. **Setting a destination**: Users can store up to five frequent destinations such as home, a friend's house, workplace, etc. An alternate location can also be selected directly from a map view.

2. **Selecting travel mode**: Users can specify their mode of travel (e.g., walking, cycling, driving, public transport, etc.). Leveraging the Google Maps API, Beacon calculates the optimal routes and estimates the time of arrival, allowing users to select their preferred path.

3. **Monitoring and analyzing**: Beacon continuously tracks and scrutinizes the user's route. If the user takes an unusual halt or detours unexpectedly, Beacon prompts the user for a response. Failing to respond triggers Beacon to alert the pre-selected emergency contacts with the user's real-time location and health information. It also has the capability to contact emergency services (112/110) with the user's precise location details.

4. **Arrival confirmation**: Upon safely reaching their destination, users can disable the tracking feature. Beacon then asks if the users wish to notify their emergency contacts about their safe arrival, which can be either accepted or declined.

## Core Features

To ensure the personal touch, Beacon introduces 'Lily,' an AI-driven assistant offering you a secure feeling of companionship rather than being surveilled. The primary features of Beacon include:

1. **Location Tracking**: Beacon tracks user location in the background, even if the phone screen is locked. Location tracking is active only during a trip.

2. **Danger Detection**: Using AI, Beacon analyzes the user's path and determines if the user might be in danger, such as taking an unexpected route or not moving for a prolonged duration. A manual 'emergency case' flag is also available for users to indicate immediate danger.

3. **Emergency Alerting**: Beacon can alert emergency contacts, including sharing live location and health information in a dangerous situation. It can also notify other Beacon users nearby and local emergency services.

4. **Arrival Status**: Once users reach their destination safely, they can mark their trip as 'Arrived Safe.' They can also optionally send a safety confirmation message to their emergency contacts.

5. **User Information Management**: Users can save up to five locations and emergency contacts. Personal information management, including surname, email, phone number, and password, is also possible.

6. **Safety Guidelines**: Beacon offers a collection of safety tips and self-defence strategies to help users avoid dangerous situations.

## Optional Features
1. **Simulated Phone Call with Lily**: To enhance the feeling of safety, users can simulate a phone call with Lily. This simulated conversation can deter potential threats, making the user feel more secure.

## Technology Stack
Beacon is a standalone mobile application developed with React Native and Expo for the frontend, while Amazon Web Services (AWS) powers the backend. A traditional server setup is being considered due to the requirement of a constant internet connection. However, the use of serverless websockets remains an option. Infrastructure management is implemented using Terraform.

To initiate development, the following resources could be helpful:

- [React Native](https://reactnative.dev/)
- [React Native with TypeScript](https://reactnative.dev/docs/typescript)
- [Expo](https://expo.io/)
- [Amazon Web Services (AWS)](https://aws.amazon.com/)
- [Google Maps API](https://developers.google.com/maps)
- [Amplify](https://aws.amazon.com/amplify/)
- [Authentication](https://docs.aws.amazon.com/amplify/latest/userguide/authentication.html)
- [User Information Storage](https://aws.amazon.com/dynamodb/)
- [Object Storage](https://aws.amazon.com/s3/)
- [React Native Websocket](https://www.npmjs.com/package/react-native-websocket)
- [AWS Websocket](https://aws.amazon.com/api-gateway/)
- [AWS Serverless Websocket](https://www.serverless.com/aws-lambda/)
- [AWS Notifications](https://aws.amazon.com/sns/)
- [AWS Cloud Development Kit](https://aws.amazon.com/cdk/)
- [AWS Command Line Interface](https://aws.amazon.com/cli/)
- [Terraform](https://www.terraform.io/)

## Design
The Beacon app gets its name from the idea of a light beacon that guides users safely home. A potential logo could symbolize a glowing beacon that illuminates a path in the dark.

## Project Origin
This project is part of a Bachelor Thesis for the FOM Fachhochschule für Oekonomie & Management in Münster, Germany.

Beacon is intended to provide a sense of security and peace of mind for people traveling alone, ensuring that help is readily available when they need it. It operates as a digital companion that accompanies users on their journeys, ready to act in the face of potential danger. With Beacon, you are never alone, and help is just a click away.
