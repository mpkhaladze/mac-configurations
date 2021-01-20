# Mac-configurations
## Redis
```$brew install redis```

After installation

Launch Redis on computer starts.

```$ ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents```

Start Redis server via “launchctl”.

```$ launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist```


Start Redis server using configuration file.

```$ redis-server /usr/local/etc/redis.conf```

Stop Redis on autostart on computer start.

```$ launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.redis.plist```

Location of Redis configuration file.

```/usr/local/etc/redis.conf```

Uninstall Redis and its files.

$ brew uninstall redis

```$ rm ~/Library/LaunchAgents/homebrew.mxcl.redis.plist```

Get Redis package information.

```$ brew info redis```

Test if Redis server is running.

```$ redis-cli ping```

shoud get ```PONG``
