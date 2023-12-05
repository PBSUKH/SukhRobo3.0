<h1 align="center">
  <b> Gojo_Satoru </b>
<!---</h1>
<h1 align="center"><img src="https://media.giphy.com/media/GL42TduR8AkNq1xRog/giphy.gif" /></h1>--->

<!---<h1 align="center"><img src="https://te.legra.ph/file/4bf3b88115068d41efadd.jpg" /></h1>--->
  
<h1 align="center"><img src="./extras/gojo_satoru__psd__by_at_yomiko_deyaec4-pre.jpg" /></h1>





# DEPLOYMENT 🚀
## Deploy To Heroku
* **Make Sure you have Heroku account**

* If you don't have heroku account what are you waiting for click [here](https://id.heroku.com/login) to make one or just deploy on other platform gudie is given below

* Just click on the button it will redirect you to Heroku website and deploy your bot there....enjoy 😉

[![DEPLOY](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/badmunda98/BADMANEGMENT)



## Variables
<details><summary><h3>List of all mandatory variables</h3></summary>
  
`BOT_TOKEN` You can get your bot token at [@BotFather](https://t.me/BotFather)

`API_ID` You can get your api id [here](my.telegram.org)

`API_HASH` You can get your api hash [here](my.telegram.org)

`DB_URI` Your [MongoDB](https://www.mongodb.com/) connection string.

`MESSAGE_DUMP`: Event logs channel where the bot will send updates. Note that it should start with `-100`.
</details>


<details><summary><h3>List of all variables</h3></summary>

`BOT_TOKEN` You can get your bot token at [@BotFather](https://telegram.dog/BotFather)

`API_ID` You can get your api id [here](my.telegram.org)

`API_HASH` You can get your api hash [here](my.telegram.org)

`PREFIX_HANDLER` Your bot handler which will activate commands

`DB_URI` Your [MongoDB](https://www.mongodb.com/) connection string.

`DB_NAME` Your [MongoDB](https://www.mongodb.com/) database name.

`OWNER_ID` Your user ID as an integer.

`GENIUS_API` Your Lyrics [Genius Api Token](https://docs.genius.com/#/getting-started-h1). To fetch lyrics of songs.

`BDB_URI` Your mongodb uri is different from the previous one to store more info.

`TIME_ZONE` Your time zone.

`RMBG_API` Your [removebackground api](https://www.remove.bg/api#remove-background) to remove the background/

`SUPPORT_GROUP`: Your Telegram support group chat username that users can contact in case of a problem.

`PREFIX_HANDLER`: Something like '/' to execute commands.

`SUPPORT_CHANNEL`: Your Telegram support channel username where users can see bot updates.

`DEV_USERS`: ID of users who are Devs of your bot. Use space to separate values.

`SUDO_USERS`: A space-separated list of user IDs you want to assign as sudo users.

`WHITELIST_USERS`: A space-separated list of user IDs whitelisted, cannot be restricted.

⚠️ **Note:** In case you are passing more than one value separate them using whitespace (space) for example If I want to pass more than one PREFIX_HANDLER
I'll pass it like `'/' '.' '!'` this.

YOU CAN ALSO HAVE A LOOK AT [VARS FILE](https://github.com/Gojo-Bots/Gojo_Satoru/blob/main/Powers/vars.py)

</details>

---------
  
# Adding your own plugin

To add your very own plugin just use the format given below and go through the [utils](https://github.com/Gojo-Bots/Gojo_Satoru/blob/master/Powers/utils) and [custom_filters](https://github.com/Gojo-Bots/Gojo_Satoru/blob/master/Powers/utils/custom_filters.py)
  
  ```python
  from traceback import format_exc
  
  from Powers.utils.custom_filters import command 
  from Powers import LOGGER
  from Powers.bot_class import Gojo 
  # All the import provided above is mandatory in case you don't want to use logger remove the first and third import 
  # Import more functions and modules as per your need
  
  @Gojo.on_message(command("<your command>")) # Pass additional filters if you need
  async def <function name>(<arguments to take>):
    <your code>
      
    '''use logger to add log info using LOGGER.info(<string>) in the platform on which bot is running 
      and error as LOGGER.error(<string>) and after LOGGER.error() use        
      LOGGER.error(format_exc())'''
      
  __PLUGIN__ = <name of plugin> # Pass the name of your plugin as string
  _DISABLE_CMDS_ = [<command as string>] # Enter the commands if you want so that they can be disabled if needed.

  __alt_name__ = [<command as string>] # Alternative name of the plugin
      
  __HELP__ = <string> # To tell about your plugin and commands you must use it
  
 
  # See any plugin to get more information about how to make a plugin 
  
 
  ```
  # Add plugins in [plugin](https://github.com/Gojo-Bots/Gojo_Satoru/tree/master/Powers/plugins) section
  ##  **Note** : Don't use <> this bracket while writing the code...
      
--------  
      
# Contributors
      
[![Contributors](https://contrib.rocks/image?repo=Gojo-Bots/Gojo_Satoru)](https://github.com/Gojo-Bots/Gojo_Satoru/graphs/contributors)


---------

# Special Thanks ❤️
      
<!----<p align='left'>
  <a href="https://github.com/iamPSYREX"><img src="https://avatars.githubusercontent.com/u/90316018?v=4" width="300" 
     height="300 alt="PSYREX"></a></br></br>
   
</p>--->

Some special thanks to the person/repo who/which helped and motivated me to create this project

* [PSYREX](https://github.com/iamPSYREX) for logos and motivating me and giving me new ideas.

* [Dan](https://github.com/delivrance) for [pyrogram](https://github.com/pyrogram/pyrogram) `library`

* [Anand](https://github.com/HellBoy-OP) for helping me to enhance the bot's security and look and also helping me out with various stuff and bugs and also for motivating me to create this project.

* [Alita_Robot](https://github.com/divideprojects/Alita_Robot) for base code.

---------

# Powered by [ɢօʝօ ɮօȶֆ](https://github.com/Gojo-Bots)


<p align='left'>
  <a href="https://github.com/Gojo-Bots"><img src="https://artfiles.alphacoders.com/160/160160.jpeg" alt="Gojo Bots"></a></br></br>
   
</p>

