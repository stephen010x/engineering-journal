## Engineering Journal
By Stephen Harris

**Date: Tuesday, Jan 7, 2025** \
*Subject: My new Engineering Journal sucks* \
I will be honest, at first I was sceptical about keeping an "engineering journal". Although I quickly realized that this would be an opportunity in disguise. For there are many things I am learning or plan to learn over the coming weeks, which I will discuss. But even better is that this provides with me the perfect opportunity to complain about my least favorite languages, or bash on the frustrating decisions of my engineering professors at the SET. I even have a few plans in mind for future topics in my engineering journal.

**Date: Thursday, 2025 Jan 9** \
*Subject: C++ sucks, but not as much as Javascript* \
Listen, we all know it. At least everybody who has learned any better language knows it. C++ is just not good. But it would at least be preferrable to Javascript, as I can at least pretend it is C.
You see, I am taking Bart's graphics class this semester. Javascript is already a language I am familiar with. But my lord I am quickly learning that some of the webapi's for javascript are just god awful. Especially in an untyped language such as JS. Especially WebGL. If only there was some way to make it typed...
Actually, that is exactly what I am planning to do.
Bart gave us a framework to base our assignments off of. And it makes these assignments stupid easy. How am I suppose to learn how to use webgl if bart already wrote it for me? Therefore, I have decided to rewrite his entire framework in C, and then compile it to webgl to be implemented into a web enviroment.
It has honestly been a great learning experience in learning the opengl api, and in compiling C to webasm. I already have most of the framework written. I just need to find or implement my own library for handling matrices so that I can set up the viewport matrices.

**Date: Tuesday, 2025 Jan 14** \
*Subject: The Turbo Regatta sucks* \
I am going to be honest, I am not excited for the upcoming design day's Turbo Regatta. They are really stretching the premise to try to include Computer Engineers in working on this project. What's worse is that this event is going to heavily cut into lab time for my Embedded Systems II class. *I'm sure it will be* so *worth it.* \
&#9; *sigh...* \
At least there seems to be prospects for me to learn how to design a PCB board. That I do look forward to.

**Date: Friday, 2025 Jan 17** \
*Subject: Webasm sucks* \
I have been spending the past two weeks trying to compile C to Webasm and Javascript. Even with tools such as Emscripten that provide an entire wrapper library for the C standard libs, it is still a nightmare to develop with.
For instance, what is to stop you from trying to allocate global memory for a struct with a flexible array member, but to accidentally allocate the space for the flexible array member in a completely different part of memory, thereby overwriting vital JS objects for the printf wrapper, thereby causing all subsequent calls to printf to fail dramatically?
Anyhow, through this process I have managed to learn things about emcc, javascript, webgl, and even C. And it *almost* works. I just need to get the viewport matrices right. I should probably just start with a simpler render model, and then branch out from there.
