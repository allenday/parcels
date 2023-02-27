# parcels

This repo is for a starter project using Firebase and Hardhat

## Installation

1. Install hardhat and firebase
```
npm install --save-dev hardhat
npm install --save-dev firebase
```

2. Create the sample project. The sample overwrites this file, so we work around.
```
mv README.md README.md.bak
npx hardhat
cat README.md >> README.md.bak
mv README.md.bak README.md
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

4. Install Hardhat dependencies

```
npm install --save-dev @openzeppelin/hardhat-upgrades
npm install --save-dev @openzeppelin/contracts
npm install --save-dev @nomiclabs/hardhat-ethers ethers
```

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

## Notes

- https://css-tricks.com/things-ive-learned-css-grid-layout/
- https://github.com/aarohmankad/identicon-api
- https://github.com/gnidan/interval-trees-solidity
- https://support.google.com/admanager/answer/2884033
- https://support.google.com/admanager/answer/1628457
- https://www.decentraboard.com/
- https://fravoll.github.io/solidity-patterns/randomness.html
- https://cssgrid-generator.netlify.app/

# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```
