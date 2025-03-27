# Build notes

## Local Build

### one time

```bash
paru -S python-pip
# needed? paru -S python-pip
paru -S zephyr-sdk-bin
mkdir ~/Development/github/petejohanson
git clone https://github.com/petejohanson/cirque-input-module ~/Development/github/petejohanson/cirque-input-module
```

### then init with

```bash
source ~/Development/github/FearlessSpiff/ravensplit-zmk-config/scripts/initAndSetupBuildEnv.s

west build -p -b nice_nano_v2 -- -DSHIELD=raveniung -DZMK_EXTRA_MODULES="/home/spiff/Development/github/petejohanson/cirque-input-module;/home/spiff/Development/github/FearlessSpiff/raveniung-zmk-config"

```
