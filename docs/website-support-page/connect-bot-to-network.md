## Connect Your Bot to a Network 

In order to get under the hood to perform updates, password recovery or extra customization, you'll need your Raspberry Pi connected to a wired network so that you can SSH in. Wireless access is disabled for security reasons.

### Step 1 — Plug the Raspberry Pi into your Wired Network
- Plug your Raspberry Pi into your networking switch/hub/router as if it was another computer you wanted to access the internet.
- It is very important, if you are using a kit that you use the Raspberry Pi's port and not one of the Dispenser ports by accident. This may cause damage to your networking equipment, your Bartendro Router or both.

### Step 2 — Find your Raspberry Pi's IP Address
- The easiest way to do that is to get into the administration section of your networking router.
- Most routers use the 10.0.0.0 or 192.168.0.0 subnet. Look up your router's address for administration. Try 192.168.0.1 or 10.0.0.1 in your browser's address bar.
- You will likely be prompted for a password. You will have to dig this up for your specific router, but they are usually very simple with defaults like login:admin password:password.
- If your can't log in with the default password, then resetting the router with the button in the back should restore it to all defaults.

### Step 3 — SSH into the RPI
- Use a terminal window or program to SSH into the RPI.
- On a Mac run Terminal.app and type SSH bartendro@x.x.x.x replacing the x's with the IP Address you acquired in the previous step.
- On a PC, install putty.exe if you don't already have it, and enter the IP address in Host Name box.
- Use the following credentials (case-sensitive): bartendro / hackme!

[Source: http://support.partyrobotics.com/Guide/Connect+Your+Bot+to+a+Network/9]
