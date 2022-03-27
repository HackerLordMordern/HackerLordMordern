// ==UserScript==
// @name         INFINITE PROJECT MORDERN EDITION
// @namespace    Hacker Lord Mordern
// @version        2
// @description  This is a script that modifies MooMoo.io!
// @author       MORDERN
// @author       Mythical Cookie and W4IT
// @match        *://moomoo.io/*
// @match        *://dev.moomoo.io/*
// @match        *://sandbox.moomoo.io/*
// @match        *://*.moomoo.io/*
// @require      https://cdnjs.cloudflare.com/ajax/libs/socket.io/1.4.5/socket.io.min.js
// @require      https://code.jquery.com/jquery-3.3.1.slim.min.js
// @require      http://code.jquery.com/jquery-3.3.1.min.js
// @require      https://cdn.jsdelivr.net/npm/fontfaceobserver@2.1.0/fontfaceobserver.standalone.min.js
// @require      https://cdn.jsdelivr.net/npm/msgpack-lite@0.1.26/dist/msgpack.min.js
// @license GNU PUBLIC LISCENCE Version 3, 29 June 2007
// ==/UserScript==
setInterval(() => window.follmoo && follmoo(), 10);//Starter resources
var spikeType;
alert("MORDERN IS UNDEFEATED");
document.getElementById('gameName').innerHTML = 'INFINITE MORDERN';
document.getElementById('loadingText').innerHTML = 'SUBSCRIBE TO HACKER LORD MORDERN'
document.getElementById('diedText').innerHTML = "HOW DARE YOU DIE? DONT ABUSE MORDERN BY DYING";
document.getElementById('diedText').style.color = "#ff0000";
document.title = 'INFINITE PROJECT MORDERN EDITION';
document.getElementById("leaderboard").append ('MOOMOO.IO MORDERN EDITION');
document.querySelector("#pre-content-container").remove();
document.getElementById("storeHolder").style = "height: 500px; width: 300px;";
function Hat (id){
    storeBuy(id);
    storeEquip(id);
}
document.addEventListener('keydown', function(e) {
    if (e.keyCode == 27 && document.activeElement.id.toLowerCase() !== 'chatbox') { // ESC for Unequip
        Hat(0);
    }
    if (e.keyCode == 66 && document.activeElement.id.toLowerCase() !== 'chatbox') { // B for Soldier
        Hat(6);
    }
    if (e.keyCode == 71 && document.activeElement.id.toLowerCase() !== 'chatbox') { // G for Turret gear
        Hat(53);
    }
    if (e.keyCode == 16 && document.activeElement.id.toLowerCase() !== 'chatbox') { // SHIFT for booster hat
        Hat(12);
    }
    if (e.keyCode == 188 && document.activeElement.id.toLowerCase() !== 'chatbox') { // "," for snow hat
        Hat(15);
    }
    if (e.keyCode == 60 && document.activeElement.id.toLowerCase() !== 'chatbox') { // < for flipper hat
        Hat(31);
    }
    if (e.keyCode == 90 && document.activeElement.id.toLowerCase() !== 'chatbox') { // Z for tank gear
        Hat(40);
    }
    if (e.keyCode == 74 && document.activeElement.id.toLowerCase() !== 'chatbox') { // J for emp helmet
        Hat(22);
    }
    if (e.keyCode == 84 && document.activeElement.id.toLowerCase() !== 'chatbox') { // T for samurai
        Hat(20);
    }
    if (e.keyCode == 89 && document.activeElement.id.toLowerCase() !== 'chatbox') { // Y for Bull Helmet
        Hat(7);
    }
});
 setTimeout( () => {
                newSend(["6", [4]]);//katana
            }, 35);
            setTimeout( () => {
                newSend(["6", [15]]);//musket
                autosecondary = true;
                newSend(["5", [secondary, true]]);
                newSend(["13c", [1, 53, 0]]);
                newSend(["13c", [0, 53, 0]]);
            }, 50);
if(a.keyCode == 46 && document.activeElement.id.toLowerCase() !== 'chatbox') {
        newSend(["6", [4]]);
        newSend(["15", [15]]);
}
if (a.keyCode == 76 && document.activeElement.id.toLowerCase() !== 'chatbox') {//reverse insta
        autoprimary = false;
        autosecondary = true;
        autoaim = true;
        doinsta = true;
        newSend(["13c", [0, 0, 1]]);
        newSend(["5", [secondary, true]]);
        newSend(["7", [1]]);
        newSend(["13c", [1, 53, 0]]);
        newSend(["13c", [0, 53, 0]]);
        newSend(["13c", [1, 21, 1]]);
        newSend(["13c", [0, 21, 1]]);
        setTimeout( () => {
            autoprimary = true;
            autosecondary = false;
            newSend(["13c", [1, 7, 0]]);
            newSend(["13c", [0, 7, 0]]);
            newSend(["13c", [0, 21, 1]]);
            newSend(["5", [primary, true]]);
        }, 40);
}
 if (a.keyCode == 32 && document.activeElement.id.toLowerCase() !== 'chatbox') {
     newSend(["ch", ['Console Insta! Log!']]);
        Hat(7);
        acc(21);
        setTimeout( () => {
            place(spikeType, myPlayer.dir + toRad(45));
            place(spikeType, myPlayer.dir - toRad(45));
        }, 40);
        setTimeout( () => {
            Hat(53);
        }, 50);
 }
const CanvasAPI = document.getElementById("gameCanvas")
CanvasAPI.addEventListener("mousedown", buttonPressD, false);
function buttonPressD(e) {
    if (document.getElementById("click").checked) {
        if (e.button == 2) {
            if(secondary == 10){
                newSend(["5", [secondary, true]]);
            }
            hat(40);
            acc(21);
            newSend(["7", [1]]);
            setTimeout( () => {
                if(secondary == 10){
                    newSend(["5", [primary, true]]);
                }
                acc(11);
                if (myPlayer.y < 2400) {
                    hat(15);
                } else {
                    if (myPlayer.y > 6850 && myPlayer.y < 7550) {
                        hat(31);
                    } else {
                        hat(12);
                    }
                }
                newSend(["7", [1]]);
            }, 100);
        }
    }
}
