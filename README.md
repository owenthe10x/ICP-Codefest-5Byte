# DigiSignID

An IC-blockchain-based Digital Signature Web Application

![Homepage](./doc/homepage.png?raw=true "Title")


## Description

This website has 2 main features:
1. Digital Signature - The user can digitally 'sign' a document via the website. Derived features:
* Single Signature - performs a digital signature on a single document
* Batch Signature - perform digital signatures on several documents at once (directly on several documents at once, so later the user can upload many documents of the same size, then select one part of the document to sign → feature automatically signs all documents)
2. Digital Validation - The user can validate certain digital documents. The user will upload a document to the website, then the document publisher and the validity of the document will appear (has it been changed or not).

## Made by 5Byte Team
1. Atqiya Haydar Luqman
2. David Dewanto
3. Imanuel Sebastian Girsang
4. Owen Tobias Sinurat
5. Syakira Fildza


## Getting Started

### Dependencies

- NodeJS 18.\* or higher https://nodejs.org/en/download/
- DFX 15 or higher
- Internet Computer dfx CLI https://internetcomputer.org/docs/current/developer-docs/setup/install/
- Visual Studio Code (Recommended Code Editor) https://code.visualstudio.com/Download
- Crypto Module
  
```bash
sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"
```

### Installing

```Clone this Git repository on your local device:
[code blocks for commands](git clone https://github.com/owenthe10x/ICP-Codefest-5Byte/)
 ```
### Executing program

1. Open command terminal: Enter the commands to start dfx local server in background:

```
cd digisign-app
 ```
Note: If you run it in MacOS, you may be asked to allow connections from dfx local server.


2. Enter the commands to install dependencies, deploy canister and run Next.js dev server:
   
```
npm install
npm run dev
 ```

3. The website will usually run on:
   http://localhost:3000/

4. Deploying the canister
```
cd src
cd azle
npm install
dfx start --background --clean
dfx deps pull
dfx deps deploy
dfx deploy
 ```
5. Cleanup - stop dfx server running in background:

```
dfx stop
```
## Notes
You will need to set up a .env file in the project directory according to the port where your deployed canister are
it would look something like this :
```
NEXT_PUBLIC_CANISTER_ID_AZLE="bkyz2-fmaaa-aaaaa-qaaaq-cai"
NEXT_PUBLIC_IC_HOST=http://localhost:4943
## Help
```
Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

1. [@ImanuelSG](Imanuel Sebastian Girsang)
2. [@DomPizzie](Owen Tobias S)

## Version History

* 0.1
    * Initial Release

## License

This project is licensed under the 5Byte License - see the LICENSE.md file for details
