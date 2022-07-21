# PoyomannSteamDeckThemes

## Tips for making your own:

### You'll need:
1. [Decky/Plugin loader](https://github.com/SteamDeckHomebrew/decky-loader)
2. [The css loader](https://github.com/suchmememanyskill/SDH-CssLoader/tree/dev) 
3. Some means of file transfer from PC to steam deck.
    1. I would recommend sshd, which can be turned on by
    2. Adding a password with 'passwd' in Konsole
    3. 'sudo systemctl enable sshd' in Konsole
    4. 'sudo systemctl start sshd' in Konsole
    5. You're now running an ssh server from the steam deck, find some way of connecting to that from your PC

### Steps:
1. Install the RGB keyboard theme into the css loader's theme folder home/homebrew/themes (the rgb one has actual comments)
2. Add a new css file in one of the RGB keyboard's folders (whichever you feel like really)
3. Modify the .json file so your new css file is added as an option
4. Make some changes to some variables in your new css file, and reboot into game mode to see if it works.
4a. I would reccomend changing the variables set in :root as they're the most important.

5. Now that your custom css is working, it's time for the work to begin. (not a step, shh)
6. Go to chrome://inspect and add your steam deck's IP address with port 8081
7. You should be able to see SP as an option, click on that.
8. You should now have a live feed of your steam deck's homepage + the keyboard if it's open
9. On the right of your screen, there's an inspect element menu, changes can be tested here and **will revert on reboot**
10. Find things you want to change, and add them to your .css file

10a. This is where having sshd comes in handy, you can edit the css file on your desktop, and have it automatically save to the steam deck.

11. Keep at this till your keyboard looks how you want it, and then post it on r/steamdeck for epic reddit karma :p

### Notes:

If you want to customize an individual key, use either of these methods:
`div[data-key-row="1"][data-key-col="2"] {background-color:#FFFFFF;}`
or
`div[data-key="w"]{background-color:#FFFFFF;}`
The top option changes keys based on where they are in the keyboard, and the second based on what key they are.
Both options work, choose whichever's easiest/most readable.


## Currently contains:

### RGB keyboard theme
An RGB keyboard, with lots of customizability.
Both the 'rainbow' and 'deck colours' patterns were made by suchmememanyskill, who also made the CSS loader

https://user-images.githubusercontent.com/48649272/179416332-b47eed4c-5b42-4b7d-bb40-b1b69de6288c.mp4

https://user-images.githubusercontent.com/48649272/179416334-4b7c7eb5-faa7-4a7d-8ca2-847f70ead44a.mp4

https://user-images.githubusercontent.com/48649272/179416331-57e73a48-46e6-40af-b99b-7f9ec7bd253f.mp4


### Astolfo keyboard theme
A pink Astolfo keyboard, made for fun.![AstolfoBlack](https://user-images.githubusercontent.com/48649272/179416386-eb74df5b-94de-444a-becb-28dfed7eb7a1.png)
![AstolfoPink](https://user-images.githubusercontent.com/48649272/179416388-fdf00675-2f32-4da8-b67c-3fe9eaff30bf.png)
