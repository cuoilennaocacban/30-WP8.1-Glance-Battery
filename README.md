# 30-WP8.1-Glance-Battery
Display percentage of battery on Lumia glance screen

Nokia Lumia (later is Microsoft Lumia) have a feature call "Glance Screen" on some devices. A restricted amount of information can be display on this screen

## Restricted information
Only some information can be displayed on the glance screen. For developers, there is only 1 type of information can be displayed: number of notifications from their apps

One drawback for this information is it can not diplay number larger than 99

## The idea
The idea is to create a "fake" notification to display the percentage of remaining battery. And when the battery reach 100%, make it disappeared.

## Update the percentage
To update the percentage, when the first started of the app, it will register a background task to check battery percentage every 15 minutes, then update the fake number of notification.

## Futures
If microsoft open more API for glance screen, there will be more cool stuff to do with it (right now, microsoft apps can display a whole grey out, colorless picture, another app also from microsoft can display weather information on glance screen)
