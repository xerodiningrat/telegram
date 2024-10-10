from telegram import Update, Bot
from telegram.ext import CommandHandler, CallbackContext, Updater

# Fungsi untuk memulai bot
def start(update: Update, context: CallbackContext):
    update.message.reply_text("Selamat datang di PREMIUMISME APP!\nList Produk:\n\n[1] AI CHATGPT+\n[2] AI CLAUDE\n[3] AI PERPLEXITY\n[4] AI YOU\n[5] ALIGHT MOTION")

# Token bot dari BotFather
TOKEN = "7374135142:AAEMJiDyHCbTPcH_moxowNVJuXt-mFcSbho"

# Buat updater dan dispatcher
updater = Updater(token=TOKEN, use_context=True)
dispatcher = updater.dispatcher

# Buat handler untuk command /start
start_handler = CommandHandler('start', start)
dispatcher.add_handler(start_handler)

# Jalankan bot
updater.start_polling()
updater.idle()
