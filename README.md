<p align="center">
    <img src="animesh.png">
</p>


Animesh is a simple working bash script for streaming anime using mpv. This
script scrapes existing anime streaming sites (only gogoanime.pe supported for
now) to get the video download links and play that using mpv. The script uses
[ueberzug](https://github.com/seebye/ueberzug), a command line utility to
display images in terminal, to show a greeting image and respective anime cover
images.

# Features

* Use ueberzug to view anime cover images  
* Save "currently watching" animes and keep record of the episodes watched and
  unwatched. (TODO)  
* Save anime for watching later in a "watchlist" (TODO)
* Display anime MAL ratings and other infos (TODO)
* Import MAL watchlist (?)


# Dependencies

1. mpv
2. ueberzug
3. libxext-dev
4. curl

# Installation

Install the necessary dependencies for the script to run.

* On ubuntu, run

  ```sh
  sudo apt-get install curl libxext-dev python3-pip mpv
  pip3 install ueberzug --user
  ``` 

* On archlinux, run

  ```sh
  sudo pacman -Syy mpv ueberzug curl
  ```

* On void, run

  ```sh
  sudo xbps-install -Sy mpv ueberzug curl
  ```

After installing the dependencies, run the ```install.sh``` script with root
privileges

```sh
sudo ./install.sh
```

# Usage

Usage is pretty straight-forward. In its current state, the script fully guides
the user through the steps interactively.

<p align="center">
  <img src="./workflow.gif" />
</p>

