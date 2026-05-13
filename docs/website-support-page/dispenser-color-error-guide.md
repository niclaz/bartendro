## Startup Dispenser Color Guide

While the bot is booting, Dispensers will turn certain colors. This guide will demystify what these colors mean.

### Step 1 — Solid Green, Blue and Off
- This is perfectly normal. While the Raspberry Pi is booting up, it isn't quite at a state where it can send logical communication to the Dispensers yet.
- After about 1 minute, the RPI should be fully booted and commanding the Dispensers with a color changing pattern.

### Step 2 — Flashing Blue followed by Solid Red
- About 3 seconds after power has been applied, the Dispenser flashes blue twice then turns solid red. This is an issue that we've seen on occasion. It is more likely to pop up on Rev3 dispensers than Rev2 dispensers.
- It is usually an intermittent issue, but there are a few things that help. Try using a different cable, one that is short, like under 2ft and is of good quality. Also, make sure that the RJ-45 plugs are firmly seated in their connectors.
- We are working to find a more global solution to this problem. Since it is intermittent it sometimes works normally. You can save time by power cycling as soon as you see the dispenser flash blue.
- You will also notice, that after a full boot that the Dispenser will go into a normal looking color changing pattern, and even show up in the UI. Don't be deceived though, it will not function properly. You will also likely notice that in the Admin > Debug menu that the Dispenser will be recognized with an ID of 3F.

### Step 3 — Flashing Red
- You should only see flashing red in pairs, or numbers greater than 2. That's because this is a Pump ID conflict.
- You can confirm this by looking at the back of the Dispenser(s) to see that indeed you have two pumps with the same ID.
- We do our best to make sure that we don't ship Dispensers with conflicting IDs, but if we had a slip and this happened to you, contact us at support@partyrobotics.com and we'll swap out one of your conflicting boards.

### Step 4 — Solid Red on Boot
- In rare cases, the Dispenser will turn red immediately once power is applied. This is usually an indication that the firmware on the Dispenser or EEPROM has slipped into the ether. This can almost always be recovered by reprogramming the Dispenser.
- If you have the ability to reprogram the Dispenser, then go for it. Otherwise, you can contact us and we'll arrange a way for you to return it to us so we can re-program it for you.

[Source: http://support.partyrobotics.com/Guide/Startup+Dispenser+Color+Guide/8]
