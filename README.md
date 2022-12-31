# A Very Opinionated List of Security Tools

Because I go on camera and inadvertently create the impression that I know what I'm doing, I often get asked what the "best" tool for a given situation is. This question often comes from a place of wanting to invest time in learning a new tool, and folks want to make sure they're making a wise decision with their time.

Unfortunately, there is no "best" tool. There are only tools that work for you and don't. Everything else is just silly tribalism. People can get very loyal to brands, to operating systems, to...text editors. None of that is about technical advantages/disadvantages; it's entirely about being part of an in-group. Resist the urge to loyalty to tools. Get your work done with what works for you.

With that warning out of the way, I felt it was appropriate to put together a list of what works for _me_. That's all this is. I make no claims about any of these selections being better than others, much less "the best." They're the set of things I've cobbled together over years of experience and that I've become comfortable using. You may love them. You may not. Either way, I hope this list proves a valuable starting point for creating your own set of preferred security tools.

## Table of Contents

- [A Very Opinionated List of Security Tools](#a-very-opinionated-list-of-security-tools)
  - [Table of Contents](#table-of-contents)
  - [How to Read This List](#how-to-read-this-list)
  - [How NOT to Read This List](#how-not-to-read-this-list)
  - [My Biases](#my-biases)
  - [The Lazy Version](#the-lazy-version)
  - [Base System](#base-system)
    - [Operating System: KDE Neon](#operating-system-kde-neon)
      - [Why I Like It](#why-i-like-it)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with)
      - [Tips to Make It Great](#tips-to-make-it-great)
    - [Web Browser: Vivaldi](#web-browser-vivaldi)
      - [Why I Like It](#why-i-like-it-1)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-1)
      - [Tips to Make It Great](#tips-to-make-it-great-1)
    - [Terminal Emulator (Linux): Terminator](#terminal-emulator-linux-terminator)
      - [Why I Like It](#why-i-like-it-2)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-2)
      - [Tips to Make It Great](#tips-to-make-it-great-2)
    - [Terminal Emulator (Windows): Windows Terminal](#terminal-emulator-windows-windows-terminal)
      - [Why I Like It](#why-i-like-it-3)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-3)
      - [Tips to Make It Great](#tips-to-make-it-great-3)
    - [Shell: Fish](#shell-fish)
      - [Why I Like It](#why-i-like-it-4)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-4)
      - [Tips to Make It Great](#tips-to-make-it-great-4)
    - [Password Manager: BitWarden](#password-manager-bitwarden)
      - [Why I Like It](#why-i-like-it-5)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-5)
      - [Tips to Make It Great](#tips-to-make-it-great-5)
  - [Cross-Functional Tools](#cross-functional-tools)
    - [Text Editor: Vim](#text-editor-vim)
      - [Why I Like It](#why-i-like-it-6)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-6)
      - [Tips to Make It Great](#tips-to-make-it-great-6)
    - [Text Editor for Programming: Visual Studio Code](#text-editor-for-programming-visual-studio-code)
      - [Why I Like It](#why-i-like-it-7)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-7)
      - [Tips to Make It Great](#tips-to-make-it-great-7)
    - [Notes: Joplin](#notes-joplin)
      - [Why I Like It](#why-i-like-it-8)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-8)
      - [Tips to Make It Great](#tips-to-make-it-great-8)
    - [Screenshots: Flameshot](#screenshots-flameshot)
      - [Why I Like It](#why-i-like-it-9)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-9)
      - [Tips to Make It Great](#tips-to-make-it-great-9)
    - [Terminal Multiplexer: TMux](#terminal-multiplexer-tmux)
      - [Why I Like It](#why-i-like-it-10)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-10)
      - [Tips to Make It Great](#tips-to-make-it-great-10)
  - [WebApp Pentesting](#webapp-pentesting)
    - [HTTP Proxy: ZAProxy](#http-proxy-zaproxy)
      - [Why I Like It](#why-i-like-it-11)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-11)
      - [Tips to Make It Great](#tips-to-make-it-great-11)
    - [Directory Brute Forcer: Feroxbuster](#directory-brute-forcer-feroxbuster)
      - [Why I Like It](#why-i-like-it-12)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-12)
      - [Tips for Making It Great](#tips-for-making-it-great)
    - [API Testing: Insomnia](#api-testing-insomnia)
      - [Why I Like It](#why-i-like-it-13)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-13)
      - [Tips for Making It Great](#tips-for-making-it-great-1)
    - [cURL Alternative: HTTPX](#curl-alternative-httpx)
      - [Why I Like It](#why-i-like-it-14)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-14)
      - [Tips to Make It Great](#tips-to-make-it-great-12)
  - [Threat Hunting/DFIR](#threat-huntingdfir)
    - [IoC Management: Sigma](#ioc-management-sigma)
      - [Why I Like It](#why-i-like-it-15)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-15)
      - [Tips to Make It Great](#tips-to-make-it-great-13)
    - [Incident Response Triage: Trellix Redline](#incident-response-triage-trellix-redline)
      - [Why I Like It](#why-i-like-it-16)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-16)
      - [Tips to Make It Great](#tips-to-make-it-great-14)
    - [Deep Analysis: Jupyter](#deep-analysis-jupyter)
      - [Why I Like It](#why-i-like-it-17)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-17)
      - [Tips to Make It Great](#tips-to-make-it-great-15)
  - [Malware Analysis/Debugging](#malware-analysisdebugging)
    - [Disassembler: Cutter](#disassembler-cutter)
      - [Why I Like It](#why-i-like-it-18)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-18)
      - [Tips to Make It Great](#tips-to-make-it-great-16)
    - [Debugger: Rizin](#debugger-rizin)
      - [Why I Like It](#why-i-like-it-19)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-19)
      - [Tips to Make It Great](#tips-to-make-it-great-17)
    - [Malware Disposition: PEStudio](#malware-disposition-pestudio)
      - [Why I Like It](#why-i-like-it-20)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-20)
      - [Tips to Make It Great](#tips-to-make-it-great-18)
    - [First Look: PE-bear](#first-look-pe-bear)
      - [Why I Like It](#why-i-like-it-21)
      - [Stuff You Gotta Deal With](#stuff-you-gotta-deal-with-21)
      - [Tips to Make It Great](#tips-to-make-it-great-19)

## How to Read This List

This is a list of tools I use across multiple job descriptions: web app pentesting, threat hunting, malware analysis, and more.

Each item in this list will have a link, an explanation of why I like it, some things I put up with while using it, and recommendations to configure it for best usability. Use these details as a _starting point_ for your toolset, not a prescription. My methods and preferences will almost certainly not be yours, and that's okay! Even if you discover that you don't like these tools, this list has done its job by pointing you in a direction.

Of course, some of you hate reading, so I've provided the quick list of the tools detailed here for the impatient.

## How NOT to Read This List

This is in no way an invitation to debate. If you think I'm wrong, that's fine. If you want to convince me you're right, let me stop you right there. I have no interest in debates about what tools are better. These tools work for me. If I find compelling evidence why I _shouldn't_ use them, like if a CEO is weirdly into cryptocurrency, I'll change it up. I'm happy you have your preferences. These are mine. They don't have to be the same.

## My Biases

I want to be clear about some of my biases when choosing tools right up front. Take these with you as you evaluate this list.

1. Whenever possible, I choose the open source option. Yes, I mean open source.
2. I prefer cross-platforms tools for when I need to work on other OSes.
3. I care about the ethics of the developers (and will make changes when I learn something new).
4. I will choose interoperability over aesthetics.

## The Lazy Version

**Base System**

* Operating System: [KDE Neon](https://neon.kde.org)
* Web Browser: [Vivaldi](https://vivaldi.net)
* Terminal (Linux): [Terminator](https://gnome-terminator.org)
* Terminal (Windows): [Windows Terminal](https://github.com/microsoft/terminal)
* Shell: [Fish](https://fishshell.com)
* Password Manager: [Bitwarden](https://bitwarden.com)

**Cross-Functional Tools**

* Text Editor: [Vim](https://vimawesome.com/)
* Text Editor (alternate): [VSCode](https://code.visualstudio.com)
* Notes: [Joplin](https://joplinapp.org)
* Screenshots: [Flameshot](https://flameshot.org)
* Terminal Multiplexer: [Tmux](https://github.com/tmux-plugins/tpm)

**WebApp Testing**

* HTTP Proxy: [ZAProxy](https://zaproxy.org)
* Directory Fuzzer: [Feroxbuster](https://github.com/epi052/feroxbuster)
* API Testing: [Insomnia](https://insomnia.rest)
* Better cURL: [HTTPX](https://www.python-httpx.org)

**Threat Hunting/DFIR**

* IoC Management: [Sigma](https://github.com/SigmaHQ/sigma)
* Incident Response: [Mandiant Redline](https://fireeye.market/apps/211364)
* Deep Analysis: [Jupyter Lab](https://jupyter.org)

**Malware Analysis/Debugging**

* Disassembler: [Cutter](https://cutter.re)
* Debugger: [Rizin](https://rizin.re)
* Malware Disposition: [PEStudio](https://pestudio.en.lo4d.com/windows)
* First look: [PE-bear](https://github.com/hasherezade/pe-bear-releases)

## Base System

### Operating System: [KDE Neon](https://neon.kde.org)

This Linux distribution is based on Ubuntu LTS, but uses the latest packages from KDE to get you the latest and greatest features of the Plasma Desktop.

#### Why I Like It

I've used so many Linux distributions over the years I've lost count. Yes—including Arch, both from scratch and prepackaged with the lovely (and now discontinued) Antergos. But the season of distrohopping or spending all my time and energy futzing with my OS has passed for me. I need my stuff to work with a minimum of configuration. That said, I _do_ have some configuration I want easily available in my desktop environment. That's why the Plasma desktop is my preferred Linux DE. And for some time now, its resource usage has outperformed GNOME. It's not as lightweight as the tiling windows managers or XFCE, but it's light enough, with an attractive out-of-the-box appearance that enables you to get working quickly.

#### Stuff You Gotta Deal With

The package manager in KDE Neon is weird! For some reason they hate when you use `apt upgrade`. Instead they have their own `pkcon` tool for upgrading packages. It's fine, but I'd prefer they not mess with the standard tool.

#### Tips to Make It Great

Configuring your virtual desktops, keyboard shortcuts, etc. can make Plasma a joy to work with. I strongly recommend taking some time to configure these to your preferences. 

Get comfy with snaps! Snaps (and Flatpak) are supported by the Discover software store, and allow easy installation of many common apps.

### Web Browser: [Vivaldi](https://vivaldi.net)

Until recently, I was a steadfast Brave user. Then I learned some grodier stuff about how Brave's business model works, and the behavior of their CEO. Vivaldi fills my need for a privacy-respecting Chromium-based browser with a few extra features I really need and don't exist in plain ol' Chromium.

#### Why I Like It

Vivaldi is Chromium-based, which means my must-have browser extensions all work fine with it. It also has the DevTools I prefer. I'm sorry Firefox, as much as I want you to be amazing, there are parts of my computing life that require some Goog-only tools (like casting).  And before someone tells me how I _can_ accomplish all this with Firefox: I know. I've tried. It's hacky and unreliable and I decided against it.

Vivaldi is fun! It feels like old-school Opera, with unexpected bells and whistles. Some fun stuff I didn't expect:

* Tiled tabs
* A neat little sidebar for apps like Mastodon or Wikipedia
* Add effects to pages like invert colors or sepia tone

Vivaldi also has cloud-synced profiles for extensions settings, and other data. This is essential for me, as I use these profiles to sync my pentesting setup from machine to machine. 

Now you might have privacy concerns about this, which is fair. But good news: the entire profile is end-to-end encrypted with a master key of your choosing.

#### Stuff You Gotta Deal With

Some of Vivaldi's behaviors are weird, like how it handles tab movements from window to window. That just goes against muscle memory, but it's mostly fine. Same goes with how tab opening works, or the fact that you need to specifically configure it to always prefer HTTPS in the settings. 

The one actually annoying thing I've found concerns dark mode. On Linux, Vivaldi does not honor system color schemes. Yes, you can add a dark theme to Vivaldi, but websites like GitHub and Microsoft Learn which are using OS-level settings for color scheme will default to light, as will any error pages. There is a Chrome flag you can set that will enable dark mode on _everything_, but that can add its own complications. I haven't found a good solution for this; I'm mainly hoping Vivaldi sorts it out in an upcoming version.

#### Tips to Make It Great

Make. Your. Own. Theme. Vivaldi has a built-in theme editor that is simple to use, and very fun! 

Also definitely take the time to create a profile and sync it for easy movement of configs from machine to machine.

### Terminal Emulator (Linux): [Terminator](https://gnome-terminator.org)

You need a terminal emulator. The built-in one in KDE (Konsole) is just fine. But Terminator has a lot of out-of-the-box features I enjoy, and enough functionality that you don't *have* to resort to a terminal multiplexer if you don't want to. That plus easy configuration for color and font themes win me over.

#### Why I Like It

Some of my favorite features:

* Easy splitting of windows
* Broadcast mode to send the same commands to multiple panes
* Easy profiles/theme configuration
* Tabs _and_ tiling

#### Stuff You Gotta Deal With

Don't forget to make `terminator` your command for `Ctrl+Alt+T` or whatever your favorite shortcut is!

#### Tips to Make It Great

Take some time to make a custom profile and save it somewhere you can move it between machines. That config lives at `~/.config/terminator/config`.

### Terminal Emulator (Windows): [Windows Terminal](https://github.com/microsoft/terminal)

Hardly a unique choice, but I think it's important to call out how good this piece of software really is. It makes using multiple shells (PowerShell, cmd, WSL) in combination on Windows quite pleasant. And with some hidden superpowers, it's maybe my favorite first-party tool from Redmond.

#### Why I Like It

Ever used PowerShell? Ever get tired of the blue window? How about the constant separate windows? Windows Terminal solves this with tabs, panes (yes, really), and handling multiple profiles for firing up shells of all kinds. It even integrates with your WSL installs (which you should absolutely be using) to put all your terminal needs in one place.

#### Stuff You Gotta Deal With

I think a fix for this is on the way, but for now opening Admin shells is still a bit odd for Windows Terminal.

#### Tips to Make It Great

Find a theme! Use it! Then customize your PowerShell experience following [these steps](https://dev.to/ansonh/customize-beautify-your-windows-terminal-2022-edition-541l).

### Shell: [Fish](https://fishshell.com)

Bash is Fine. Zsh is fine. But I'm a Terminal dork, and I wanted something a little more feature-filled. I happened upon Fish years ago, and have been satisfied with it ever since.

#### Why I Like It

```shell
#!/usr/bin/fish

# Resize images in a directory

cd images
for i in (ls *.png)
  convert -resize 50% resized-$i
end
```

How is that for some clean syntax? Maybe it's not POSIX-compliant, but honestly that never really gets in my way. Instead, I have a much cleaner scripting language. 

What's more, Fish has top-rate command completion and history, better even than zsh. It is just a much more comfortable shell to use every day.

#### Stuff You Gotta Deal With

Sometimes, certain programs that expect a POSIX-compliant shell will have issues in Fish. You can drop to a bash or zsh session in those cases, or wrap the program invocation in `bash -c` if you really need to. It doesn't happen often, but it's worth knowing the workaround when it does.

#### Tips to Make It Great

Right away, install [Oh My Fish](https://github.com/oh-my-fish/oh-my-fish) to add extensions to fish, including themes and other capabilities.

I use OMF to install [bobthefish](https://github.com/oh-my-fish/theme-bobthefish), which provides Git symbology on the command line. To use it, you'll need Powerline enabled fonts, which you can get [here](https://github.com/powerline/fonts).

### Password Manager: [BitWarden](https://bitwarden.com)

#### Why I Like It

I was a LastPass customer for over a decade. Their recent mismanagement of their security incident convinced me they could no longer be trusted with my information. However, their failure is not an indictment of the concept of a password manager. While some feel that a local-only solution like KeePass is the only "secure" solution, I feel strongly that tools like a browser-integrated password manager are necessary as long as passwords are around to improve the overall strength and uniqueness of users' passwords.

So, Bitwarden. They've been around for some time, offering both a hosted and self-hosted version of an open source password management solutions. 

#### Stuff You Gotta Deal With

One thing I liked about LastPass was some of the custom data types they had out of the box, like bank accounts and SSH keys. Bitwarden lacks these, but can store the data nevertheless.

#### Tips to Make It Great

I'm still learning about Bitwarden, but I think my biggest recommendation for making it great is to use it. Like actually use it. Make it part of your everyday use of your browser. Use the mobile app. Tell your friends. Make weak passwords a thing of the past.

## Cross-Functional Tools

### Text Editor: [Vim](https://vimawesome.com/)

Use it or don't. It's not a religion and nobody's making you.

#### Why I Like It

Let's get this out of the way. Vim is hard to use. Anyone who says otherwise is being pretentious and trying to appear superior. It's not the kind of text editor anyone starts with. It requires practice to gain proficiency. Many commands are unintuitive, or intuitive for a different generation.

This is starting to read like why I don't like it. And yet, I love Vim. It took me a while to get comfortable with it, but after forcing myself to do so, Vim became kind of a superpower for a lot of use cases. Processing text files with Vim makes many processes faster or cleaner. It can be a hex editor. It can filter values. Oh, and of course the [regular expression](https://taggartinstitute.org/p/intro-to-regular-expressions) support.

#### Stuff You Gotta Deal With

Well, it's Vim. You have to learn it. I think it's worth the time investment for the powerful tool you gain access to.

#### Tips to Make It Great

Vim has a vast plugin ecosystem. [VimAwesome](https://vimawesome.com) is where you'll find them. There are multiple Vim plugin managers, but I've settled on [Vim-Plug](https://github.com/junegunn/vim-plug).

My `.vimrc` is pretty specialized, but you can certainly [see it](https://gist.github.com/mttaggart/b788e618eddca83a9c033572bfdf3c76) as a starting point.

### Text Editor for Programming: [Visual Studio Code](https://code.visualstudio.com)

I've used all the Electron-based text editors—all the way back to Adobe Brackets. Atom was cool, until it wasn't. Sublime Text is its own thing, and so is Notepad++. Kate on KDE is pretty neat as well, but for a single solution across platforms and languages, Visual Studio Code can't be beat.

#### Why I Like It

Extensions. That's why. The extension ecosystem gives VSCode the benefits of an IDE without the bloat of an IDE. 

I write Rust, I get the benefits of `rust-analyzer`. I write Hashicorp stuff, I have HCL syntax support. 

Heck, I can even load Jupyter Notebooks if I want. I can even open the editor directly from Windows Subsystem for Linux and interact with my projects on that filesystem.

#### Stuff You Gotta Deal With

Memory bloat, I guess? I've honestly never had a real issue with VSCode. It's a very solid bit of kit.

#### Tips to Make It Great

Extensions make the difference. But one super important setting that isn't an extension is bracket pair colorization. This makes brackets and parentheses pairs use separate colors to make them easier to visually match. Not sure why this isn't a default, but it's suuuuper handy.

### Notes: [Joplin](https://joplinapp.org)

You might think it's weird for someone who wrote a [whole dang C2 framework](https://github.com/mttaggart/OffensiveNotion) for a different notes app to be recommending this one. I promise there are good reasons.

#### Why I Like It

I'm a text guy. Not everyone is. I know some folks take notes primarily by diagram. Me? I'm too hyperverbal for that. I like lists. I like paragraphs. I like headings. Put simply, I like Markdown, and anything that gets in the way of me writing Markdown for my notes is not a value-add. That's why Notion, as nifty as it is for several use cases, is not my preference for note-taking.

So why Notion? Why not another Markdown-based solution like [Obsidian](https://obsidian.md)?

Obsidian's fine, but it isn't open source. As I said up top, when comparing solutions, I try to choose the open one whenever possible. But that's not all. Joplin has a few features I require or vastly prefer.

At the top of that list is the built-in note encryption. By syncing encrypted notes with Joplin Cloud, I get the convenience of my notes everywhere with the security of end-to-end encryption. That makes Joplin suited even for red team engagements, as described in [Responsible Red Teaming](https://taggartinstitute.org/p/responsible-red-teaming).

#### Stuff You Gotta Deal With

I dearly wish Joplin supported Google Drive. It doesn't, which is part of why I pay for Joplin Cloud. That and it's a nice way to give back to the project.

I also don't love that the notes are not stored as flat files, but I understand why. Be aware that you'll need to export your notes before using them directly with another app.

There are many, *many* plugins to choose from, so I encourage you to explore them. I'd also encourage you to keep the list to a minimum.

#### Tips to Make It Great

My list of must-have plugins is exceedingly short:

1. `plugin-bundle`: creature comforts like a table of contents and in-line todos.
2. `rich-markdown`: enables inline rendering of images.
3. `joplin-excalidraw`: enables inline editing of Excalidraw diagrams.

I also really do enjoy using Joplin Cloud for syncing. Easy to set up and a great way to support the project. Don't forget to enable encryption!

Lastly, Joplin has a [TUI app](https://joplinapp.org/terminal/)! It's installed with either `snap` or `npm` (I know, I know) and allows a fun terminal access to your notes. The fact that you can then edit your Joplin notes with Vim is *(chef's kiss)*.

### Screenshots: [Flameshot](https://flameshot.org)

Plasma Desktop has its own built-in screenshot tool which works well enough. As does Windows, of course. I lived and died by `Win+Shift+S` before I discovered Flameshot. Now, I use it basically exclusively for my screengrabbing needs.

#### Why I Like It

It's cross-platform, for one thing. With Flameshot, I can standardize my screenshotting process across any OS I'm working on. Easy access to annotation/redaction tools makes it an even bigger win.

#### Stuff You Gotta Deal With

The only, ONLY thing that's a tad frustrating with Flameshot is that on Linux, you'll need to manually bind a key sequence to the command `flameshot gui` for keyboard access. Clicking on the taskbar icon works too, but I'm a keyboard guy.

I have Meta+Shift+F mapped to `flameshot gui` on my Linux machines.

#### Tips to Make It Great

In addition to setting keyboard shortcuts, setting your font and color preferences can really personalize your screenshots. Other than that, this thing is pretty much perfect out-of-the-box. Install it everywhere.

### Terminal Multiplexer: [TMux](https://github.com/tmux-plugins/tpm)

If you're on a Linux system, you likely already have TMux installed, or it's readily available. TMux is another one of these tools that require some practice to use well, but I think it's quitel worth the time investment for the productivity wins.

#### Why I Like It

Even though the terminal emulator I prefer (see above) can split panes, TMux can do so both locally and on a remote system, and does so much more fluidly than Terminator does. Once the keyboard shortcuts are muscle memory, it's trivial to fire up new tabs and panes to move about the environment, set up ad-hoc dashboards, or monitor systems/output.

#### Stuff You Gotta Deal With

Like Vim, TMux takes practice. The good news is, there are a ton of resources to learn. TryHackMe even has a [room on TMux](https://tryhackme.com/room/rptmux)! I recommend going through it.

#### Tips to Make It Great

[TMux Plugin Manager](https://github.com/tmux-plugins/tpm) grants you access to some very useful extensions. My [tmux.conf](https://gist.github.com/mttaggart/e33b55646ddd49de9dcdb8afe8beaa7c) gives you some idea of what's possible, including saving sessions and making copy/paste easier.

## WebApp Pentesting

### HTTP Proxy: [ZAProxy](https://zaproxy.org)

No surprise here. I wrote an [entire course](https://academy.tcm-sec.com/courses/practical-web-application-security-and-testing?affcode=770707_ws5_bhdw) on how to use ZAP for professional webapp testing. But I actually do love it. The ZAP team have created a powerful open source tool for web app testing that competes favorably with commercial alternatives. I started using ZAP when Burp Pro was not available through my employer, and I got comfortable enough with it to actually *prefer* ZAP.

#### Why I Like It

This is going to bewilder some of you, but I find the ZAP user interface much easier to navigate than Burp's. I won't go so far as to call it intuitive—just too many knobs and levers for that—but I never get lost.

The Fuzzer in particular works extremely well, and getting comfortable with that aspect of the app will make your testing much more effective. The same is true for the authentication handling and context configurations, which allow you to specify what technologies you're attacking for a given context. Basically, I appreciate how configurable ZAP is for the specific test I'm doing.

And when I'm done, the reporting is invaluable. ZAP's built-in reports are not the only necessary artifact of a proper webapp test, but they provide important details such as specific parameters for a discovered vulnerability, as well as CWE listings to guide report recipients in remediation.

#### Stuff You Gotta Deal With

Like any Java application, ZAP could be more performant. Sometimes when handling large responses, ZAP freaks out and I've had to kill the window. Luckily sessions can be saved so recovery isn't too bad. I don't recommend running ZAP on anything less than 8GB of RAM.

ZAP will raise a ton of what I consider "junk" alerts by default. You'll want to configure some [Global Alert Filters](https://www.zaproxy.org/docs/desktop/addons/alert-filters/alertfilterdialog/) to adjust severity for your own situation.

#### Tips to Make It Great

ZAP's plugins really are something else. Here are a few I love:

* FuzzDB Lists
* Python Scripting
* Community Scripts
* Wappalyzer
* SAML
* JSON view

Python scripting is its own rabbit hole, but even the built-in Zest scripting can easily extend ZAP's abilities for you. Explore the script templates and community scripts to get a sense of what's possible.

I'd also recommend checking out the Automation features. These allow you to create scan templates and sets of tasks to be run for each new context. Takes a lot of the setup out of your testing process.

### Directory Brute Forcer: [Feroxbuster](https://github.com/epi052/feroxbuster)

There are tons of great options in this space. Dirbuster, GoBuster, and more. None of them have stayed slotted into my workflow like Feroxbuster. Sure, I'm inclined to like Ferox because it's written in Rust, but it's the featureset that keeps it on the lineup.

#### Why I Like It

Feroxbuster is fast. Like crazy fast. Sometimes *too* fast (see below). But it gets the job done, and does so with a host of configuration options that work perfectly for my methodology.

#### Stuff You Gotta Deal With

Feroxbuster can be so fast that it can bring down less resilient servers. It's important to use the command-line options to run it at the correct speed and concurrency rate for your target. I tend to use `-L 15 -t 15` for my default throttle, but that's 225 concurrent requests. If you need to slow it down, remember that your concurrent requests will be:

**connection limit** (`-L`) x **threads** (`-t`)

So 2 threads with a connection limit of 10 results in 20 concurrent requests.

It's really worth your time to read the [surprisingly extensive documentation](https://epi052.github.io/feroxbuster-docs/docs/).

#### Tips for Making It Great

As above, read the docs. But here are a couple of options I love:

* `--burp-replay`: Automatically sends any hits on your configured status codes (`-s`) to a proxy listening on port 8080.
* `--auto-bail` stops scanning directories with a ton of errors


### API Testing: [Insomnia](https://insomnia.rest)

ZAP is great when there's a browser-based interface to test. That isn't always the case. Sometimes you're testing an API directly. I used to use Postman for this, but in keeping with my attempt to use open source tools whenever possible, Insomnia has filled the niche quite nicely.

#### Why I Like It

Insomnia handles the gnarly parts of API testing fairly seamlessly, like OAuth token acquisition (assuming you have that information). It also makes adding additional headers simple. But perhaps the most important feature of Insomnia is that it does in fact accept Postman collection files as imports. This allows me to work with dev teams who use Postman as a matter of course. 

#### Stuff You Gotta Deal With

Honestly, I'm still getting used to how Insomnia handles certain things, like separate spaces for different projects. In Postman, these were "Collections." Insomnia uses folders. Still works fine, just a different workflow.

#### Tips for Making It Great

Insomnia also has an extensive [plugin ecosystem](https://insomnia.rest/plugins). I would check out some of the OAuth ones, and perhaps the cloud integrations, if that's your bailiwick. 

### cURL Alternative: [HTTPX](https://www.python-httpx.org)

This is not by any means required, but I bet you'll love it once you've tried it. `cURL` is great for quick testing of URLs, but it leaves a lot to be desired for the modern user. HTTPX picks up the slack, adding useful command line options to interact with URLs. Output is colorized as well.

#### Why I Like It

Imagine if `cURL` were written with webapp testing in mind. That's pretty much it. The command line options say it all.

#### Stuff You Gotta Deal With

It's Python, so the normal installation weirdness applies. I strongly recommend [pipx](https://pypi.org/project/pipx/).

#### Tips to Make It Great

Well, sometimes you'll get JSON output, so [jq](https://stedolan.github.io/jq/) should almost certainly be in the toolbelt.

## Threat Hunting/DFIR

### IoC Management: [Sigma](https://github.com/SigmaHQ/sigma)

This one might be a bit obvious, but I'm including it anyway. If you're not using Sigma to generate/save threat detection rules, you should. Sigma means you're not locked into one vendor's weirdo format, and can easily convert rules from one platform to another.

#### Why I Like It

In a word: `sigmac`. The Sigma Converter tool makes it simple to convert rules from a generic Sigma format to specific SIEM queries like Splunk, Azure, and more. It'll even export out to STIX for sharing. IoC Sharing is caring.

#### Stuff You Gotta Deal With

Not all the converted queries will work perfectly with your setup, depending on field/index names, so you may wish to create a custom conversion config.

#### Tips to Make It Great

What I just said.

### Incident Response Triage: [Trellix Redline](https://fireeye.market/apps/211364)

You've just gotten access to a compromised machine. You don't have your normal EDR. You don't have other logs. What are you going to do to get data quickly?

That's what Redline is designed for. Redline allows you to create customized collectors to gather exactly what data you want from an endpoint—including memory snapshots if you wish.

#### Why I Like It

Redline is essentially a self-contained version of Trellix's (née FireEye) endpoint protection software. It uses the same tools to gather evidence, and then displays the evidence in a table-based interface. The collection is simple enough, and the display, while basic, beats the pants off Event Viewer.

#### Stuff You Gotta Deal With

The timeframe management just straight-up sucks. You can't paste timestamps in any format, and it's a hassle to move back and forth between views because those time filters may or may not be saved. Also, Windows Event logs can be collected, but aren't always parsed correctly, so searching by column of data is hit-and-miss.

#### Tips to Make It Great

I got nothing. I wish Trellix would update this thing, or any of the other tools they offer. I'm not holding my breath.

### Deep Analysis: [Jupyter](https://jupyter.og)

Well this one comes as no surprise either. I [wrote](https://taggartinstitute.org/p/python-for-defenders-pt1) 2 [courses](https://taggartinstitute.org/p/python-for-defenders-pt2) on this subject. But really, I can't stress how often I fire up Jupyter notebooks to perform in-depth investigations on collected data. Once you have this capability, it's a superpower.

#### Why I Like It

I like Python. I like data science. I like Python for data science. But seriously, at the risk of repeating what I've written elsewhere, Jupyter allows the creation of reusable analysis tools that are self-documenting when written correctly.

#### Stuff You Gotta Deal With

Learning Python isn't exactly a simple prerequisite. There are other kernels besides Python, but none with the analytical toolset so ready to hand.

#### Tips to Make It Great

Use [Jupyter Widgets](https://ipywidgets.readthedocs.io/en/latest/). Seriously. And learn a data viz library, whether it's Plotly, Seaborn, Bokeh, or d3. Use it well to explain your data.

## Malware Analysis/Debugging

### Disassembler: [Cutter](https://cutter.re)

Sometimes, you gotta look at the bytes. Cutter makes this easy across platforms! And by integrating the Ghidra decompiler, you can even get C-like syntax for your review. 

#### Why I Like It

It's full-featured, easy to use, and gets right to the point of analyzing binaries. What sets it apart from some others is some extra love for exotic binaries. I haven't found anything that parses Rust or Go-compiled samples as well as Cutter.

#### Stuff You Gotta Deal With

It *claims* to have a debugger built-in, but I've never seen it work. I really want it to. If the debugger worked, that'd be basically the only tool I'd need for most analysis tasks.

#### Tips to Make It Great

Cutter is fine as-is, but if you use it in conjunction with its CLI debugger counterpart (see below), you're really cooking' with gas.

### Debugger: [Rizin](https://rizin.re)

All the cool features (and more!) of radare2 without grody developer behavior. Rizin is a fork of Radare, and this new dev team creates both Rizin and Cutter. I've been using both for some time and quite enjoy the experience—usually.

#### Why I Like It

It's not GDB. 

But seriously folks, I find the command structure much more intuitive for Rizin than the GNU debugger. 

The debugging process is quite distinct from GDB's, requiring the use of [rz-run](https://book.rizin.re/tools/rz-run/intro.html) scripts or one-liners to load input/arguments.

#### Stuff You Gotta Deal With

The command line syntax is unique, and takes some getting used to. I recommend going through the [Rizin Book](https://book.rizin.re/index.html) to learn the ins and outs.

Also, unfortunately the Python integration is not nearly as complete as it is for GDB. Scripted debugging is possible, but rather unwieldy. Which is why...

Visual mode is also...a lot. Again, it's about practice. But like a lot of other things on this list, the time invested in learning it is rewarded with remarkable capability.

#### Tips to Make It Great

...Rizin is best paired with an IPython3 REPL in a nearby terminal window. I like doing this with Tmux. IPython (installed with Jupyter) along with [pwntools](https://docs.pwntools.com/en/stable/) is the perfect companion to Rizin. It's a lot of terminal, but that's how I like to work. 

### Malware Disposition: [PEStudio](https://pestudio.en.lo4d.com/windows)

This is the first install I make on a malware analysis machine. When investigating a malware sample, I like to work smarter, not harder. My malware analysis is not academic; it's in service of incident response or threat hunting. I don't need to know how every single subroutine works. I do need to quickly disposition a sample for evilness. PEStudio does this by checking for suspicious imports, strings, and VirusTotal results.

#### Why I Like It

Does what it says on the tin. 

#### Stuff You Gotta Deal With

It can be a little slow, so plan to get a sandwich or do some other analysis while it runs.

#### Tips to Make It Great

None, really. Consider this a first step in analysis, not a complete picture.

### First Look: [PE-bear](https://github.com/hasherezade/pe-bear-releases)

When you're ready to go a little deeper, PE-bear is a nice middleground between full-on static analysis and the quick disposition provided by PEStudio. With this, you get a hex view, stats, imports, and other information about the executable. 

#### Why I Like It

It's lightweight, cross-platform, and informative at a glance. 

One killer feature is the comparison of 2 binaries side-by-side. 

#### Stuff You Gotta Deal With

Nothing frustrating I've found so far, as long as you're using the tool for its purpose.

#### Tips to Make It Great

None so far. It's pretty great as-is!




