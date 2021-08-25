### 视频教程地址

https://www.bilibili.com/video/BV1gf4y117aU?from=search&seid=8372827042697178885


# chunkwm, yabai and skhd configs
My personal chunkwm, yabai and skhd configs


NOTE: yabai requires System Integrity Protection to be disabled to work properly. See [here](https://github.com/koekeishiya/yabai/wiki/Disabling-System-Integrity-Protection) for more information.

## Installing for chunkwm
```sh
# Remove previous links
$ rm -f "${HOME}"/.{chunkwm,skhd}rc

# Install configs
$ git clone https://github.com/itgoyo/yabai-config.git "${HOME}"/.config/chunkwm
$ ln -s "${HOME}/.config/chunkwm/chunkwm/chunkwmrc" "${HOME}/.chunkwmrc"
$ ln -s "${HOME}/.config/chunkwm/chunkwm/skhdrc" "${HOME}/.skhdrc"
```

## Installing for yabai
```sh
# Remove previous links
$ rm -f "${HOME}"/.{yabai,skhd}rc

# Install configs
$ git clone https://github.com/itgoyo/yabai-config.git "${HOME}"/.config/yabai
$ ln -s "${HOME}/.config/yabai/yabai/yabairc" "${HOME}/.yabairc"
$ ln -s "${HOME}/.config/yabai/yabai/skhdrc" "${HOME}/.skhdrc"
```

## Keyboard shortcuts
### Chunkwm / Yabai
#### Changing focus
<kbd>alt</kbd> + <kbd>hjkl</kbd>

### focus
| Action       | Key Combination                                  |
|--------------|--------------------------------------------------|
| focus west  | <kbd>alt</kbd> +  <kbd>h</kbd> |
| focus south | <kbd>alt</kbd> +  <kbd>j</kbd> |
| focus north | <kbd>alt</kbd> +  <kbd>k</kbd> |
| focus east  | <kbd>alt</kbd> +  <kbd>l</kbd> |


#### Resize windows

| Action       | Key Combination                                  |
|--------------|--------------------------------------------------|
| Resize left  | <kbd>shfit</kbd> + <kbd>cmd</kbd> + <kbd>h</kbd> |
| Resize down  | <kbd>shfit</kbd> + <kbd>cmd</kbd> + <kbd>j</kbd> |
| Resize up    | <kbd>shfit</kbd> + <kbd>cmd</kbd> + <kbd>k</kbd> |
| Resize right | <kbd>shfit</kbd> + <kbd>cmd</kbd> + <kbd>l</kbd> |
| Equalise     | <kbd>shfit</kbd> + <kbd>cmd</kbd> + <kbd>0</kbd> |

#### Move windows
<kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>hjkl</kbd>

#### Move windows to workspace

| Action                      | Key Combination                                    |
|-----------------------------|----------------------------------------------------|
| Send to last active desktop | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>m</kbd>   |
| Send to previous workplace  | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>p</kbd>   |
| Send to next workplace      | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>n</kbd>   |
| Send to workplace           | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>num</kbd> |

#### Rotate windows

| Action               | Key Combination                                  |
|----------------------|--------------------------------------------------|
| Rotate clockwise     | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>r</kbd> |
| Rotate anticlockwise | <kbd>alt</kbd> + <kbd>r</kbd>                    |
| Flip on x-axis       | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>x</kbd> |
| Flip on y-axis       | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>y</kbd> |

#### Window actions

| Action            | Key Combination                                  |
|-------------------|--------------------------------------------------|
| Fullscreen        | <kbd>alt</kbd>  + <kbd>f</kbd>                   |
| Native fullscreen | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>f</kbd> |
| Center window     | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>c</kbd> |

#### Insertion point

| Action                       | Key Combination                                                     |
|------------------------------|---------------------------------------------------------------------|
| Insert left                  | <kbd>shift</kbd> + <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>h</kbd> |
| Insert down                  | <kbd>shift</kbd> + <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>j</kbd> |
| Insert up                    | <kbd>shift</kbd> + <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>k</kbd> |
| Insert right                 | <kbd>shift</kbd> + <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>l</kbd> |
| Cancel insert (chunkwm only) | <kbd>shift</kbd> + <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>x</kbd> |

#### Misc

| Action          | Key Combination                                                     |
|-----------------|---------------------------------------------------------------------|
| Toggle float    | <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>space</kbd>                |
| Toggle gaps     | <kbd>lctrl</kbd> + <kbd>alt</kbd> + <kbd>g</kbd>                    |
| Restart chunkwm | <kbd>lctrl</kbd> + <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>r</kbd> |

### Non-chunkwm
#### Show information
##### Description
Uses `osascript` to show information like CPU, memory, battery, etc. The CPU script requires [osx-cpu-temp](https://github.com/lavoiesl/osx-cpu-temp) installed. The song script supports iTunes and cmus.

Click [here](scripts) to view the script folder

Note: May have to change the location of the scripts in skhdrc

##### Key Combination
<kbd>fn</kbd> + <kbd>lalt</kbd> + <kbd>num</kbd>

##### Screenshots
<img width="382" height="101" src="screenshots/cpu.png?raw=true"><img width="382" height="101" src="screenshots/mem.png?raw=true">
<img width="382" height="101" src="screenshots/bat.png?raw=true"><img width="382" height="101" src="screenshots/disk.png?raw=true">
<img width="382" height="101" src="screenshots/song.png?raw=true">

```
fn + lalt - 1 : /path/to/script
fn + lalt - 2 : /path/to/script
fn + lalt - 3 : /path/to/script
...
```

#### Opening applications
#### Launch iTerm2
##### Description
Launches iTerm2 using like in i3-wm.

Click [here](scripts/open_iterm2.sh) to view the script

##### Key Combination
<kbd>alt</kbd> + <kbd>return</kbd>

```
alt - return : /path/to/launch/terminal
```
