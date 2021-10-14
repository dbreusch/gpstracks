# GPS Tracks
A GPS track viewer and manager web app.

Draws heavily from Udemy course on React, Node, Express and more but integrates
it all into a new, custom MERN application.

## Organization

This app is split into multiple pieces:
* gpstracks: the main organizing component
* [auth-api](https://github.com/dbreusch/auth-api): a Node submodule handling user authorization
* [users-api](https://github.com/dbreusch/users-api): a Node submodule for managing users
* [frontend](https://github.com/dbreusch/gpstracks-frontend): a React app (and submodule) implementing the UI

## Housekeeping
To refresh the submodules from their respective GitHub repositories involves the
following steps (in this folder):
```
git submodule update --remote --recursive
git add .
git commit -m "Updating submodule to latest"
git push
```

Updating in a cloned folder is a little bit different:
```
git pull
git submodule update --remote --recursive
```

Note that the add / commit / push should *not* be needed for the cloned version.
