# 🎨 windhawk-wallpaper-adaptive-widgets

A collection of **Windhawk mods** and a **YASB config** for a desktop that changes with your wallpaper:

- 🎵 **Audio Visualizer + Lyrics** that remembers its position and layout **per wallpaper**
- 🕒 **Desktop Clock** that changes style and position per wallpaper
- 📊 **YASB status bar** config and theme
- 🖼️ Sample **wallpapers** and **cutouts** (for the 3D "behind the subject" effect)

---

## 📁 What's in this repo

| File / Folder | What it is |
|---|---|
| `Audio-visualizer-and-lyrics` | Windhawk mod: audio visualizer, lyrics, album widget, player |
| `Clock-s` | Windhawk mod: desktop clock |
| `YASB/` | My YASB config and styles |
| `wallpaper/` | Example wallpapers |
| `cutout/` | Example cutout PNGs |
| `electroharmonix.ttf` | Font for the clock's 4th (Tech) style |

---

## ⚠️ Step 1: Turn off the wallpaper change animation (important!)

The mods switch layouts when your wallpaper changes. Windows' fade animation can make this look glitchy, so turn it off first.

1. Press `Win + R` to open the Run dialog.
2. Type this and press Enter:

```
SystemPropertiesPerformance.exe
```

3. In **Performance Options**, under the **Visual Effects** tab, select **Custom**.
4. In the list, **uncheck** `Animate controls and elements inside windows`.
5. Click **Apply**, then **OK**.

---

## ⚠️ Step 2: Install Windhawk (required)

The mods **will not work** without it.

1. Download Windhawk from **https://windhawk.net**
2. Install it and open it.

---

## 🎵 Step 3: Audio Visualizer + Lyrics mod

### Install

1. Open **Windhawk** → **Create a new mod**.
2. Open the file `Audio-visualizer-and-lyrics` from this repo and **copy all of its code**.
3. In Windhawk, **select everything**, delete it, and **paste** the copied code.
4. Click **Compile Mod**, then make sure the mod is **Enabled**.

### Edit the layout for each wallpaper

1. Make sure the **Player** is enabled in the mod settings (**Player Menu → Show Player tray button**). A button appears in your system tray.
2. Set the wallpaper you want to customise.
3. Click the **Player** tray button → click the **⚙️ gear** → **Open desktop layout editor**.
4. Move the visualizer, lyrics and album widget where you like, change bars and colors, and optionally choose a **cutout PNG**.
5. Click **Apply**.

That layout is now saved for **that wallpaper only**. Change the wallpaper and repeat. 🎉

> To show lyrics, turn on **Lyrics → Enable lyrics widget** in the mod settings.

---

## 🕒 Step 4: Desktop Clock mod

### Install

1. Install the font first: right-click `electroharmonix.ttf` → **Install**. The **4th style (Tech)** is made for this font, so it looks right only with it.
2. In Windhawk → **Create a new mod**, paste the code from `Clock-s`, click **Compile Mod**, and make sure it is **Enabled**.

### Edit the clock for each wallpaper

1. Set the wallpaper you want to customise.
2. Press **`Ctrl + Alt + Shift + C`** to enter the layout editor.
3. Drag to move, drag the corners (or scroll) to resize, and press **`S`** to switch between the 7 styles. [Style 6 have 7 more style inside it so you have many styles].
4. Press **`Enter`** to save. **`Esc`** cancels.

The clock now remembers that position, size and style for **that wallpaper**. Repeat for your other wallpapers.

> The shortcut can be changed in the mod settings, and the editor shows all other keys on screen.

### 🔤 Use your own fonts

**Option A: Install the font normally**
1. Right-click a `.ttf` / `.otf` file → **Install**.
2. In the clock's Windhawk settings, type the font's name in that style's font setting.

**Option B: Without installing**
1. Put your font files in any folder, for example `C:\ClockFonts`.
2. In the clock's Windhawk settings, set **Custom fonts folder** to that folder.
3. Type the font name in the font settings.

In the editor, **Custom style (5th)** also lets you pick fonts with **`F`** or **`G`**.

---

## 📊 YASB (status bar) setup

1. Install **YASB** from https://github.com/amnweb/yasb and run it once.
2. Open `C:\Users\<YourName>\.config\yasb\`
3. Copy the files from the `YASB/` folder of this repo into it (back up your old ones first).
4. Restart YASB.

---

## 🙏 Credits

- Audio visualizer mod by **sarthakaksh**, forked from **NeiZ [NeiZqwe]** and contributors
- Lyrics from **[LRCLIB](https://lrclib.net)**
- Built on **[Windhawk](https://windhawk.net)** and **[YASB](https://github.com/amnweb/yasb)**

## 📄 License

MIT. See [LICENSE](LICENSE).
