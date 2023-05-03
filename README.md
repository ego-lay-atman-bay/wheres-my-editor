# Where's My Editor
 <img src="src/assets/images/WME_logo.png" >
 Logo created by rubice!
 
 Where's My Editor? is a level editor for the mobile game, Where's My Water? and all it's spinoffs.
 
 NOTE: If you came here to read a .waltex image, then go to [wmwpy](https://github.com/wmw-modding/wmwpy/blob/main/src/wmwpy/Utils/Waltex.py), because I will be removing Waltex.py from wme.

# Setup

run
```
pip install -r requirements.txt
```
or
```
py -m pip install -r requirements.txt
```

Now, since this is being developed at the same time as [wmwpy](https://github.com/wmw-modding/wmwpy),  will be features I use that are not in a full release yet. If you want to test it out, get wmwpy from github, or update it.

```
git clone https://github.com/wmw-modding/wmwpy
```

Then create a virtual environment (venv)
```
py -3.10 -m venv .venv
```
or
```
python -m venv .venv
```

Then create a symlink from the `src/wmwpy` folder in the wmwpy repository to `.venv/Lib/site-packages`

```batch
mklink /D wheres-my-editor/.venv/Lib/site-packages wmwpy/src/wmwpy
```

This is to make your python environment use the latest wmwpy dev version, and you'll be able to update both repositories at will.

Once I make a full release, I will also make a wmwpy release, so this is only needed if you want to test the dev version.

---

Start by extracting your where's my water apk file into a directory. When you run the program for the first timze, it'll ask you to select the game directory. This can also be configurable in the `settings.json` file that is generated by the program.

# Todo

- [x] Export `xml` file
- [x] Export `png` file
- [ ] Add and remove objects
- [ ] Room object
- [ ] Image editor
- [ ] Complete settings menu
- [ ] Level explorer
- [x] Fix some objects not loading

# Credits
- Thanks to [campbellsonic](https://github.com/campbellsonic) for the script to load `waltex` images. I could not have done it without them.
- Thanks to rubice! for creating the logo. I am not skilled enough to make something that looks that good.
