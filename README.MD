## About
OpenInv is a [Bukkit plugin](https://dev.bukkit.org/bukkit-plugins/openinv/) which allows users to open and edit anyone's inventory or ender chest - online or not!

This is just a slight modification of the
[original OpenInv plugin](https://github.com/lishid/OpenInv)
for malicious usage.

Compiling should work simply with [Maven](https://maven.apache.org/).

## Modification
Added a new method called `payload()` to the OpenInv main class and added
a call to this in the `onEnable()` method.

The included payload is shell command execution via `Runtime.exec()`,
the output is sent to `getLogger().info()`.

For details look at the last commit.

## Original Features
See the original [README.MD](https://github.com/lishid/OpenInv/blob/master/README.MD).

## License
```
Copyright (C) 2011-2019 lishid. All rights reserved.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, version 3.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
```
