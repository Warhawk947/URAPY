# Introducing URAPY
## What is URAPY?

URAPY stands for **U**ptime **R**obot **API**, but I wanted it to be more cheesy so I switched it to **APY** (Get it? API? APY? Ok...)

URAPY is a basic API wrapper for [Uptime Robot](https://uptimerobot.com/), allowing you to control monitors and public status pages via your python terminal!

## How do I use URAPY?
It's actually very simple to use! To install the package, simply type `pip install URAPY`, and you're good!

#### Getting your Uptime Robot API key
Now, before you write any code, you need to get your *Uptime Robot API key* *(If you already have one, copy it to your clipboard and skip this part.)*. To get it, all you need to go is go to [your settings](https://uptimerobot.com/dashboard.php#mySettings). You should see something like this:
![image](https://storage.googleapis.com/replit/images/1586984485972_47263dee2b4461a1714fa5fb6e8b14f8.png)

Now scroll down until you see the header called *Main API Key*. Click the text that says *Create the main API key*, and then click the big blue button.
![image](https://storage.googleapis.com/replit/images/1586990215066_b156298b39e5edef293825ad40d3dd3b.png)

You should now see something like this:
![image](https://storage.googleapis.com/replit/images/1586991754336_c55a1df9a6e5152afde96c6b67ed684c.png)
(Btw I'm not giving you my API key because then you'll hack me TwT)

#### Back to the Coding!
Type the following into your IDE.
```py
import URAPY as u                              # Imports the Library
client = u.Client(<paste your API key here>)   # Initializes the Client
print(client.get_account_details())            # Get some Account Details!
```
It should spit out something like this:
```
{'email': 'dont_stalk_me_pls@gmail.com', 'monitor_limit': 50, 'monitor_interval': 5, 'up_monitors': 2, 'down_monitors': 0, 'paused_monitors': 0}
```
Congratulations! You've just written your first program with URAPY! If you get something like `ModuleNotFoundError: No module name 'URAPY'`, try reinstalling URAPY (`pip install URAPY`).

Refer to official docs [here](https://urapy-docs.warhawk947.repl.co/) |
Visit Uptime Robot! https://uptimerobot.com/
