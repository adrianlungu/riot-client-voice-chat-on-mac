# Riot Client with Voice (for League of Legends, TFT, etc)

**An app to run League of Legends on MacOS with Voice enabled.** 

### How to run

1. Download the app by downloading the repo, or downloading from the Releases page
2. (Optional) Move it into your `/Applications` folder
3. Run it
4. Enjoy

### About

The League of Legends client, as well as the Riot Client still have issues on MacOS with asking for permissions to use the microphone. This prevents the proper usage of the in-game League Chat with Voice. 

On M1 at least, the following hack does not seem to be working anymore, possibly due to changes in how League of Legends is started, or potentially due to Rosetta: 

```bash 
cd '/Applications/League of Legends.app/Contents/LoL/'

./LeagueClient.app/Contents/MacOS/LeagueClient
```

This app wraps the following script to be able to easily run it from the Applications folder easily:

```bash
cd "/Users/Shared/Riot Games/Riot Client.app/Contents/Frameworks/RiotClient.app/Contents/MacOS/"

./RiotClientUx
```

It seems that running the Riot Client instead of the League Client allows the League Client to be run properly and ask for microphone permissions from MacOS. 

### Tested On

- [x] MacOS Monterey 12.6 on M1 Pro 
