# MacBook Dev Setup 💻

A list of my personal preferences and tools to setup a new MacBook for web development. Heavily inspired by Tania Rascias [blog post](https://www.taniarascia.com/setting-up-a-brand-new-mac-for-development/).

## Package Manager

Install Homebrew as package manager.

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Make sure everything is up to data.

```sh
brew update
```

## Terminal

Replace default terminal with iTerm2:

```sh
brew install --cask iterm2
```

Add NightOwl Theme: https://github.com/nickcernis/iterm2-night-owl

Install Oh My Zsh as shell.

```sh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Install Starship prompt: https://starship.rs/de-de/guide/

Install [Fig](https://fig.io) for handy autocompletion.

## Apps

Visual Studio Code (Editor)

```sh
brew install --cask visual-studio-code
```

Chrome & Firefox (Browser)

```sh
brew install --cask google-chrome firefox
```

Maccy (Clipboard Manager)

```sh
brew install --cask maccy
```

Magnet (Window Management): Download from the [App Store](https://apps.apple.com/de/app/magnet/id441258766?mt=12)

Spotify (Music)

```sh
brew install --cask spotify
```

Insomnia (API tool)

```sh
brew install --cask insomnia
```

1Password (Password Manager): https://1password.com/de/downloads/mac/

Raycast (Spotlight alternative)

```sh
brew install --cask raycast
```

Bear (Note Taking): Download from the [App Store](https://apps.apple.com/de/app/bear-private-notizen/id1091189122?mt=12)

Zoom (Video Calls): https://zoom.us/download

Around (Video Calls): https://around.co

Local (Local WordPress Development): https://localwp.com

Local PHP Development: https://oliverbrux.de/blog/laravel-valet-die-schnelle-mamp-alternative-fuer-den-mac#:~:text=Valet%20ist%20eine%20minimalistische%20Entwicklungsumgebung,Projektes%20um%20Valet%20zu%20nutzen

GitHub Desktop: https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/installing-and-authenticating-to-github-desktop/installing-github-desktop

## Node.js

Install nvm to use multiple Node.js versions and be able to switch between them project based.

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```

Install the latest Node.js version

```sh
nvm install node
```

Restart terminal and run the final command.

```sh
nvm use node
```

Set a default version:

```sh
nvm alias default xx.xx
```

## Git

Install via Homebrew.

```sh
brew install git
```

Create a global configuration file.

```sh
touch ~/.gitconfig
```

Input the config and create some aliases

```
[user]
  name   = Firstname Lastname
  email  = you@example.com
[github]
  user   = username
[alias]
  a      = add
  ca     = commit -a
  cam    = commit -am
  cm     = commit -m
  s      = status
  p      = push
  pom    = push origin master
  puom   = pull origin master
  cob    = checkout -b
  co     = checkout
```

## System Settings

- Make Chrome default browser
- Automatically hide and show Dock
- Enable "Tap to click"

## Application Settings

### Chrome

- Install uBlock Origin
- Install React DevTools
- Install JSONView
- Install Duplicate Tab Shortcut

### Visual Studio Code

- Press `CMD + SHIFT + P` and click "Install code command in PATH"
- Install Night Owl Theme
- Install Prettier
- Install file-icons
- Install ESLint
- Install Auto Rename Tag
- Install Live Share
- Install Simple React Snippets
- Install Tailwind CSS Intellisense
- Set editor font to 'Operator Mono'
- Set sidebar location to right
