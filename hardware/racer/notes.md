Hey, 

Super inspired by this project, looks really cool and I love the open source aspect so thank you! 

I'm starting from scratch and scrabbling in the dark a bit, so I thought I would document my thinking before I commit to the expensive and slow iteration part of the process (ordering a junk pcb because I made a mistake). I'm not explicitly asking for help from the maintainers, but if you want to steer me in the right direction, It'd be much appreciated. 

My experience is somewhat common: good programming experience, very novice solderer, no PCB design experience, so I'm going to follow my nose and see where it gets me.

First, the hardware. I see a KiCad project. KiCad seems to be FOSS software for managing the design of PCBs. https://www.kicad.org/download/ 

I downloaded the project and installed it. You can load the KIcad project and have a look around, pretty cool but I don't understand it one bit :D. Seems like the important concept is layers, one for later :D. (n.b. the font chosen is not present on a default Windows install).

![image](https://github.com/user-attachments/assets/6965bad9-3fa6-4eee-8bef-0bc664791954)


After a bit of searching, it looks like a good candidate for getting the PCBs built is jlcpcb, I'm sure there's a reason why they're so cheap, but as a novice, price is king as I'm certain to make some mistakes. It asks for a gerber file, this is the .zip file in the repository. This loads nicely.

![image](https://github.com/user-attachments/assets/b49f985d-cce4-4c6c-badd-ee6263755149)

I'm going to assume the defaults are reasonable....

Now I get offered assembly. I'm assuming assembly is soldering on the parts. Sounds good. I'm going to choose to assemble the top layer so I get a balance of soldering practice and time spent. Again default options. I don't know what a stencil is so I'm not going to order one 😁

Next I get asked for a BOM (which I know is bill of materials) and a CPL file, which is apparently a pick and place file. I can see a BOM but not a pick and place file. I do the lazy software engineer thing and look for a way to generate one from KiCad. I don't find one, so I google "KICad CPL jlcpcb" which leads me to this plugin https://github.com/Bouni/kicad-jlcpcb-tools. After following the install instructions I can now generate a CPL file. It seems to generate a separate gerber file, which I assume is more tailored towards 

![image](https://github.com/user-attachments/assets/cfc8337d-e78a-43bf-b59e-baca2810b615)

