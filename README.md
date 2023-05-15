# Where's My Editor?
<p align="center">
 <img alt="Where's My Editor? logo" src="src/assets/images/WME_logo.png" width="50%" >
 <br>
 Logo created by rubice!
</p>
 Where's My Editor? is a level editor for the mobile game, Where's My Water? and all it's spinoffs.
 
 NOTE: If you came here to read a .waltex image, then go to [wmwpy](https://github.com/wmw-modding/wmwpy/blob/main/src/wmwpy/Utils/Waltex.py). `waltex.py` has moved there.

# Setup

run
```
pip install -r requirements.txt
```
or
```sh
py -m pip install -r requirements.txt
```

Now, since this is being developed at the same time as [wmwpy](https://github.com/wmw-modding/wmwpy), there will be features I use that are not in a full release yet. If you want to test it out, get wmwpy from github, or update it (this is in the `requirements.txt`)

```sh
pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
```

Once I make a full release, I will also make a wmwpy release, so this is only needed if you want to test the dev version.

---

Start by extracting your where's my water apk file into a directory. When you run the program for the first timze, it'll ask you to select the game directory. This can also be configurable in the `settings.json` file that is generated by the program.

# Build exe
## Install modules
To build an exe for wme, first install pyinstaller

```sh
pip install pyinstaller
```

Next install the `requirements.txt`

```sh
py -m pip install -r requirements.txt
```

Make sure `wmwpy` is installed from github (you shouldn't need to do this, as `wmwpy` is installed from github in the `requirements.txt`)

```sh
pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
```

## Build exe

```sh
py build.py
```

or

```sh
python build.py
```

The output is in `dis/wme.exe` (if you're not on windows, it probably won't be an exe).

# Todo

- [x] Export `xml` file
- [x] Export `png` file
- [x] Add and remove objects
- [ ] Room object. 
    - This has kind of been implemented, because wmw1 uses the image for the room placement, but the later games use an object (which can be loaded).
- [ ] Complete settings menu
- [ ] Level explorer
- [x] Fix some objects not loading
- [ ] Image editor

# Credits
- Thanks to [rubice!](https://youtube.com/@rubice2022) for creating the logo. I am not skilled enough to make something that looks that good.
- Thanks to [campbellsonic](https://github.com/campbellsonic) for the script to load `waltex` images. I could not have done it without them.
