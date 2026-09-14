# Gear
Projects for Equinox
 # my  Planetary Gear 

## this project was very suitable on the one hand to dive more deeply into Autodesk Fusion and on the other hand sharpen my technical thinking  (allthough this project is still very beginnerfriendly)

## Techstack: I used only Autodesk Fusion (and a sheet of paper for little notes)

## what is a planetary gear? A planetary gear is a structure out of many gears: the sun gear, which is the big gear in the center of the system, mostly 3 planet gears, which are the ones circeling around the "sun" and the ring gear on the outer site of the planet gears with internal teeth enclosing the planet gears.
## This device is used in many different products but has one main function it increases or decreases rotational speed and can also adjusts the torque (depends on the configuration). The main benefit of this device is that it can handle a very high power density, because it can handle a fast torque on 3 smaller gears on a smaller room. One factor why it is also used, when you only have little space spare is the coaxial alignment -->input and output shafts are basicly the same central axis. So it is often used in different types of engines, also in E-vehicles and bicycles but also in , for example, small smarthome devices, which is also one of the reason I wanted to learn about it and possibly implement it in my own projects in the future.

## the important part, which makes a planetray unique in some way is the gear ratio. 

## * ring gear          $$i = 1 + \frac{N_r}{N_s}$$
## * sun gear           $$i = 1 + \frac{N_s}{N_r}$$
## * planet gear        $$i = -\frac{N_r}{N_s}$$

 ## | ** ring gear **  |   | `$i = 1 + \frac{N_r}{N_s}$` |
 ## | ** sun gear **   |   | `$i = 1 + \frac{N_s}{N_r}$` |
 ## | ** planet gear **|   | `$i = -\frac{N_r}{N_s}$`    |

( ## these equations are relevant, because trough them you know at which ratio which gears makes on full turn. This is important for the torque, power density and later on the velocity. )

## So I chose a gear ration of 3: 
# * $$3 = 1 + \frac{N_r}{N_s}$$ |-1
# * $$2 = \frac{N_r}{N_s}$$
# * $$ 1{N_r} = 2{N_s}$$

## So I had to pick a value for the sun gear and then double it for the ring gear.
## Then I thought about one of my favourite relatives, who works for a big car manufacturer with engines and stuff (who also told me about planetary gears). And he appears to be 22, which was quite a fitting value (sorry for the unnessessary explanation).

# * $$ 2 = \frac{44}{22}$$ 
# * $$ 3 = 1 + \frac{44}{22}$$

## The equation makes sense, so my gear ratio was set.
### * but how about my planet gears? 
## This is also quite simple:
#  $$N_r = N_s + 2 N_p$$
# So: |-N_s
# $$N_r - N_s = 2 N_p$$
# So: $$| \frac{|}{2}$$
# $$ N_p = \frac{N_r - N_s}{2}$$

## with my current values:
# $$ N_p = \frac{44 - 22}{2}$$
## conclusion: 
# N_p = 11
# N_s = 22
# N_r = 44

## homeview:
![homeview planetary gear (Autodesk Fusion)](<final pg homev.png>)

## topview:
![top planetary gear (Autodesk Fusion)](<final pg top.png>)

## sideview:
![sideprofil planetary gear (Autodesk Fusion)](<final pg side.png>)

## f3d file:
[f3d file](<../Planetary Gear/Planetary Gear 2.f3d>)

## step file:
[stepper file](<../Planetary Gear/Planetary Gear 2.step>)

## stl file for cura:
[stl file](<../Planetary Gear/Planetary Gear 2.stl>)

## I also designed a plattform for the whole structure, but I decided to throw it away for now, so it wasnt my main focus.
![deleted plattform](Plattform(del).PNG)

## I did everything from measuring to calculating the sizes all by myself and used no help besides my calculator (sometimes)

## AI enclosure:
### I used AI:
* for researching the mathematical equations
* for instructions and tips on how to learn and implement new stuff in autodesk fusion 
* (+ recommending shortcuts)
* explaining errormessages in the software













