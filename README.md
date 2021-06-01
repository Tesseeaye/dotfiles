# dotfiles
Dotfiles for the Nordic theme I modified for Openbox

* I'll edit the readme later with more instructions. I'm still learning how to set all of this up outside of my archcraft install.

June 1st, 2021: Added my own version of the Nordic theme's polybar. I rewrote some of it by starting with the basic config from Polybar's documentation and copied over what I liked from the Nordic theme. Most of this is still written by the original author; adi1090x. I've changed the font of some of the icons and learned a bit more about how I was using the modules I found [here](https://github.com/polybar/polybar-scripts) and was able to clean them up a little. I still don't know how to make it so I can use one weather script, but essentially it's making the same calls twice to OpenWeatherMap.

To get the weather to work correctly you'll need to add your city and API token for OpenWeatherMap into both weather bash scripts in `~/.config/polybar/cyberbar/scripts/` directory. I know the bare minimum of bash, and don't know how/nor care at this point to clean up those files to just fetch the weather with no fluff. 

I also had it set up so if I clicked either the icon or the temperature, it would open a link to weather.com and show me the forecast in firefox, you can do that too, or maybe set it up for a terminal command to show your weather in the terminal. If I reference firefox or alacritty in my files you'll have to change it to whatever you use.

Another thing, I switched the date module for a calendar module. When you click the date/time it shows a small calendar, I had issues with the script, the calendar was on the wrong monitor. I didn't know what was actually going on in the bash script to determine it's position, but I knew where, so I just hard coded the x value that I wanted it at. You'll want to change this probably.

The cyberbar only comes with the modules it displays out of the box. I may add more in the future, but I designed this one to be the way that I like it to look on my desktop, but customize it however you want and upload it where ever you want :)
