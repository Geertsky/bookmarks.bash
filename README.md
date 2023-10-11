# bookmarks.bash
Bookmarks.bash is repository just to tryout writing nvim plugins.

bookmarks.bash contains a `/etc/profile.d` script that defines, optionally prefixed aliases for `cd` commands to the paths defined in a lua table in `BOOKMARKSPATH`.
The `bookmarks.bash` script is meant to be used in combination with the [bookmarks.nvim](https://github.com/Geertsky/bookmarks.nvim) plugin. 
# installation
```
git clone https://github.com/Geertsky/bookmarks.bash
cp bookmarks.bash/etc/profile.d/bookmarks.sh /etc/profile.d/
```

## bookmarks.lua
The `bookmarks.lua` returns a table a typical example:
```
return {
  ce='/etc',
  ch='/home',
}
```

# Configuration
In the `bookmarks.sh` script there are two variables that influence the functioning of the `booksmarks.sh` script:
|variable       |Description                                                        |
|---------------|-------------------------------------------------------------------|
|`BOOKMARKSPATH`|Points to the lua file containing the table with aliases for paths.|
|`PREFIX`       |An optional prefix for the aliasses.                               |
