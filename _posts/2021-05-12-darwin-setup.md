---
layout: post
title:  "How I setup my Mac"
date:   2021-05-12
categories: mac, setup
---

# Darwin
MacOS Big Sur 11.2.3 (20D91)

### System Preferences
1. Open `System Preferences`
2. Choose `General`
3. Uncheck `Allow wallpaper tinting in windows`
4. Uncheck `Close windows when quitting an app`
5. Uncheck `Allow Handoff between this Mac and your iCloud devices`
6. Return and choose `Dock & Menu Bar`
7. Uncheck `Animate opening applications`
8. Check `Automatically hide and show the Dock`
9. Uncheck `Show recent applications in Dock`

### Finder Preferences
1. Open `Preferences`
2. Uncheck all options for desktop
3. Set `New finder window show:` to your username
4. Choose `Sidebar`
5. Check home diretory
6. Uncheck tags
7. Uncheck hard drives
8. Uncheck Recent
9. 

### Create home directory
```
cd ~
mkdir Home
```

### Create dotfiles directory
```
cd ~/Home
mkdir dots
```

### Install Xcode (optional)
1. Open `App Store`
2. Log in with your Apple ID
3. Search `Xcode`
4. Click `Get`
5. Open `Xcode` and let it install components

### Install Bear Notes (optional)
1. Open `App Store`
2. Log in with your Apple ID
3. Search `Bear`
4. Click `Get`

### Install brew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Install pictogram (optional)
```
brew install pictogram
```

### Install lunar (for external monitor)
```
brew install --cask lunar
```

### Install lightweight windows manager Rectangle
1. `brew install --cask rectangle`
2. Go to `Preferences`
3. Add 20 px gap

### Install nerd font (I like Fira Code, there are more)
```
brew tap homebrew/cask-fonts
brew install --cask font-fira-code-nerd-font
```

### Setup Terminal
```
1. Open Preferences
2. Choose `Profiles`
3. Press `Change...` next to Font
4. Choose installed nerd font, and size
```

### Setup ZSH (I also like fish)
1. `touch ~/Home/dots/zshrc`
2. `ln -s ~/Home/dots/zshrc ~/.zshrc`
3. Install Starship promt 
    - `brew install starship`
    - `eval "$(starship init zsh)"` add to the end of `~/.zshrc`
4. ...

### Install `exa` (todo: change this to isntall my toolkit)
```
brew install exa
# add `alias ls='exa -a --group-directories-first --git-ignore'` to ~/.zshrc
```

### Setup Ruby
```
brew install rbenv
rbenv init
# add to ~/.zshrc using vim/nano:
# eval "$(rbenv init -)"
exec "$SHELL"
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash
rbenv install 3.0.0
rbenv global 3.0.0
```

### Setup Python
```
brew install pyenv
# add to ~/.zshrc using vim/nano:
# eval "$(pyenv init -)"
exec "$SHELL"
pyenv install 3.9.1
pyenv global 3.9.1
pyenv rehash
```

### Setup Rust
```
brew install rust
```

### Setup Racket
```
brew install racket
```

### Install VS Code (optional)
```
brew install visual-studio-code
mv ~/.vscode ~/Home/dots/vscode
ln -s ~/Home/dots/vscode ~/.vscode
```
Use pictogram to set icon from this directory. (optional)

### Setup VS Code
1. Open `Settings`
2. Set `workbench.settings.editor` to json
3. Open `Settings` again
4. Set `telemetry.enableTelemetry` to false
