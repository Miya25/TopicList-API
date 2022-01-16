Official TopicBotList API!
 ***
 **examples**
 ***
  
**const Discord = require("discord.js");
const client = new Discord.Client();
const TopicList= require("TopicBotList.js");
const dbl = new TopicList("TOKEN-HERE", client);
client.login("bot token here!");***
***
***Certificate Application Example***

***dbl.certificateApplication("Bla bla bla bla bla bla bla bla bla bla bla bla...", () => {
    console.log("Certificate successfully applied.");
})***
***
***Vote Checking***

***dbl.checkVote("userId").then((value) => {
    if(value === 1) {
        console.log("User voted.")
    } else {
        console.log("User not voted.")
    }
})***
***
***All Operations***
***const TopicBotList = require('TopicBotList.js');
const { Client } = require("discord.js");
const client = new Client();
const dbl = new TopicBotList("TopicBotList-Bot-Token-Here", client)
dbl.on("ready", () => {
    console.log('TopicBotList ready!')
})
dbl.checkVote("userId").then((value) => {
    if(value === 1) {
        console.log("User voted.")
    } else {
        console.log("User not voted.")
    }
})
dbl.certificateApplication("Bla bla bla bla bla bla bla bla bla bla bla bla...", () => {
    console.log("Certificate successfully applied.");
})
client.on("ready", () => {
    console.log("Logged as in "+client.user.tag)
})
client.login("Discord-Bot-Token")***