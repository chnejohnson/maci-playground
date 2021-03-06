# MACI playground


## Guilds

Install dependencies
```
yarn install
```

### Roles

```ts
const [deployer, coordinator, alice, anyone] = await ethers.getSigners();
```

### Initiate

Start hardhat network at http://127.0.0.1:8545/

```sh
yarn start
```

Compile contracts

```sh
yarn compile
```

Deploy MACI, Ballot, and others.

```sh
yarn hardhat:local scripts/deployMaci.ts
```

Get maci info

```sh
yarn hardhat:local scripts/callMaci.ts 
```

### Vote

Sign up
```sh
yarn hardhat:local scripts/signUp.ts
```

Publish Message
```sh
yarn hardhat:local scripts/vote.ts
```

Publish Messages
```sh
yarn hardhat:local scripts/submitMessageBatch.ts
```

Change Key
```sh
yarn hardhat:local scripts/changeVote.ts
```


### Tally

```sh
yarn hardhat:local scripts/tallyWithoutProofs.ts
```

```sh
yarn hardhat:local scripts/tally.ts
```


### Verify