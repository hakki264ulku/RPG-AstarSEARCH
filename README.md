# :video_game:  RPG-A*SEARCH

# RPG With SDL2 & GO Language
* This project is developed to practice basic programming skills and have an understanding of game development.
* In the project, SDL2 library is used for the UI of the game.
* This game is built with go language by using the basic game development practices and A* Search for the sake of artificial intelligence for monsters to be able to find and follow the player.
* You can play the game by running the executable file: rpg.exe


# 🚀 Tech Stack
* GO Language
* SDL2 Library

# 💿 Requirements for Running on local

* First you need to install GO lang to your local machine
* Then, it's needed to follow the below instructions for installing the SDL2 bindings for go

* [SDL2](http://libsdl.org/download-2.0.php)
* [SDL2_image](http://www.libsdl.org/projects/SDL_image/)
* [SDL2_mixer](http://www.libsdl.org/projects/SDL_mixer/)
* [SDL2_ttf](http://www.libsdl.org/projects/SDL_ttf/)
* [SDL2_gfx](http://www.ferzkopp.net/wordpress/2016/01/02/sdl_gfx-sdl2_gfx/)

Below is some commands that can be used to install the required packages in
some Linux distributions. Some older versions of the distributions such as
Ubuntu 13.10 may also be used but it may miss an optional package such as
_libsdl2-ttf-dev_ on Ubuntu 13.10's case which is available in Ubuntu 14.04.

On __Ubuntu 14.04 and above__, type:\
`apt install libsdl2{,-image,-mixer,-ttf,-gfx}-dev`

On __Fedora 25 and above__, type:\
`yum install SDL2{,_image,_mixer,_ttf,_gfx}-devel`

On __Arch Linux__, type:\
`pacman -S sdl2{,_image,_mixer,_ttf,_gfx}`

On __Gentoo__, type:\
`emerge -av libsdl2 sdl2-{image,mixer,ttf,gfx}`

On __macOS__, install SDL2 via [Homebrew](http://brew.sh) like so:\
`brew install sdl2{,_image,_mixer,_ttf,_gfx} pkg-config`

On __Windows__,
1. Install mingw-w64 from [Mingw-builds](http://mingw-w64.org/doku.php/download/mingw-builds)
    * Version: latest (at time of writing 6.3.0)
    * Architecture: x86_64
    * Threads: win32
    * Exception: seh
    * Build revision: 1
    * Destination Folder: Select a folder that your Windows user owns
2. Install SDL2 http://libsdl.org/download-2.0.php
    * Extract the SDL2 folder from the archive using a tool like [7zip](http://7-zip.org)
    * Inside the folder, copy the `i686-w64-mingw32` and/or `x86_64-w64-mingw32` depending on the architecture you chose into your mingw-w64 folder e.g. `C:\Program Files\mingw-w64\x86_64-6.3.0-win32-seh-rt_v5-rev1\mingw64`
3. Setup Path environment variable
    * Put your mingw-w64 binaries location into your system Path environment variable. e.g. `C:\Program Files\mingw-w64\x86_64-6.3.0-win32-seh-rt_v5-rev1\mingw64\bin` and `C:\Program Files\mingw-w64\x86_64-6.3.0-win32-seh-rt_v5-rev1\mingw64\x86_64-w64-mingw32\bin`
4. Open up a terminal such as `Git Bash` and run `go get -v github.com/veandco/go-sdl2/sdl`.
5. Then you can repeat __Step 2__ for [SDL_image](https://www.libsdl.org/projects/SDL_image), [SDL_mixer](https://www.libsdl.org/projects/SDL_mixer), [SDL_ttf](https://www.libsdl.org/projects/SDL_ttf)
    * NOTE: pre-build the libraries for faster compilation by running `go install github.com/veandco/go-sdl2/{sdl,img,mix,ttf}`

* Or you can install SDL2 via [Msys2](https://msys2.github.io) like so:
`pacman -S mingw-w64-x86_64-gcc mingw-w64-x86_64-SDL2{,_image,_mixer,_ttf,_gfx}`

To get the bindings, type:\
```
`go get -v github.com/veandco/go-sdl2/sdl`\
`go get -v github.com/veandco/go-sdl2/img`\
`go get -v github.com/veandco/go-sdl2/mix`\
`go get -v github.com/veandco/go-sdl2/ttf`\
`go get -v github.com/veandco/go-sdl2/gfx`

or type this if you use Bash terminal:\
`go get -v github.com/veandco/go-sdl2/{sdl,img,mix,ttf}`
```
* Finally, import repository into your local, navigate to your local directory and simply type:\
`go run main.go`


# 📝 License
This project is made available under the MIT License.
