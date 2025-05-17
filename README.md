# binary-bot
call put trading bot strategy

Bots with Strategy :
Candle Stick Strategy
Digit Strategy
Direction Strategy
Loss Martingale Reverse Recovery Strategy 
MACD Strategy
MACD Array Strategy
Median Digit Strategy
Multiple Martingale Strategy
RSI Strategy
RSI Array Strategy
SMA Strategy
Ticks List Strategy
---- So we are not responsible----
621acb7382a80bc1959c329ecda6537ccc023052
adding websocket to the Binary bot development..

const WebSocket = require('ws');
const DerivAPI = require('@deriv/deriv-api/dist/DerivAPI');

// app_id 1089 is for testing, create your own app_id and use it here.
// go to api.deriv.com to register your own app.
const connection = new WebSocket('wss://ws.derivws.com/websockets/v3?app_id=1089');
const api        = new DerivAPI({ connection });
const basic = api.basic;

basic.ping().then(console.log)