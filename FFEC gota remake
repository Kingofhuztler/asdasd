// ==UserScript==
// @name         FFEC's Script -
// @namespace    http://tampermonkey.net/
// @version      1.1.4
// @description  Let's improve your Gota experience!
// @author       FFEC
// @match        http://gota.io/web/*
// @grant        GM_addStyle
// @contributor  Verseh
// @icon         http://i.imgur.com/1K3g5EF.png
// @downloadURL  https://github.com/FFEC/FFEC-s-Script/raw/master/FFEC's%20Script.user.js
// ==/UserScript==

function addStyleSheet(style){
  var getHead = document.getElementsByTagName("HEAD")[0];
  var cssNode = window.document.createElement( 'style' );
  var elementStyle= getHead.appendChild(cssNode);
  elementStyle.innerHTML = style;
  return elementStyle;
}

//Custom Font, Logo, Viruses and Mothercells

GM_addStyle('* #logo {background-image: url("http://i.imgur.com/PIy1bq2.png");}');

GM_addStyle('* @font-face {font-family: "Ubuntu"; src: url("https://fonts.googleapis.com/css?family=Ubuntu");}');

addStyleSheet('@import url(https://fonts.googleapis.com/css?family=Ubuntu);');

GM_addStyle('* #chat-body td {font-family: "Ubuntu";}');

GM_addStyle('* #main-stats {font-family: Ubuntu;}');

GM_addStyle('* .main-bottom-stats {font-family: Ubuntu;}');

GM_addStyle('* .coordinates {font-family: Ubuntu;}');

GM_addStyle('* #leaderboard-panel {font-family: Ubuntu;}');

GM_addStyle('* #score-panel {font-family: Ubuntu;}');

GM_addStyle('* #main {font-family: Ubuntu;}');

GM_addStyle('* .gota-btn {font-family: Ubuntu;}');

GM_addStyle('* #popup-party {font-family: Ubuntu;}');

GM_addStyle('* #chat-input {font-family: Ubuntu;}');

//Border Removal
document.getElementById("leaderboard-panel").style.borderRadius = "0";
document.getElementById("leaderboard-panel").style.borderWidth = "0px"; 
document.getElementById("leaderboard-panel").style.boxShadow = "0px 0px 0px black";
document.getElementById("score-panel").style.borderRadius = "0";
document.getElementById("score-panel").style.borderWidth = "0px"; 
document.getElementById("score-panel").style.boxShadow = "0px 0px 0px black";
document.getElementById("minimap-panel").style.borderRadius = "0";
document.getElementById("minimap-panel").style.borderWidth = "0px"; 
document.getElementById("minimap-panel").style.boxShadow = "0px 0px 0px black";
document.getElementById("minimap-panel").style.marginBottom = "3px";
document.getElementById("party-panel").style.borderRadius = "0";
document.getElementById("party-panel").style.borderWidth = "0px"; 
document.getElementById("party-panel").style.boxShadow = "0px 0px 0px black";

//Custom Borders
GM_addStyle('* .main-panel {border: solid 3px rgba(99, 97, 95, 0.5)}');
GM_addStyle('* .main-panel {border-radius: 0px}');
GM_addStyle('* .main-panel {box-shadow: 0px 0px 0px 0px rgba(0,0,0,0.52)}');
GM_addStyle('* .gota-btn {border-radius: 15px}');
GM_addStyle('* .main-bottom-stats {border-radius: 5px}');
GM_addStyle('* #popup-party {border-radius: 0px}');
GM_addStyle('* #popup-party {box-shadow: 0px 0px 0px 0px rgba(0,0,0,0.25)}');

//Cell Color Mode
document.addEventListener('keydown', function(e) {
       var key = e.keyCode || e.which;
       switch (key) {
           case 113:
               if (player.rainbow === false) {
                   player.rainbow = true;
                   rainbowColors = ["#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600", "#FF6600"];
} else {
  player.rainbow = false;
}
       }
   });

//Social Media Button Removal
$(".main-bottom-links").replaceWith("");

//Double Split Macro
(function() {
    var amount = 2; // Number of splits
    var duration = 5; // Split delay in milliseconds

    var overwriting = function(evt) {
        if (evt.keyCode === 16) { // 16 is Shift
            for (var i = 0; i < amount; ++i) {
                setTimeout(function() { // 32 is Space
                    window.onkeydown({keyCode: 32}); 
                    window.onkeyup({keyCode: 32});
                }, i * duration);
            }
        }
    };

    window.addEventListener('keydown', overwriting);
})();
//Max Split Macro
(function() {
    var amount = 4; // Number of splits
    var duration = 5; // Split delay in milliseconds

    var overwriting = function(evt) {
        if (evt.keyCode === 17) { // 17 is Control
            for (var i = 0; i < amount; ++i) {
                setTimeout(function() { // 32 is Space
                    window.onkeydown({keyCode: 32}); 
                    window.onkeyup({keyCode: 32});
                }, i * duration);
            }
        }
    };

    window.addEventListener('keydown', overwriting);
})();
