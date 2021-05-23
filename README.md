# Telegram-Bot
##### By BiragadeeshwarnDEV
Code: 
```
from telegram import *
from telegram.ext import *

bot = Bot("1891311861:AAGn4suWUH1Lg3p4OAwWIHbDXKw9XHHk6ZY")
#print(bot.get_me())
updater = Updater("1891311861:AAGn4suWUH1Lg3p4OAwWIHbDXKw9XHHk6ZY",use_context=True)

dispatcher = updater.dispatcher

def test_fuction(update:Updater,context:CallbackContext):
    bot.sendMessage(
        chat_id = update.effective_chat.id,
       text="Hi Iam SharkTHEbot I Can Share Files And That Only "
    )

start_value = CommandHandler('start',test_fuction)

dispatcher.add_handler(start_value)

def test_fuction1(update:Updater,context:CallbackContext):
    bot.sendMessage(
        chat_id = update.effective_chat.id,
       text="Hi, Try /latestvideo"
            " /whoareyou"
            " /bestwallpapers"
    )

start_value = CommandHandler('HELLO',test_fuction1)

dispatcher.add_handler(start_value)

def test_fuction2(update:Updater,context:CallbackContext):
    bot.sendMessage(
        chat_id = update.effective_chat.id,
       text="This Is My Favarioute Acounts https://t.me/LetItRipple, https://t.me/Yourswallpapars "
    )

start_value = CommandHandler('bestwallpapers',test_fuction2)

dispatcher.add_handler(start_value)

def test_fuction3(update:Updater,context:CallbackContext):
    bot.sendMessage(
        chat_id = update.effective_chat.id,
       text="How I Code My Telegram BOT Promo - https://www.youtube.com/watch?v=3NuCIq0lPKU, Python Music Player || TechGenix Tamil - https://www.youtube.com/watch?v=PXwFEgfHNEY, Make Discord BETTER! - https://www.youtube.com/watch?v=iGpnT0fKryw "
    )

start_value = CommandHandler('latestvideos',test_fuction3)

dispatcher.add_handler(start_value)

updater.start_polling()
```
