# weather-bot
Simple telegram weather bot with **NodeJS**. Bot can give current weather for a given location and manage subscriptions for users to be alerted everyday with weather prediction.

## Requirements ##
- Create a bot and get your bot token. More info in [Telegram web.](https://core.telegram.org/bots) 
- Register for free and get your token in [OpenWeatherMap.](https://openweathermap.org/api)
- Tested on node 7.10.0.

## Installation ##
Edit the following info in `config.js`.  

- Place your telegram bot token in `TELEGRAM_BOT_TOKEN`.  
- Put your openweather token in `OPENWEATHER_TOKEN`.  
- Set the absolut path for sqlite database file in `SQLITE_DB_PATH`.
- Install sqlite3 (if it is not present) on your OS.

Download dependencies and run in NodeJS:  

    npm install   
    node index.js    


> 
> 
> **How can I message all of my bot's subscribers at once?**
> 
> Unfortunately, at this moment we don't have methods for sending bulk messages, e.g. notifications. We may add something along these lines in the future.
> 
> In order to avoid hitting our limits when sending out mass notifications, consider spreading them over longer intervals, e.g. 8-12 hours. The API will not allow more than ~30 messages to different users per second, if you go over that, you'll start getting 429 errors.

From [OpenWeatherMap web](https://openweathermap.org/price), free plan allows **60 calls per minute**.

