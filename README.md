UltraLoop is a converter from [Ultrastar][1]'s song format to [blitzloop][2]'s

It is built with bison and flex, so make sure you have those ;)

Compile with make and enjoy!

Note the conversion is inherently lossy, since Ultrastar has pitch information but blitzloop doesn't - also, most Ultrastar files use MP3 as their audio format, which is incompatible with blitzloop - but audio conversion is better handled by readily available tools ;)

Just make sure you check whether the "#OFFSET:" property in the ultrastar .txt is still correct - if it isn't, either change it in the ultrastar .TXT and run ultraloop again, or add the difference between the new and old offset to both the floats in the Timing block.

[1]: http://ultrastardx.sourceforge.net/
[2]: https://github.com/marcan/blitzloop
