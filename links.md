# Links

A link is a pointer pointing to a file or directory. A pointer is an object that stores a memory address. For more technical details, refer to the [Wikipedia article on Pointers](https://en.wikipedia.org/wiki/Pointer_(computer_programming)). Links allow a filename to refer to a file.

There are two types of links.

### A softlink
```bash
ln -s [original filename] [link name]
```

### A hardlink
```bash
ln [original filename] [link name]
```
