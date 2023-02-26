# firebase-hardhat-sandbox

This repo is for a starter project using Firebase and Hardhat

## Installation

1. Install hardhat and firebase
```
npm install --save-dev hardhat
npm install --save-dev firebase
```

2. Create the sample project.
```
npx hardhat
```

Use the JavaScript option.

3. Initialize firebase
```
firebase init
```

In the first menu, at minimum you'll want to select:
- `Hosting: Configure files for Firebase Hosting...`
- `Emulators: Set up local emulators for Firebase products`

In the project setup menu, either create a new project or use an existing one.

In the emulators menu, at minimum you'll want to select:
- `Hosting Emulator`

Other options can be safely left as defaults. If you need to update anything later, re-run `firebase init`.

## Running locally

You'll need a few separate shells.

1. In shell 1, run a local node on all network interfaces.
```
npm run hh:node
```

2. In shell 2, run firebase
```
npm run fb:start
```

Verify that you can connect to the local firebase server in your browser at
[http://localhost:5000](http://localhost:5000).

3. In shell 3, deploy to the hardhad project to the local node
```
npm run hh:deploy
```

## Next steps

- Check the [Hardhat getting started guide](https://hardhat.org/hardhat-runner/docs/getting-started#quick-start)
- Check the [Firebase getting started guide](https://cloud.google.com/firestore/docs/client/get-firebase)

