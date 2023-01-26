# Intro to BYOF

We are incredibly excited to announce the launch of first-of-a-kind feature on Polygon --> Build Your Own Farms (BYOF).&#x20;

### What is BYOF?

Build-your-own-farms (BYOF) allows users to create and deploy farms themselves. It can be thought of as a no-code farming-as-a-service.

#### Benefits

* Easy for partners to create farms.
* A great platform for teams to promote their project by giving out rewards in the project’s native tokens.
* No need to wait for a specific date to launch farms.
* No need to deploy farms manually, farms will automatically be deployed from the time specified by the creator.
* Free up our tech team’s bandwidth so they can focus on other development angles.

### How does the BYOF functionality work?

#### Cloning mechanism

The factory contract will clone the dummy contract and create a new farm contract with the parameters provided by the farm deployer. We have dummy contracts for Launch, Popular, Dual/Ecosystem farms. Other strategies can also be added, we will just need to add a dummy contract for that strategy to the factory contract
