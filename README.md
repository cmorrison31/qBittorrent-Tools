# qBittorrent-Tools
This project is a collection of scripts for managing torrents in a 
qBittorrent instance.

## Available Scripts
 - orphaned_torrents
 - unregistered_torrents

## Note
qBittorrent-Tools is not affiliated with the official 
[qBittorrent project.](https://www.qbittorrent.org//)

# License
This project is licensed under the MIT license. See LICENSE.txt for more 
information.

# Configuration
Create a `config.ini` file like so:

```ini
[qBittorrent-Tools]
username = username
password = password
server url = example.com:port
paths to ignore = 'some path'

[path maps]
some path = another path
```

# Example Usage
Call the script function for the operation you wish to execute. The 
`config.ini` file needs to be in the same directory as your script. 

For example, if checking for unregistered torrents, the following script 
calls the appropriate function.

```python
from qBittorrentTools import Scripts


def main():
    Scripts.unregistered_torrents()
    

if __name__ == "__main__":
    main()

```
