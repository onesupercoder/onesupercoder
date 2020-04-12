---
title: "My Idea for quickset"
date: 2020-04-11T02:02:58-06:00
description: "Quick and easy coder set up"
tags: [projects]
---


{{< highlight bash >}}
             .__        __                   __   
  ________ __|__| ____ |  | __  ______ _____/  |_ 
 / ____/  |  \  |/ ___\|  |/ / /  ___// __ \   __\
< <_|  |  |  /  \  \___|    <  \___ \\  ___/|  |  
 \__   |____/|__|\___  >__|_ \/____  >\___  >__|  
    |__|             \/     \/     \/     \/      
{{< / highlight >}}

I'm an updater.  I like to keep my system up to date.  I like to update the OS, my programming language and my dependencies.  I also love to try different programming languages.

What if you could update and set up your machine for a preferred programming language or even job role with just one simple command?

{{< highlight shell >}}
$ quickset rails
| Upgrading apt packages...
/ Installing zsh...
- Installing homebrew...
\ Installing rbenv & ruby-build...
| Installing postgresql...
/ Installing rails....
- Installing vs code + extensions...
{{< / highlight >}}

{{< highlight shell >}}
$ quickset web-designer
/ Installing vscode...
- Installing gimp...
\ Installing whatever web designers use...
* Done.
{{< / highlight >}}

My dream is to just run a command and setup my computer as a majority of developers would for that language and paradigm.  Maybe even one day having it switch roles or apps on and off.

### Amazing tools

There are so many amazing tools out there developers use:

1. Homebrew
2. Docker
3. Oh-my-zsh
4. Git
5. VS Code, Intellij, VIM
6. Postgres, sbt, java, rvm, python... stuff (and others depending on the language)
6. A bunch i'm probably missing cause i'm not that cool

And i usually just keep a mental note and or look for more and keep a list.  All the awesome-[language goes here] usually gives me ideas of projects. For example for react development: https://github.com/enaqx/awesome-react#react-development-tools  But not everyone knows the best and most up to date and how to find, use or install them.  (Okay i'm not helping with the use part.... yet...)

Even existing developers could use it to update libraries and packages all at once.

{{< highlight shell >}}
$ quickset
| Updating oh my zsh...
/ Upgrading apt packages...
- Updating homebrew....
\ Updating java...
| Updating sbt...
/ Checking for dependency updates in project...
* Done.
{{< / highlight >}}

Its definitely not for production environments where upgrading packages could crash software, but it seems like a useful idea for myself.  Most everyone else will probably never need or want it, but for me it will be nice to use and practice setting up vms on my computer.


#### Update

I built the first version of quickset in pure bash: https://github.com/quickset-org/quickset-bash-archive
And now i'm working on one in Scala because I enjoy developing in Scala so much more.
