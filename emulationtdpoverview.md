# Emulation TDP Testing

## Story:
Recently we have been testing power consumption on the deck after seeing some interesting results online from other deck users showing off some impressive performance per watt.  
Naturally we wanted to get in on some testing and came up with the following baseline we hope everyone can follow:

- Docked mode - Similar to the Switch, Docked Mode is any time the deck is recieving power from an external source.  The idea here is when in docked mode, we treat
the deck like a desktop and give it everything it has to maximize visual quality as well as performance, targeting stable 60 FPS

- Portable mode - Any time the dock is not recieving power, regardless whether it is connected to a dock.  (Docks can be connected without power and will drain the battery
faster for example)

About about the deck battery:
https://www.steamdeck.com/en/tech/
 - Per the valve website, the deck is rated at 40WHr, and valve indicates that the deck will last approx 2-8 hours.  This essentially breaks down to:
 - The Deck uses a 45w power supply
 - 
 
 20w TDP / 40WHr = 2 Hr batter life.   10w TDP / 4WHr = 4 Hr battery life.   5w TDP / 40WHr = 8 Hr battery life.  

 So the goal is to get the total TDP down to as close to 5w as possible for the maximum amount of battery the deck can put out.  Obviously this will not be possible
 for some games and emulation that are more modern, but that also doesnt mean that we can't push our TDP down as much as possible without sacraficing a stable FPS on 
 games from generations inbetween.  


| Lowest TDP | Lowest CPU MHz | Lowest GPU MHz | 
| ------ | -------|
| 3w | 400 MHz | 400 MHz |

| Lowest Total TDP | Lowest CPU TDP | Lowest GPU TDP | 
| ------ | ----------- | -------|
| 5w | .3w | .3w |

## Emulator TDP Settings

### N64 Portable TDP settings

| TDP limit | CPU MHz | GPU MHz | Total TDP | 
| ----- | ------ | ------ | -------- | 
| 5w | 400 MHz | 400 MHz | 5w TDP |


### Switch Portable TDP settings

| TDP limit | CPU MHz | GPU MHz | Total TDP | 
| ----- | ------ | ------ | -------- | 
| 10w | 2700 MHz | 1000 MHz | 22w TDP | 



## Things that effect TDP Consumption:
1. Display Brightness - Turn down to reduce TDP
2. Turn off Bluetooth and Wireless intennas 
3. Turn off FSR when not using it
4. 


