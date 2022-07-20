# YTerMusic

YTerMusic is a terminal based Youtube Music Player.
It's aims to be as fast and simple as possible.

## Features

- Play your Youtube Music SuperMix in the terminal
- Memory efficient (Around 20MB of RAM while fully loaded)
- Cache all downloads and store them
- Work even without connection (If musics were already downloaded)
- Automic background download manager

## Installation

- Download the lastest version from `releases`
- Create a `headers.txt` file and copy your headers from the nav when browsing https://music.youtube.com/
  - Your headers should be in the following format:
  ```
  HeaderName: HeaderValue
  ```
- Run `ytermusic.exe`

## Screenshots

![https://user-images.githubusercontent.com/16625987/163998193-8c5557e5-3d97-489d-b678-0a5b8db1c523.png](https://user-images.githubusercontent.com/16625987/163998193-8c5557e5-3d97-489d-b678-0a5b8db1c523.png)
![https://user-images.githubusercontent.com/16625987/163998477-0feb87a0-dfde-4940-a5d1-09807968ec6d.png](https://user-images.githubusercontent.com/16625987/163998477-0feb87a0-dfde-4940-a5d1-09807968ec6d.png)

## Building from source

- Clone the repository
- Install rust `https://rustup.rs`
- Run `cargo build --release`
- The executable is in `target/release/ytermusic.exe` or `target/release/ytermusic`

## Usage

- Use your mouse to click in lists if your terminal has mouse support
- Press `Space` to play/pause
- Press `f` to search
- Press `Arrow Right` or `>` to skip 5 seconds
- Press `Arrow Left` or `<` to go back 5 seconds
- Press `CTRL + Arrow Right` or `CTRL + >` to go to the next song
- Press `CTRL + Arrow Left` or `CTRL + <` to go to the previous song
- Press `+` for volume up
- Press `-` for volume down
- Press `ESC` to exit the current menu
- Press `CTRL + C` or `CTRL + D` to exit

## Features and upcomming features

- [x] Playlist selector
- [x] Error message display in the TUI
- [x] Enable connection less music playing
- [ ] Cache limit to not exceed some given disk space
- [x] A download limit to stop downloading after the queue is full
- [x] Mouse support

## Changelog

Alpha a0.0.5

- Added local database cache to improve IO accesses
- Added searching for musics in the local library
- Greatly improved render performance and RAM usage
- Error management and error display in specific screen

Alpha a0.0.4

- Added menu navigation
- Added searching for musics
- Added new terminal backend

Alpha a0.0.3

- Mouse support to select playlist and music
- Download limiter
- Connection less music playing

Alpha a0.0.2

- Playlist selector
- Improved error management
- Improved TUI
- Performance upgrade
- Switch to Rustls instead of openSSL
