# Build notes

## Local Build

### one time

```bash
mkdir ~/Development/github/petejohanson
git clone https://github.com/petejohanson/cirque-input-module ~/Development/github/petejohanson/cirque-input-module
```

### then Build

```bash
cd ~/Development/github/zmkfirmware/zmk/app
west build -p -b nice_nano_v2 -- -DSHIELD=raveniung -DZMK_EXTRA_MODULES="/Users/spiff/Development/github/petejohanson/cirque-input-module;/Users/spiff/Development/github/FearlessSpiff/raveniung-zmk-config"

```
