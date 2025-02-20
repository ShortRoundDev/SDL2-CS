This is a fork of flibitijibibo's SDL2-CS. It bindgs the custom functions I wrote for SDL2.

# Original Readme, from the Original author:

This is SDL2#, a C# wrapper for SDL2.

Project Website: https://github.com/flibitijibibo/SDL2-CS

License
-------
SDL2 and SDL2# are released under the zlib license. See LICENSE for details.

About SDL2
----------
For more information about SDL2, visit the SDL wiki:

http://wiki.libsdl.org/moin.fcg/FrontPage

About the C# Wrapper
--------------------
The C# wrapper was written to be used for FNA's platform support. However, this
is written in a way that can be used for any general C# application.

The wrapper provides bindings for the following libraries:
- SDL2
- SDL2_image
- SDL2_mixer
- SDL2_ttf

Note that SDL2# will not provide every single SDL2 function. This is due to
limitations in the C# language that would cause major conflicts with the native
SDL2 library and its extensions.

SDL2# is a pure port of the C headers. The naming schemes for this library will
be exactly as they are done in the C library, with little-to-no concern for
"appropriate" C# style. The namespace indicates that this is SDL2, the class
names will indicate which library file the function/type/value exists in, and
everything else will be as close to the C version as technically possible.

About the Visual Studio Debugger
--------------------------------
When running C# applications under the Visual Studio debugger, native code that
names threads with the 0x406D1388 exception will silently exit. To prevent this
exception from being thrown by SDL, add this line before your SDL_Init call:

SDL.SDL_SetHint(SDL.SDL_HINT_WINDOWS_DISABLE_THREAD_NAMING, "1");

Roadmap
-------
To see the current roadmap for SDL2#, visit the GitHub issues page:

https://github.com/flibitijibibo/SDL2-CS/issues
