---
title: "Alacritty on Windows!"
date: 2025-11-12
descritpion: "Let's try Alacritty on Windows!"
tags: [alacritty, windows, windows 11, terminal, computers, IT, programming]
---

When you're programming on Windows, there will be few of times that you'll need to open a command-line emulator! Microsoft has created a kind of terminal emulator[^terminalwindows] that is integrated to Windows. It's a good option, but if you use it for a while, you'll notice a few of things that are actually pretty glitched if you're coming from Linux. As an example, try to copy some text from Notepad++, then, try to paste it while using `ssh` connected to Linux, it's a hard duty. It's not integrated very well to a bunch of things, I mean, you can't even paste something easily, even using Windows Terminal. So Alacritty kicks in!

It's a pretty simple terminal emulator. Using PowerShell as default, it was faster than using Windows's native emulator... Maybe placebo! I need to benchmark it!

![Alacritty switched to CMD](/assets/alacritty_switched_to_cmd.png)

- [Alacritty home](https://alacritty.org/)
- [Alacritty requirements](https://github.com/alacritty/alacritty?tab=readme-ov-file#requirements)

It fixes most of problems I've ever had in CMD/PowerShell. You should try it out! You may be surprised if you use it!

[^terminalwindows]: [Console-host - AKA Command Prompt and/or Powershell](https://learn.microsoft.com/en-us/windows/console/definitions#console-host)