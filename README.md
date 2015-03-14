# Matrix Client script for WeeChat

This script is considered beta quality as not all functionality is in place and still has known bugs, and unknown bugs to be discovered and fixed.

## What is Matrix ?

Matrix is a new open source realtime federated chat protocol. You can read more about it on [http://matrix.org/blog/faq/](their website).

## What is WeeChat ?

[http://weechat.org](WeeChat) is a super powerful CLI chat client that's extensible in many languages to allow for new protocols like Matrix.

## How to load and use the plugin

```bash
# Clone my repo
git clone https://github.com/torhve/weechat-matrix-protocol-script.git
# Copy the script into WeeChat's Lua autoload dir
cp weechat-matrix-protocol-script/matrix.lua ~/.weechat/lua/autoload
# Start WeeChat
weechat
```

```
/lua load matrix.lua
/set plugins.var.lua.matrix.user username
/set plugins.var.lua.matrix.password secret
/matrix connect
```

## How to get WeeChat & Lua deps up and running on Debian/Ubuntu:

```bash
sudo apt-get install weechat lua-cjson
```

## How to get WeeChat & Lua deps up and running on OSX:

```bash
sudo port install weechat +lua
sudo port install luarocks
sudo luarocks install lua-cjson
export LUA_PATH="/opt/local/share/luarocks/share/lua/5.2/?.lua;/opt/local/share/luarocks/share/lua/5.2/?/init.lua;$LUA_PATH"
export LUA_CPATH="/opt/local/share/luarocks/lib/lua/5.2/?.so;$LUA_CPATH"
```



# License

MIT
