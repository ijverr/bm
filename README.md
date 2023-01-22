# bm - A simple bookmarking script
## Installing the script

1. Make sure you have these programs installed: *fzf, xclip, xdg-utils, papirus-icon-theme.*

1. Open the *bm* file in a text editor and replace `/home/user/Documents/bookmarks/` with the full path to your bookmarks folder.

1. If you don't have the Papirus icon theme installed, you can replace `/usr/share/icons/Papirus/64x64/apps/xclipboard.svg` with your desired icon for the notification.

1. Move the edited *bm* file into a PATH folder.\
To find such folders, run `echo $PATH` in a terminal. You can also create a folder for scripts and add it to PATH.

## Adding bookmarks

This is an example directory tree of a bookmarks folder:
```
~/Documents/bookmarks/
├── art
├── cooking
├── electronics
├── fitness
├── linux
├── misc
├── self-hosted
└── text_editing
    ├── groff
    ├── latex
    └── vim

```


To add a bookmark, simply create a text file in the category of your choice and paste the URL address of the website into the first line of the file's content. The name of the file will be the bookmark's title.

## Opening bookmarks

Open the terminal and execute `bm`. Now you can search for a category or specific bookmark. Press enter to open the link.

Thanks to *fzf*, you don't have to type in the exact words.\
For example, if you want to find bookmarks in the "linux" category containing the word "server", you can type in "linserv" and you'll likely get decent results.


The script also detects .onion links. When you want to open such a link, it gets copied to clipboard and a notfication is shown. 
