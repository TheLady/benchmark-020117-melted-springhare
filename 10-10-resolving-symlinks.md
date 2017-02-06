---

### 10: Resolving Symlinks

Many Unix-based systems support symbolic links (also known as symlinks). This is where one directory name is transparently mapped to another. Symbolic links can be used to 'redirect' one directory to another directory.

Your challenge is to resolve a given path name into its actual location given a series of symbolic links. Symbolic links can also point to other symbolic links.

**Example Input:**
```
1
/home/private/documents:/stuff/urgent/docs
/home/private/documents/office
```

**Example Output:**
```
/stuff/urgent/docs/office
```

**Another Example Input:**

```
3
/bin:/usr/bin
/usr/bin:/usr/local/bin/
/usr/local/bin/log:/var/log-2017
/bin/log/lib
```

**Another Example Output:**
```
/var/log-2017/lib
```

### Strategy
create key-value pairs of all file paths
create null keys and pass in the  variable representing the new filepath.
make input of new file path generate original file path


newPath1 = oldPath1
newPath2 = oldPath2
newPath3 = oldPath3

if symlink = new_path
   return original_filepath

oldFilepath.newFilepath

hash table?

### Code


