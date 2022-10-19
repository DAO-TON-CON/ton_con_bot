# TON CON BOT
[@ton_con_bot](https://t.me/ton_con_bot)

![Downloads](https://img.shields.io/github/downloads/DAO-TON-CON/ton_con_bot/total) ![Contributors](https://img.shields.io/github/contributors/DAO-TON-CON/ton_con_bot?color=dark-green) ![Issues](https://img.shields.io/github/issues/DAO-TON-CON/ton_con_bot) ![License](https://img.shields.io/github/license/DAO-TON-CON/ton_con_bot) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

This project contains everything you need to launch your own Telegram bot quickly.

This bot is designed for communication with interested audience, CON presale, buying cryptocurrency TON and also has referral program.

## Built With

This project is developed in procedural PHP version 7+ without the use of libraries, which allows you to run it on any hosting that supports PHP and MySQL. This approach also makes it easy and accessible to edit the bot's code. 

## Getting Started

This is an example of how you may setting up your project locally.
To get a local copy up and running follow these simple steps described below.

### Prerequisites

This project requires any hosting that supports PHP 7 and MySQL. 

### Installation

Main bot executable script: `tgbot.php`

1) Fill in the user data in the `config.php` file, namely:

############################<br/>
$admin = 00000; // ChatID of a manager, owner <br/> 
$verifyrecipient = "XXXX"; // TON wallet for getting vefification transactions  <br/>
$reference = 5; // Is not in use  <br/>
$depopercent = 5; // A referral percent for deposits  <br/>
$NFTRefPercent = 10; // Referral percent  <br/>
$wallet2donate = "XXXXX"; // TON wallet for donations  <br/>
$verifRefFee = 0.05; // Commission to referral from verification payment  <br/>
$api_key = 'XXX'; // TON CON API Key  <br/>
$roskassa_publickey = 'XXXX'; // TON CON Public Key  <br/>
$roskassa_secretkey = 'XXXX'; // TON CON Secret Key  <br/>
$tonconrate = 0.1; // CON and CryptoBot commission  <br/>
$NFTwalletTON = "XXXXX"; // TON Wallet for incoming payments <br/> 
$nftCatRate = 45; // Is not in use  <br/>
$nftDogRate = 65;// Is not in use  <br/>
$toncenterAPIKey = "XXXXX"; // API Key of Toncenter website  <br/>
$CryptoPayAPIToken = ""; // CryptoPay API Token  <br/>
define('TOKEN', 'XXXXX'); // Add the Bot API Token  <br/>
############################<br/><br/>

2) Register the bot in Cryptopay by specifying the postback URL: [https://yourdomain/BotFolder/postback_cryptopay.php](https://yourdomain/BotFolder/postback_cryptopay.php)

3) Set the postback URL in the Tegro Money account: [https://yourdomain/BotFolder/postback.php](https://yourdomain/BotFolder/postback.php)

4) Fill in the MySQL database data in the `global.php` file

5) Import MYSQL database structure from `database.sql` file

6) Install the webhook at https://api.telegram.org/ for the `tgbot.php` script:
[https://api.telegram.org/botXXXXX/setWebhook?url=https://yourdomain/BotFolder/tgbot.php](https://api.telegram.org/botXXXXX/setWebhook?url=https://yourdomain/BotFolder/tgbot.php)

7) Bot texts can be edited in the `langs.php` file

8) Place the script [https://yourdomain/BotFolder/tonratechecker.php](https://yourdomain/BotFolder/tonratechecker.php) on cron with execution once a day

## Usage

Find the bot in the Telegram environment by its username: `@YourBot` and start it with the command `/start`

## Roadmap

See the [open issues](https://github.com/DAO-TON-CON/ton_con_bot/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/DAO-TON-CON/ton_con_bot/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
* Please make sure you check your spelling and grammar.
* Create individual PR for each suggestion.
* Please also read through the [Code Of Conduct](https://github.com/DAO-TON-CON/ton_con_bot/blob/main/CODE_OF_CONDUCT.md) before posting your first idea as well.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

https://github.com/DAO-TON-CON/ton_con_bot/commit/c208edcb519704cc98b2d9835d5ab9fef17b4d4e

## Authors

* **Lana Cool** - *Developer* - [Lana Cool](https://github.com/lana4cool/) - *Telegram bots on PHP*

## Acknowledgements

* [Lana](https://github.com/lana4cool/)
