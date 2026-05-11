# My-Home-Assistant-Card-Tips
Repo with home assistant card code and examples

Just a repo i made for myself and other home assistant geeks with code i've found/used.
Web searching sucks for the forums at times so i decided to put my tips on here to be more easily searchable

##Hourly-Weather Card:

https://github.com/seamonkey420/My-Home-Assistant-Card-Tips/blob/main/hourly-weather%20card

-swap the icon and the time around
-remove the bar background
-change weather icons to the lovelace weather icons vs wdi; also set the colors (even though i am not using them)

<img width="1212" height="512" alt="image" src="https://github.com/user-attachments/assets/143cc31b-c684-4601-b78d-da1130d477a7" />

##Weather-Forecast Card:

https://github.com/seamonkey420/My-Home-Assistant-Card-Tips/blob/main/weather-forecast%20card

-configure all text sizes
-remove the summary/current temp/info
-just show the next five days of highs and lows and conditions (to match my hourly).

you can use same method to swap elements around by using the margin-top/margin-bottom, sometimes you will need to set position as relative or absolute.

<img width="1198" height="506" alt="image" src="https://github.com/user-attachments/assets/33598ab3-fdab-477c-8fb5-3a01a27fc136" />


##Other Notes:

also, if you want to change the background color of a card that uses a style: and not a style: |, append this at the end of the cardmod code (found on this thread). otherwise the normal ha card background will work. 

changing certain cards to use the Style: | can break the formatting of items so below solution works w/those type of cards (mainly entity cards that you modify text / icon size for):
```
.: |
      ha-card {
        background: black;
      }
```
