## Engineering Journal
By Stephen Harris

**Date: Tuesday, Jan 7, 2025** \
*Subject: My new Engineering Journal sucks* \
I will be honest, at first I was sceptical about keeping an "engineering journal". Although I quickly realized that this would be an opportunity in disguise. For there are many things I am learning or plan to learn over the coming weeks, which I will discuss. But even better is that this provides with me the perfect opportunity to complain about my least favorite languages, or bash on the frustrating decisions of my engineering professors at the SET. I even have a few plans in mind for future topics in my engineering journal.

**Date: Thursday, Jan 9, 2025** \
*Subject: C++ sucks, but not as much as Javascript* \
Listen, we all know it. At least everybody who has learned any better language knows it. C++ is just not good. But it would at least be preferrable to Javascript, as I can at least pretend it is C.
You see, I am taking Bart's graphics class this semester. Javascript is already a language I am familiar with. But my lord I am quickly learning that some of the webapi's for javascript are just god awful. Especially in an untyped language such as JS. Especially WebGL. If only there was some way to make it typed...
Actually, that is exactly what I am planning to do.
Bart gave us a framework to base our assignments off of. And it makes these assignments stupid easy. How am I suppose to learn how to use webgl if bart already wrote it for me? Therefore, I have decided to rewrite his entire framework in C, and then compile it to webgl to be implemented into a web enviroment.
It has honestly been a great learning experience in learning the opengl api, and in compiling C to webasm. I already have most of the framework written. I just need to find or implement my own library for handling matrices so that I can set up the viewport matrices.

**Date: Tuesday, Jan 14, 2025** \
*Subject: The Turbo Regatta sucks* \
I am going to be honest, I am not excited for the upcoming design day's Turbo Regatta. They are really stretching the premise to try to include Computer Engineers in working on this project. What's worse is that this event is going to heavily cut into lab time for my Embedded Systems II class. *I'm sure it will be* so *worth it.* \
&#9; *sigh...* \
At least there seems to be prospects for me to learn how to design a PCB board. That I do look forward to.

**Date: Friday, Jan 17, 2025** \
*Subject: Webasm sucks* \
I have been spending the past two weeks trying to compile C to Webasm and Javascript. Even with tools such as Emscripten that provide an entire wrapper library for the C standard libs, it is still a nightmare to develop with.
For instance, what is to stop you from trying to allocate global memory for a struct with a flexible array member, but to accidentally allocate the space for the flexible array member in a completely different part of memory, thereby overwriting vital JS objects for the printf wrapper, thereby causing all subsequent calls to printf to fail dramatically?
Anyhow, through this process I have managed to learn things about emcc, javascript, webgl, and even C. And it *almost* works. I just need to get the viewport matrices right. I should probably just start with a simpler render model, and then branch out from there.

**Date: Tuesday, Jan 21, 2025** \
*Subject: VS Code Sucks* \
Let me tell a tale of my history with IDEs. Less than a decade ago when I was first learning programming, I was getting a little tired of using Windows Notepad for writing anything other than batch scripts. I realized that I needed to find an IDE. I tried many of them. Eclipse, Code::Blocks, NetBeans. and they all within the perview of my own subective belief to be utter *garbage*. They were heavy, slow, resource consuming, they were saturated with features I didn't want, menu littered with buttons and viewports and margins, they enforced project formats, took up more than reasonable space on your hard drive (in my opinion), had agregious startup times with those stupid startup banners. It wasn't until I realized that you could use a compiler without an IDE that I ditched the whole IDE scene and just found a good old-fashioned text editor with code highlighting (via Notepad++), and called it good. I used Notepad/Notepad++ for years until my Windows operating system decided to commit Seppuku so hard that it wiped the very fabric of my hard drive's partition sceme off the drive such that neither the partition recovery nor file recovery could recover anything other than the Windows boot partition after two arduous 48 hour scans of my hard drive. 
To make matter short, I switched to linux, installed a command line distro, never installed a desktop window manager, and lived the rest of my days on the command line interface with my command line editor of choice, where everything is simple, lightweight, minimalistic, documented, and yet still *powerful*.

