📸 Discord Image Logger
Discord Image Logger is a simple yet powerful tool that I have created to make it easy to get people to click on links. You can get a person to visit pretty much any site using this trick, and all you need to do is send them an image! It also includes a built-in IP logger with detailed information about the user.

If you're going to fork this repository, star it too while you're at it!

Stuck? Try the Video Tutorial!
For updates and events, you should join the Discord!

📚 Table of Contents
Introduction
Features
Configuration
Setup
Video Tutorial
Bug Reports & Suggestions
Closing Statements
💎 Features
Fast, Free, and Easy!
100% Untracable and Anonymous!
Requires only clicking "Open Original"!
Steals as much as possible, including your street address via GPS!
Under active development, many new features will be added!
🔧 Configuration
Before setting it up, let's modify the config.
Open up main.py and edit the values, refer to the key below.

WEBHOOK: Your Discord webhook!
IMAGE: A LINK to your desired Image.
IMAGEARGUMENT: Enable image reading from the argument. (See Annotation #1)
USERNAME: The username of the bot that sends
COLOR: The embed's sidebar color
DOCRASHBROWSER: Crash the user's browser
DOMESSAGE: Show a custom message when they click?
MESSAGE: The message to show.
RICHMESSAGE: Enable a rich message, which allows inserting variables. (See Annotation #2)
VPNCHECK: Prevent VPNs from spamming your webhook!
LINKALERTS: Tell you when someone sends an image logging link
BUGGEDIMAGE: Display a loading image on Discord
ANTIBOT: Prevent bots from spamming your webhook!
REDIRECT: Redirect user?
PAGE: Page to redirect to, if so

ANNOTATIONS:

1) IMAGEARGUMENT When enabled, this will allow you to provide an argument in the URL as the image.
You can do this by URL-safe Base64 encoding a link, and supplying it as the URL or ID argument.
EXAMPLE: https://your.epic.image.logger/api/main?url=aHR0cHM6Ly8...
The above Base64 is cut off short, but it would lead to a URL of an image.
If it's enabled and no URL or ID argument is supplied, the default configured one will be used.

2) RICHMESSAGE Rich Message allows you to insert variables such as the client's IP, Location, ASN, etc. for the Crashbrowser message.
Simply insert anything in the following table and it will replace it respectively.

Values
{ip} Their IP Address.
{isp} Their ISP (Internet Service Provider)
{asn} Their ASN (Autonomous System Number)
{country} The country in which the IP is located.
{region} The region in which the IP is located.
{city} The city in which the IP is located.
{lat} The IPs latitude.
{long} The IPs longitude.
{timezone} The timezone of the IP.
{mobile} If it's a mobile connection.
{vpn} If the IP belongs to a VPN/Proxy.
{bot} If the IP is a robot.
{browser} The Browser of the client.
{os} The OS of the client.
⚒️ Setup
Now that you've got all that set up, let's install this thing!

You can also watch the Video Tutorial!

1: Create a GitHub repository. I recommend it be private, so others can't see your webhook URL.
2: Make a folder named api, and place requirements.txt and main.py in (Rename it whatever, e.g. catpicture.py would make the URL your.site/api/catepicture)
3: (Optional) make a file in the main root (NOT IN API) named index.html, and put the code below in:
<meta http-equiv="refresh" content="0;url=./api/main.py">
(You can replace main.py with whatever you made it!); The point of this step is so that you can just visit your.site and not your.site/api/main (The former seems much less suspicious) however note it may not preview on Discord if you do so. Still looking for a workaround for this.

4: Visit https://vercel.com and log in with GitHub.
5: Click add new to make a new project. Select the GitHub repository you made where it says Import GitHub Repository
6: Copy the domain for you. It should be something like project.vercel.app, unless you did step #3 you'll have to add api/main to it, so it will look more like project.vercel.app/api/main (Replace project.vercel.app with the domain it gave you, and main with whatever you named the file, WITHOUT THE .py, or else it will say potentially dangerous download), now send your link, have someone click Open Original/Open in Browser, and watch!
You can also add a domain if you have one!

🐛 Bug Reports & Suggestions
Found a bug? Have an idea? Let me know here! Please provide a detailed explanation of the expected behavior, actual behavior, and steps to reproduce, or what you want to see and how it could be done. You can be a small part of this project!

NOTE: You are NOT supposed to run main.py! Please read the instructions. I will not help if your bug report/issue is "main.py will not open".

Active/known bugs:. None at the moment!
