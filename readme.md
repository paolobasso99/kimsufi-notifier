# Kimsufi Notifier
This is a simply python 3 script that checks OVH api to see if one or more specified [Kimsufi](https://www.kimsufi.com/en/) models are available.

## Why 
Some Kimsufi models (like KS-2) are never in stock. These servers are ridiculous cheap so as soon someone cancel their subscription someone else grabs the server. I really wanted to rent this server and this tool helped me, it took 2 months with a check every 10 seconds to rent a KS-2.

# Requisites
For the notifications this app uses my [personal-notifications](https://github.com/paolobasso99/personal-notifications) service that has to be hosted on a server. Check the [personal-notifications page](https://github.com/paolobasso99/personal-notifications) in order to configure it.

# Setup
1. It is higtly recomended to use a python `venv`, to setup it, for Linux go inside the project's root and type: `python3 -m venv venv`.
Then you can activate the venv using: `source venv/bin/activate`.
Next install the required packages: `pip install -r requirements.txt`.
Now you can exit the `vevn` with `deactivate`.
2. Copy `.env.example` to a `.env` file and personalize it.
3. You can start the script in the background with `nohup /project/venv/bin/python /project/app/app.py &`
4. If you want to stop the program you need to kill its process
