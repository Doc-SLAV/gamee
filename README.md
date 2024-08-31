# Gamee

Auto Claim Wat Point from gamee



# Table of Contents

- [Gamee](#gamee)
- [Table of Contents](#table-of-contents)
- [Feature](#feature)
- [Register ?](#register-)
- [How to Use](#how-to-use)
  - [Bot.py Parameter](#botpy-parameter)
  - [Windows](#windows)
  - [Linux](#linux)
  - [Termux](#termux)
- [How to Get Data](#how-to-get-data)
- [Javascript Command to Get Telegram Data for Desktop](#javascript-command-to-get-telegram-data-for-desktop)
- [Run for 24/7](#run-for-247)

```text
Sorry, I can't add the feature to complete the 'race' because my device doesn't support it. 
When I press the play button, it only shows a black blank, then I asked someone and he replied “maybe your internet is problematic”. Then I waited until this morning and I tried again but still couldn't.
Then I tried to see the console menu and it turned out that there was an error that my device did not support playing the game.
So I only updated for mining action, maybe I will update for “racing” action later when I buy rdp (Remote Desktop Protocol / Windows Server) or buy a new device.
That's all, thank you.
```

# Feature

- [x] Auto Claim
- [x] Auto Daily Spin
- [x] Spin Using Ticket
- [x] Support Multi Account
- [x] Claim Previous Session Mining Rewards

# Register ?

Ask u friend for invitation code !

# How to Use

## Bot.py Parameter

Here are some parameters that can be used in bot.py or the bot's main script

| parameter       | desctiption                                                                         |
| --------------- | ----------------------------------------------------------------------------------- |
| --data          | serves to set custom input data (default: data.txt)                                 |
| --config        | serves to set a custom config file (default: config.json)                           |
| --marinkitagawa | serves to run the bot script without deleting the terminal / console display first. |

## Windows 

1. Make sure you computer was installed python and git.
   
   python site : [https://python.org](https://python.org)
   
   git site : [https://git-scm.com/](https://git-scm.com/)

2. Clone this repository
   ```shell
   git clone https://github.com/Doc-SLAV/gamee.git
   ```

3. goto gameetod directory
   ```
   cd gamee
   ```

4. install the require library
   ```
   python -m pip install -r requirements.txt
   ```

5. fill the `data.txt` file with your data, how to get data you can refer to [How to Get Data](#how-to-get-data)
6. execute the main program 
   ```
   python bot.py
   ```

## Linux

1. Make sure you computer was installed python and git.
   
   python
   ```shell
   sudo apt install python3 python3-pip
   ```
   git
   ```shell
   sudo apt install git
   ```

2. Clone this repository
   
   ```shell
   git clone https://github.com/Doc-SLAV/gamee.git
   ```

3. goto gamee directory

   ```shell
   cd gamee
   ```

4. Install the require library
   
   ```
   python3 -m pip install -r requirements.txt
   ```

5. fill the `data.txt` file with your data, how to get data you can refer to [How to Get Data](#how-to-get-data)
6. execute the main program 
   ```
   python bot.py
   ```

## Termux

1. Make sure you termux was installed python and git.
   
   python
   ```
   pkg install python
   ```

   git
   ```
   pkg install git
   ```

2. Clone this repository
   ```shell
   git clone https://github.com/Doc-SLAV/gamee.git
   ```

3. goto gamee directory
   ```
   cd gamee
   ```

4. install the require library
   ```
   python -m pip install -r requirements.txt
   ```

5. fill the `data.txt` file with your data, how to get data you can refer to [How to Get Data](#how-to-get-data)
6. execute the main program 
   ```
   python bot.py
   ```

# How to Get Data
   
   1. Active web inspecting in telegram app, How to activate just search on google
   2. Goto gamee bot and open the apps
   3. Press `F12` on your keyboard to open devtool or right click on app and select `Inspect`
   4. Goto `console` menu and copy [javascript code](#javascript-command-to-get-telegram-data-for-desktop) then paste on `console` menu
   5. If you don't receive error message, it means you successfully copy telegram data then paste on `data.txt` (1 line for 1 telegram data)
   
   Example telegram data

   ```
   query_id=xxxxxxxxxx&user=xxxxxxfirst_namexxxxxlast_namexxxxxxxusernamexxxxxxxlanguage_codexxxxxxxallows_write_to_pmxxxxxxx&auth_date=xxxxxx&hash=xxxxxxxxxxxxxxxxxxxxx
   ```

   6. If you want to add more account. Just paste telegram second account data in line number 2.
   
   Maybe like this sample in below

   ```
   1.query_id=xxxxxxxxxx&user=xxxxxxfirst_namexxxxxlast_namexxxxxxxusernamexxxxxxxlanguage_codexxxxxxxallows_write_to_pmxxxxxxx&auth_date=xxxxxx&hash=xxxxxxxxxxxxxxxxxxxxx
   2.query_id=xxxxxxxxxx&user=xxxxxxfirst_namexxxxxlast_namexxxxxxxusernamexxxxxxxlanguage_codexxxxxxxallows_write_to_pmxxxxxxx&auth_date=xxxxxx&hash=xxxxxxxxxxxxxxxxxxxxx
   ```

# Javascript Command to Get Telegram Data for Desktop

```javascript
copy(Telegram.WebApp.initData)
```

# Run for 24/7 

You can run the script bot for 24/7 using vps / rdp. You can use `screen` application in vps linux to running the script bot in background process