**Date: Wednesday, Jan 22, 2025** \
*Subject: Code Composer Studio Sucks* \
The previous entry was really a preface to this entry. I am very resistant to ever using an IDE, and I will go to great lengths to simply not use an IDE, or really anything with a startup time greater than one second (which happens to include virtually every IDE).
This brings us to Code Composer Studio. In my Embedded Systems II class, we have to use Code Composer studio in order to program this archeic MSP430 microcontroller. Based on our labs, the CCS IDE is kind of awful, and absolutely convoluted. I am completely resolved to never using CCS for the rest of this class. My mission has been to remain on the command line with a good ol-fashioned makeflie to handle all the tedious parts. This path I have taken has been met with... mixed results. Both me and Jason have been spending the past few days trying to compile both C and Assembly independant of CCS, and flashing it to the microcontroller. I found an official TI GCC toolchain for compiling to the microcontroller, as well as an official tool for flashing. We actually got the C code to compile and flash to the microcontroller successfully, with expected behavior. However, we ran into a great multitude of problems whilst trying to assemble our assembly code, and have spent the rest of the day trying to figure out how to get the assembly to work. At this point I am pretty sure the msp430 versions of objcopy and the objdump executables are buggy and unreliable for extracting the hex for flashing.
However, I am moving onto the next phase of my plan. I downloaded CCS today on my pc, and not because I plan to use it. But instead, I realized that the CCS has it's own dedicated toolchain of C/C++ compilers, debuggers, assemblers, hex extractors, and flashers. Each and every single one of them a *completely standalone executable*. They were all beautifully standalone, and each of them have some measure of documentation if you know where to look. The CCS toolchain appears to be exclusively found within the CCS installer, as I could not find them anywhere else on the World Wide Web. But that should pose no problem. The wonderful standalone CCS toolchain is just a copy-and-paste away from being relocated to my project directory, and I could thereafter delete the Convoluted Code Composer Studio from the face of my digital world.

**Date: Tuesday, Jan 28, 2025** \
*Subject: Kicad is actually good? Nah, Kicad sucks* \
So my Turbo Regatta group were planning to go with a pcb design for our electronics. However, I have been finding that a terrible pain. Kicad is honestly kind of nice, but it isn't logisim nice. Good enough to design a PCB board with at least. However, the biggest issue is being able to find PCB parts that can be imported into Kicad. But even when you do, Kicad's import tools are absolute garbage. Like, good heavens please end my misery.

**Date: Monday, Feb 10, 2025** \
*Subject: I suck* \
Whoops. I kind of forgot about this journal. Well, time to make up for lost time by adding two entries this week.
So I guess what I did this and last week: I love showing off to my professors. This week for my graphics class we were assigned to create a bunch of bouncing balls with gravity for an assignment. The problem is though that I did such a good job writing the physics engine and with keeping everything vectorized that I 'accidentally' made a 3D ball collision framework. And in order to use it for 2D balls, I simply just stacked the balls so perfectly aligned on the z-axis that they ignored the z-axis entierly. That was, until I accidentally added a tiny force on the z-axis, causing the 2D stack to become unstable and collapse into a 3D stack. And well, when that happened, I figured, why not go all the way? So I generated a spherical mesh using longitudal strips, wrote a vertex shader that encorperated directional lighting. That was the first time I ever successfully wrote shader code. And honestly... I love it.

