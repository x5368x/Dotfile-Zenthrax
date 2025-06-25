# A complete BSPWM Window Manager Environment
<div align = center>

![bspwm-dotfiles](https://github.com/gh0stzk/dotfiles/assets/67278339/0340846a-74d4-4a43-9430-142b0832738d)




&ensp;[<kbd> <br> Install <br> </kbd>](#-installation)&ensp;
&ensp;[<kbd> <br> Features <br> </kbd>](#-features)&ensp;
&ensp;[<kbd> <br> Themes <br> </kbd>](#-the-themes)&ensp;
&ensp;[<kbd> <br> Keybindings <br> </kbd>](#very-useful-keybindigs-to-know)&ensp;
&ensp;[<kbd> <br> Wiki <br> </kbd>](https://github.com/gh0stzk/dotfiles/wiki)&ensp;
<br><br><br></div>



<br>

## 👻 Welcome

Welcome to my dotfiles. I’m gh0stzk from Mexico.

These dotfiles are designed with the goal of providing a bspwm environment that is lightweight, efficient, and functional, tailored for any use—whether it’s gaming, web browsing, or a productive work setting.

You’ll have 18 unique themes to choose from, each with its own style, colors, and navigation bar options. With this variety, you’re sure to find one that suits your preferences and needs.

## :book: Wiki
I already started writing the [**Wiki**](https://github.com/gh0stzk/dotfiles/wiki), you should give it a read. If it is your first time with a WM, you may be interested in reading [First steps after installing the dotfiles](https://github.com/gh0stzk/dotfiles/wiki/Firsts-steps-after-installing) or maybe read [frequently asked questions and answers](https://github.com/gh0stzk/dotfiles/wiki/Questions---Answers) [Keybinds](https://github.com/gh0stzk/dotfiles/wiki/Keyboard-Shortcuts) [Firefox Theme](https://github.com/gh0stzk/dotfiles/wiki/Firefox-Theme).

## 🚀 Features
<img src="https://user-images.githubusercontent.com/67278339/221605474-21d65156-0cf7-485c-bd1a-40792c37817e.png" alt="Linux Fetch" align="right" width="450">

#### Change themes on the fly

You can switch themes instantly, with no need to restart your session or environment. With just one click, the change is applied immediately.

#### Consistency Across the Environment

Each theme not only changes the appearance of bspwm but also instantly transforms the color scheme in terminals (Alacritty & Kitty), eww widgets, polybar bars, notifications, gtk theme, launchers and more. Visual harmony is guaranteed in every corner of your system.

#### Performance optimized

BSPWM is not a desktop environment (DE), and that’s exactly what makes it stand out in terms of lightweight performance. On my systems, my BSPWM-dotfiles environment starts with under **500 MB of RAM usage**. While these numbers don't tell the whole story, they do highlight the minimalist approach that a window manager should embrace.

It’s true that Wayland-based environments like Hyprland and Sway are modern and popular, but they come at a cost — for instance, Hyprland typically starts with nearly 1 GB of memory usage, which contradicts the idea of being truly lightweight.

Thanks to the latest major update to Picom, we now have stable and lightweight animations on X11. Additionally, I’ve optimized my setup to avoid unnecessary service reloads. Unlike distributions such as Archcraft or other dotfiles in the web —which restart bspwm, sxhkd, picom, dunst, and others whenever the theme changes— my environment keeps these services running without interruption.

It’s designed so that services/daemons which only need to be launched once do so correctly, and aren’t restarted every time a theme is switched. Changing the theme doesn’t require restarting bspwm, since it’s entirely possible to update its appearance using bspc without reloading the window manager.

In short, my setup is faster, smoother, and more stable than what’s provided by preconfigured distributions.

In addition, each theme can be configured independently — either by manually editing the theme’s configuration file or using my RiceEditor application. This ensures a high level of customization: if you want a minimalist setup for a specific theme, you can disable animations, shadows, rounded borders, or fading effects. On the other hand, if you prefer a more visually rich theme with all those features enabled, that’s fully supported as well. My dotfiles are built to provide that level of flexibility.

#### Multi-Monitor support

If you have multiple monitors, BSPWM will automatically detect and configure up to 4 displays when launching with my dotfiles.

If you connect an additional monitor while the session is already running, simply reload BSPWM using the `Super + Alt + r` key combination, and your monitors will be configured instantly.

You can check the Wiki [👉 Monitors Setup](https://github.com/gh0stzk/dotfiles/wiki/Monitors-setup) if you want to edit the default layouts.

#### RiceEditor

Is an application designed to simplify the customization of your current theme. It allows you to easily adjust various visual and configuration aspects, tailoring your environment to your preferences without the need to manually edit configuration files.

#### Eww Widgets

4 different widgets, including a calendar, music player, profile card and a cheatsheet. These widgets are not only functional but also instantly adapt to the color scheme of the selected theme.

#### Jgmenu

Explore an elegant right-click menu (Desktop) made with Jgmenu, which also syncs with themes for flawless visual consistency. 

#### LockScreen

The lockscreen automatically adapts to the active theme and offers two locking options: it can capture the current screen with a blur effect, or use a specific wallpaper depending on the current theme.

#### Wallpaper Engines

My dotfiles support **5 different methods** for setting your favorite wallpaper:

1. **Theme**: Sets a random wallpaper from the theme’s Walls directory. (Default)
2. **CustomDir**: Sets a random wallpaper from a directory you specify.
3. **CustomImage**: Sets a specific image as wallpaper.
4. **CustomAnimated**: Supports animated wallpapers (.mp4, .mkv, .gif).
5. **Slideshow**: Changes the wallpaper every 15 minutes with a random image from the theme’s Walls directory.

Each option is **theme-specific**, meaning you can have an animated wallpaper in one theme, a static image in another, or a custom directory in a third — And all your settings will be preserved per theme. By default, all themes load a random wallpaper from their Walls folder.

Check the wiki for more details: [👉 Wallpapers Configuration](https://github.com/gh0stzk/dotfiles/wiki/Wallpapers-Configuration)

#### Scratchpad

A _scratchpad_ is a tool designed to provide quick, temporary access to applications or notes without disrupting the desktop workflow. When activated, the scratchpad appears over the current workspace, allowing the user to access applications like a terminal, text editor, or any configured tool. Minimizing it hides the scratchpad from view but keeps it running in the background, ready to be reopened with a simple keyboard shortcut.

It's ideal for quick note-taking, running commands, or accessing auxiliary tools without losing focus on the current task.

#### Visual Composition and Animations

Each theme features a unique color palette, along with transparencies, shadows, and animations—all designed to maintain visual balance without impacting performance or overwhelming the environment.

#### Rofi Applets

Rofi applets to simplify your workflow:

- Wallpaper Selector - See the wiki [WallpaperSelector](https://github.com/gh0stzk/dotfiles/wiki/WallpaperSelector)
- Network Manager
- Bluetooth Controller
- Clipboard Manager
- Screenshot Tool
- Android MTP Manager
- Power Menu
- Keyboard Layout
- Terminal Selector (Alacritty or Kitty)
- Rofi app launcher style selector
- Tab app switcher

#### Tmux Configuration

Benefit from a newly added tmux configuration and design, enhancing your terminal multiplexing experience.

#### Neovim Setup

Simple yet powerful neovim configuration with the following features:

- Treesitter
- Lsp servers
- Completions [blink.nvim](https://github.com/Saghen/blink.nvim)
- Formatting [conform.nvim](https://github.com/stevearc/conform.nvim)
- Picker [Snacks-picker](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md)
- Explorer [Snacks-explorer](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md)
- Tab Line [barbar.nvim](https://github.com/romgrk/barbar.nvim)
- Statusline [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)
- Autopairs [mini-autopairs](https://github.com/echasnovski/mini.nvim/blob/main/readmes/mini-pairs.md)
- Hipatterns [mini-hipatterns](https://github.com/echasnovski/mini.nvim/blob/main/readmes/mini-hipatterns.md)
- Indent guides [Snacks-indent](https://github.com/folke/snacks.nvim/blob/main/docs/indent.md)
- Dashboard [Snacks-dashboard](https://github.com/folke/snacks.nvim/blob/main/docs/dashboard.md)
- WhichKey [which-key.nvim](https://github.com/folke/which-key.nvim)

#### Optimized ZSH Configuration

Optimized, native ZSH configuration. Not __Oh-My-Zsh__ or other bloated plugin managers. Some features:

- Fastest and optimized performance compinit function
- Autocompletion
- Syntax highlighting
- History substring search
- Fzf-tab completion with previews!!

---

### 🎨 Launchers

| :tshirt: Theme Selector |
|:-:|
|![Screenshot-11_12_2023-01-06-03](https://github.com/gh0stzk/dotfiles/assets/67278339/b11b5c58-b9ec-446b-8980-4f77bebb3432)|

| :traffic_light: Wallpaper Selector |
|:-:|
|![Shot-2024-11-08-134530](https://github.com/user-attachments/assets/dbac8c47-f12c-4242-97d6-38ad1193f76b)|

### 🎨 The themes

| Emilia |
|:-:|
|<img src="https://user-images.githubusercontent.com/67278339/280174054-8f56d12d-4efa-4024-99e1-4679591b45ca.gif" alt="Emilia Rice" align="center">|

| Jan |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/6e4959b7-6d07-42c6-8ede-2f3c16094ad2" alt="Jan Rice" align="center"> |

| Aline |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/5ae48d8d-ebcb-4fd5-9c80-78fc325a7a38" alt="Aline Rice" align="center"> |

| Andrea |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/1bfd302f-0e3f-4973-975b-56c78d6140ee" alt="Andrea Rice" align="center"> |

| Cynthia |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/5df45139-1d73-4f5f-8e8d-a417c86bfb96" alt="Cynthia Rice" align="center"> |

| Isabel |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/f2a0002f-3370-4361-9301-08abadcad600" alt="Isabel Rice" align="center"> |


| Silvia |
|:-:|
|<img src="https://github.com/gh0stzk/dotfiles/assets/67278339/616c2d93-fabf-41c2-9ab8-9c7b4d6a2e35" alt="Silvia Rice" align="center">|

| Melissa |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/a63e250d-c5d1-4360-afd7-cf64bf55a0fc" alt="Melissa Rice" align="center"> |

| Pamela |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/f9e85839-53c9-4e15-a800-8a2f7ca40691" alt="Pamela Rice" align="center"> |

| Cristina |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/e14c6777-25f6-4621-a88b-4fda71dbcc7f" alt="Cristina Rice" align="center"> |

| Karla |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/5455afdf-cc2f-4a8c-8fcd-526c59066d50" alt="Karla Rice" align="center"> |

| z0mbi3 |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/ff65caa8-6a15-4873-bf05-edf89ac0985d" alt="z0mbi3 Rice" align="center"> |

| Brenda |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/22e37944-5aad-46bf-8934-3a57d1718ed2" alt="Brenda Rice" align="center"> |

| Daniela |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/f296d6b4-9c8a-49ae-bf63-d82e5105f122" alt="Daniela Rice" align="center"> |

| Marisol |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/d11d20c5-1edc-44c8-901b-a4103a139617" alt="Daniela Rice" align="center"> |

| h4ck3r |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/2d55fcc6-1ea4-4d56-8c46-3a3fe10566fe" alt="Hacker Rice" align="center"> |

| Varinka |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/454d82b4-8f09-4768-bf51-6ce7818ad226" alt="Varinka Rice" align="center"> |

| Yael |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/cbb0a1cc-4e2d-46a2-a4f2-ee0be3d08b50" alt="Yael Rice" align="center"> |

---

### Rofi applets

| ![Shot-2024-11-09-131850](https://github.com/user-attachments/assets/05107f74-e137-41c0-9132-31d9c4fa0bb4) | ![Shot-2024-11-09-131918](https://github.com/user-attachments/assets/c5680b39-9aba-41e5-a781-7f23f7f8e336) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                                 Power Menu                                                 |                                                Screenshoter                                                |

| ![Shot-2024-11-09-132031](https://github.com/user-attachments/assets/0893b0b6-1211-43cb-9923-f4e42af70f4b) | ![Shot-2024-11-09-133244](https://github.com/user-attachments/assets/03546cb9-cf0d-42a2-b424-458c887e67c2) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Keyboard Layout                                               |                                               Android Mount                                                |

| ![Shot-2024-11-09-150142](https://github.com/user-attachments/assets/f7d1c404-c2e8-43c0-ad5e-6b052e3918c3) | ![Shot-2024-11-09-155335](https://github.com/user-attachments/assets/889d2ccf-beff-402d-8804-6d82c5638860) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Network Manager                                               |                                             Clipboard Manager                                              |

| ![Shot-2024-11-09-153419](https://github.com/user-attachments/assets/4af56dfa-f61f-4b45-8350-d064fe67663a) | ![Shot-2024-11-09-153444](https://github.com/user-attachments/assets/9a5d86e3-d58c-4b26-bb3e-86ec4974261a) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                             Bluetooth Manager                                              |                                              Terminal Manager                                              |

| ![Shot-2025-04-08-084756](https://github.com/user-attachments/assets/835366c8-88c5-4daf-8260-5c822e27abc8) | ![Shot-2025-04-08-084924](https://github.com/user-attachments/assets/c32f3cdb-7a5a-4372-b6f2-3f4a09f50868) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Tab app switcher                                              |                                              Rofi style selector                                           |

---

### Rofi app launcher styles
| ![Shot-2025-04-08-090012](https://github.com/user-attachments/assets/57ebcc98-73ea-4f76-bb2b-fe3f187be5e7) | ![Shot-2025-04-08-090041](https://github.com/user-attachments/assets/26361cd3-c3b4-48a2-a550-8df5cff120f5) | ![Shot-2025-04-08-090107](https://github.com/user-attachments/assets/16da6b0f-5a9e-4410-bb95-cb9fe696ce55) |
| :---: | :---: | :---: |
| Normal | Full | Minimal |

### Fzf tab terminal completions with previews!

| ![fzf tab](https://github.com/user-attachments/assets/2771e549-f7cc-44da-baf2-6c9fa299f0fb) |
| :---: |
| cd, ls, pacman, systemctl, kill, cat, commands with preview! |

### Eww widgets

| ![ProfilePane](https://github.com/user-attachments/assets/07827cff-63b9-40db-b0ef-8c214a5d8ec3) | ![Calendar](https://github.com/user-attachments/assets/5ffcff9e-0852-4d9f-83b5-4bce71e69f7c) | ![MusicPlayer](https://github.com/user-attachments/assets/b96c49a1-57d1-43e5-bff0-cab2e6b4d101) |
| :---: | :---: | :---: |
| Profile Panel | Calendar | Music Player |

| ![Shot-2024-11-10-000520](https://github.com/user-attachments/assets/a0871d4e-5b2b-4e64-ae79-617feec71cf1) |
| :--------------------------------------------------------------------------------------------------------: |
|                                                Cheat Sheet                                                 |

---

### Rice Editor

| ![Shot-2024-11-09-155549](https://github.com/user-attachments/assets/2ac910c8-171f-47eb-8210-1469b6f75cc2) |
| :--------------------------------------------------------------------------------------------------------: |
|                                                Rice Editor                                                 |

### Lockscreen

| ![Lockscreen](https://github.com/user-attachments/assets/2f09b915-f426-49c3-b9b6-07be4e781f5a) |
| :--------------------------------------------------------------------------------------------: |
|                                           Lockscreen                                           |

### Jgmenu

| ![Jgmenu](https://github.com/user-attachments/assets/82daebec-66a6-4716-8e78-b02fcec7e77c) |
| :----------------------------------------------------------------------------------------: |
|                                           Jgmenu                                           |

## Yazi config

https://github.com/user-attachments/assets/8e15cc1a-88b8-4a7e-a4de-e7da76021406

## Tmux theme

| ![ezgif com-animated-gif-maker](https://github.com/gh0stzk/dotfiles/assets/67278339/dd5f7261-0631-4a91-b584-51ca8859c197) |
| :-----------------------------------------------------------------------------------------------------------------------: |
|                                                        Tmux theme                                                         |

## Scratchpad

https://github.com/user-attachments/assets/79764678-c519-4a41-a333-2a862a6d10f8

## Environment

| ![Gtk-Ranger-Music](https://github.com/user-attachments/assets/a7f7c082-5ffd-4a6c-babf-7361764cec80) |
| :--------------------------------------------------------------------------------------------------: |
|            The environment changes with each theme. In the gif: (Ranger, Thunar, Ncmpcpp)            |

### Firefox theme

| Firefox theme - z0mbi3 Fox |
|:-:|
| <img src="https://github.com/gh0stzk/dotfiles/assets/67278339/9b956d3d-fc7b-49ca-b27f-dc6aa83d9e2f" alt="Firefox theme - z0mbi3-Fox" align="center"> |

### Neovim setup

| Neovim setup |
|:-:|
| ![Neovim setup](https://github.com/user-attachments/assets/a70a0ebb-9921-4d2d-88f3-5eabdc5d10f9) |
| Plugins included [Neovim setup wiki](https://github.com/gh0stzk/dotfiles/wiki/Neovim-setup) |

## Very useful keybindigs to know...

| Keys | Action |
| :-------------------: | :---------------------------------------------------------------: |
| `super` + `x` | Close Windows |
| `super` + `Enter`<br>`super` + `alt` + `Enter` | Open a terminal<br>Open a floating terminal. |
| `alt` + `@space` | Display menu to select a theme. |
| `super` + `@space` | Apps Menu. |
| `super` + `alt` + `w`| Opens a menu to select a wallpaper. |
| `super` + `alt` + `h`<br>`super` + `alt` + `u` | Hides bar/s<br>unhide bar/s |
| `super` + `alt` + `s` | Takes screenshot. |
| `ctrl` + `alt` + `[plus,minus,t]` | Changes transparency on focused window. |
| `ctrl` + `super` + `alt` + `p`<br>`ctrl` + `super` + `alt` + `r`<br>`ctrl` + `super` + `alt` + `k` | Power off computer<br>Restart computer<br>Brute kill a window/process |
| `super` + `alt` + `r` | Restart bspwm. |
| `alt` + `F1` | Show keybinds cheatsheet |

And more.. You need to look sxhkdrc file for more, or press Alt + F1 for a cheatsheet.

---

> [!CAUTION]
> ⚠️⚠️⚠️ My dotfiles are designed for a **1600x900** resolution with **96 DPI** on a single monitor.
> Some elements may appear different on higher or lower resolutions. You may need to make adjustments to adapt them to your preferences and setup. ⚠️⚠️⚠️

> [!important]
> ✏️✏️✏️ The installer assumes you already have a **functional** Arch Linux installation, whether it’s a fresh install or an existing setup.
>
> A login manager of your choice is required; **lightdm** is recommended.
>
> The rofi connection manager applet, works with **NetworkManager**
>
> If using a virtual machine, be sure to change the Picom backend from **glx** to **xrender** before rebooting, and verify that hardware acceleration is correctly configured in your VM. ✏️✏️✏️

> [!warning]
> :wrench::wrench::wrench: I have tested the installation and functionality of these dotfiles on both high- and low-end machines.
>
> Some adjustments may still be needed, such as changing the Picom backend or VSync settings to ensure compatibility with your graphics card.
>
> If you encounter any issues, feel free to open an [issue](https://github.com/gh0stzk/dotfiles/issues). :wrench::wrench::wrench:

---

### 💾 Installation:

> [!NOTE]
> The installer only works for **ARCH** Linux, and based distros. (Except NO-Systemd ditros like Artix)

Before running this command, check [RiceInstaller](https://raw.githubusercontent.com/gh0stzk/dotfiles/master/RiceInstaller) to make sure it's working and confirm it's safe for your system.

- Open a terminal and execute this commands one by one:

```sh
# Download the installer in your $HOME
curl -LO http://gh0stzk.github.io/dotfiles/RiceInstaller

# Give it execution permission
chmod +x RiceInstaller

# Run the installer
./RiceInstaller
```
