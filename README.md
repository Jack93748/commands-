# commands-
{
    "token": "Put your token here that you want to use",
    "channel_id": "ID of the commands channel",
    "message": ".follow gggdgdf"
from flask import Flask
from threading import Thread

app = Flask('')

@app.route('/')
def main():
    return "Ready!"

def run():
    app.run(host="0.0.0.0", port=8080)

def keep_alive():
    server = Thread(target=run)
    server.start()
    