**Date: Monday, Feb 11, 2025** \
*Subject: WebGL sucks* \
I am lying a little with the title that WebGL sucks. But I have to keep up the naming theme, you know?
Anyhow, WebGL is still kind of a pain, and I would like it a lot less if it weren't for programmable shaders. In fact, I have since discovered a shading language specific to Microsoft's DirectX called HLSL. And as much as I love GLSL shaders, I *love* HLSL. It's language philosophy and approach to programmable shaders is just... it's so good. You can upload vertex data as struct data members instead of OpenGL's stupid attribute stuff. And, while GLSL treats data passed from one shader to the next as global syntax, HLSL actually treats them as input parameters and output return values to a function, which is... it's just so much better. I mean, come on! It isn't even that big of a difference, but it is just so...

<img title="" src="./media/feels-good.png" alt="" width="128">

I think when I get around to writing a C framework around OpenGL, I am going to try to use HLSL, and compile it to Spir-V so that I can use it with OpenGL.

**Date: Wednesday, Feb 19, 2025** \
*Subject: Dr. Dave suck* \
So design review 2 came around for the Turbo Regatta. I created a beautiful differential op-amp that is regulated with a zener diode, along with a wonderfully constructed circuit diagram. That itself had to be reviews by one of the professors, but ultimately they approved of it. However, one professor, the school's head of the Engineering, Dr Dave, expressed doubt about whether or not a single Arduino Nano could handle all of the peripherals I was attaching to it just two weeks before. Particularly the pwm signals and the 2000 RPM externally triggered interrupts. So this week, I came prepaired. First of all, the pwm servos are handled by hardware, so they honestly aren't actually a problem at all. As for the interrupts, I dissassembled the count interrupt, counted all of the clock cycles, added on the clock cycles for the interrupt overhead, and came up with the exact number of clock cycles per second the interrupts would be taking per second, which ends up being around 0.02% of the processing time on the arduino. But of course, Dr. Dave had the audacity to still dispute my claims? 

<img title="" src="./media/crying-cat.jpg" alt="" width="128">

Like, what the heck? 2000RPM is literally just 33Hz! Even for a 16MHz processor, with each interrupt taking exactly 58 clock cycles, that is childs play! I guess non-emirical analysis was not enough to prove something that, quite honestly, can be figured out intuitively. It is embarrassingly obvious that the adruino can handle this stuff. Well, I guess it is time to actually aquire experimental evidence so that I can refute this dumb criticism.

**Date: Thursday, Feb 27, 2025** \
*Subject: Arduino Sucks* \
I got the experimental data in. And my goodness, it is almost exact. The experimental evidence almost perfectly predicts exactly how many clock cycles the increment counter handler takes each interrupt. And I am willing to bet that the discrepency is due to Arduino's own millisecond interrupt counter, which honestly probably takes up more processing power than all of my peripherals combined.
Anyway, my math places the interrupt to take 58 clock cycles, and the experiment predicts the interrupt to take 61 clock cycles. A difference of only 3 cycles. Pretty impressive if I do say so myself. Furthermore, I was only able to overwhelm Arduino's microprocessor at a combined interrupt rate of 260 kHz, which is also perfectly predicted by the curve created by the experimental data. Honestly, I don't think I've seen more accurate and precice experimental data than I've seen here. I don't think Dr. Dave can actually dispute it this time. And if he does, then honestly I am just going to be really upset.
Honestly this whole ordeal has been a massive waste of my time just to prove to a doctor of engineering, that doesn't understand how arduinos work, the increasingly obvious fact that the load I am placing on this arduino is embarrassingly small. Like, the millisecond interrupt counter, the one that the arduino library inserts into every program that uses it, likely takes up more processing power than the rest of my peripherals combined! Like, good lord professor, just take a hint! In my circuit, a friggin' differential amplifier with a diode is all that stands between a 18V battery, and a fried Arduino Nano, and the load of the arduino's peripherals is what he is worried about?



### Potential Future topics:
 - Windows sucks
 - Linux sucks
 - Assembly sucks (not really. Assembly is actually cool)
 - C is cool. (I could probably segue this one when I start programming the microcontrollers for the turbo regatta)
