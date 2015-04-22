The source code for the binary space partitioner we used for DOOM is now available at ftp.uwp.edu: /incoming/id/doombsp.zip.

The catch is that the source has a few objective-c constructs in it, so it will take some work to port to dos.  The only thing that will be a hassle is replacing the collection objects, the majority is just straight C.

This code was written and extended, not evolved, so it probably isn't the cleanest thing in the world.  Please, PLEASE, PLEASE do not ask for support on this.  I have far too much occupying my time as it is.

Our map editor does NOT work on wad files.  It saves an ascii text representation of the file, then launches doombsp to process that into a wad file. I have included the input and output for E1M1, so you can verify any porting work you perform.

Having two programs allowed us to seperate the tasks well under NEXTSTEP, but people working on dos editors will probably want to integrate a version of the bsp code directly into the editor.

If you are creating new DOOM maps for other people to use, we would apreciate it if the wadfiles you create use a PWAD identifier at the start of the file instead of the normal IWAD.  This causes DOOM to tell the user that they are playing a modified version, and no technical support will be given.

If you are creating a map editor for distribution to other people, contact Jay WIlbur (jayw@idsoftware.com) about getting a license agreement for the use of our trademark, etc.  Its not a money issue, just some legal jazz.

BTW, there IS a bug in here that can cause up to a four pixel wide column to be drawn out of order, causing a more distant floor and ceiling plane to stream farther forward than it should.  You can sometimes see this on E1M1 looking towards the imp up on the ledge at the entrance to the zig zag room.  A few pixel wide column of slime streams down to the right of the walkway.  It takes a bit of fidgeting with the mouse to find the spot.  If someone out there tracks it down, let me know...

Have fun!

John Carmack
Id Software
