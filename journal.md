# Astra: The AI Quadruped dog
## What is this?
 - A dog which acts as a companion robot dog.
 - Uses Actuators with planetary gearbox and multiple sensor for advanced AI!
 - Using jetson nano orin super (raspberry pi using for testing)!!!
<hr>

## Day 1: Research and starting fusion
I have already researched enough­. imma start.  
Opened fusion, set up a new project and started with the leg design.  
Okay im using carbon fiber rods for the leg! I chose carbon fiber because it’s super strong and lightweight so the motors don’t need to work as hard.  

And for the foot im using a silicon molded ball thing :suspect:  
![image](https://github.com/user-attachments/assets/a484d9ee-e3fb-4956-9189-59755a48dcfe)  

A somewhat completed foot 🦶. I made the socket in fusion so the ball can snap in tightly but still move a bit to absorb shocks. Modeled a curved base so the silicone grips the floor better. This will help the dog run without slipping.  

## Day 2: I dint show you something b4
I actually had started designing 2 ACTUATORS. One was using a [camera motor](https://shop.iflight.com/ipower-motor-gm5208-12-brushless-gimbal-motor-pro279?srsltid=AfmBOorSPDTZzSXuuPQEK-6dXlJDZKPpKBmCNM_RbTE9hdy-FQK5-I5s) - i forgot whats that called. but that only had 2.5kg/cm which i had observed after an entire day.  
I modeled the casing, made a basic planetary gearbox to try boosting torque, and even planned the mount holes.  

Faliure photo :( -  
<img width="800" height="691" alt="image" src="https://github.com/user-attachments/assets/45ea33c6-00d5-4e5f-b279-b606f09da980" />  

I was going to make like a planetary gearbox but nvm.. torque too low so pointless.  

Then i thought i would use the eaglepower 90kv motor just like [Aaed Musa](https://www.aaedmusa.com/). I designed a custom gearbox for it in fusion, added space for a magnetic encoder, and was almost done. But later i realised it would become too expensive after me buying odrive s1's.  

So i went on alibaba and the chepaest thing which i found which has an encoder and driver built into it was this motor  

THE GIM6010-8!!!!!!!!!!!!!!!!!!!!!!  
This was the perfect motor because it had a stall torque of 11n.m and the motor was tested by someone over [here](https://hackaday.io/project/202366-the-unnamed-spider-bot/log/239789-steadywin-gim6010-8-stock-controller-vs-odrive-vs-tinymovr)  
Also this has a driver and it has like planetary gaerbox in it. so this was perfect. and it was kinda cheap. bruh - 70$ 💸  
Can someone help me rob a bank 💰.. jkjk dont call 911  
Yeah, wasted i gues 3-4 days on deciding a motor.

## Day 3-5: Designed something :)
<img width="527" height="720" alt="image" src="https://github.com/user-attachments/assets/2479ea3e-21bd-4bdd-a5e8-79031847fe31" />  

If you can see these are gt2 belts. so like the motor will stay on the hip but drive the knee axis.  
I modeled the motor bracket, belt pulleys, and tensioner in fusion so the belt stays tight even after long use.  
This is actually useful because research showed that the battery would drain faster if the motor was near the knee because of incraesed weight 🤓. So yeah, moving the motor higher saves energy and reduces leg inertia.  

## Day 5-10: did very little stuff
Im very distracted. but I still made the knee, hip, and abduction joint (aka moves your lige side to side) models ready in fusion.  

Here’s some final thingies for all axis -  
<img width="768" height="710" alt="image" src="https://github.com/user-attachments/assets/af21569c-1b7a-4061-a7fb-c2848313d185" />  
<img width="687" height="747" alt="image" src="https://github.com/user-attachments/assets/2b7f7a8e-bfe6-4666-a015-4e262485f24d" />  
<img width="788" height="663" alt="image" src="https://github.com/user-attachments/assets/50e04550-c8cb-45ac-8262-d855f62e2327" />  
<img width="1002" height="634" alt="image" src="https://github.com/user-attachments/assets/73c51646-343d-488b-9573-8464e38bd3d5" />  

So basically the leg was done! I modeled every mounting hole, designed bearing housings for smooth motion, and made space for the belts to run without rubbing.  
Also added attachment points for the carbon fiber rods so they can slide in and be locked with screws.

## Day 10: Dont ask me why is this so complex..
Yeah i just realized it would be hard to 3d print and assemble some parts. so fixed my issues!  
Went back in fusion, split some parts into two pieces so they can fit on my printer bed, added alignment pins so they fit perfectly when assembled. Also thickened a few parts for strength and added more space for tools to reach bolts.

## Day 11-13: Final Full dog design.
Today I designed my almost complete dog.  
<img width="862" height="757" alt="image" src="https://github.com/user-attachments/assets/5f591f54-7b1a-448d-ab76-287098ec5f76" />  

I took the individual legs and assembled them onto a main body frame in fusion.  
Designed the body plates with holes for ventilation and mounts for electronics. Made space in the center for battery and Jetson Nano Orin Super (and Pi for now).  
Also routed cable channels so all wiring will be hidden and won’t get caught while running.  
Even added small gussets for frame strength because carbon rods + 3D parts can flex if not supported.  

I also finished my overly expensive [BOM](https://docs.google.com/spreadsheets/d/1tXSbPTXzO7x9RjKfoS4aTnTzwVyE0GcGUCTSj2ZbIsA/edit?gid=0#gid=0).  
Right now i am not adding sensor mounts and all to my dog since i will test my ai stuff and then add sensors and all for autmoated dog exploration.

I am not sure if it looks good. But remember to star my repo ⭐

## Day 11: Final stuff
Some final adjustments, submitted in highway pitstop channel.  
Double checked the belt alignment in fusion using the joint animation feature to see if there’s any clash. Printed some test pulleys to see if they fit the belt perfectly.  
Tweaked bolt hole sizes for M3 hardware so I don’t have to force them in later.  
Feeling good about this now.
