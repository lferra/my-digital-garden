---
{"dg-publish":true,"permalink":"/gentoo/"}
---


Some env variables overrides
/etc/X11/xinit/xinitrc.d
/etc/X11/xinit/xinitrc.d/61-cadence-session-inject.sh

```shell
export LADSPA_PATH="$LADSPA_PATH:`$INSTALL_PREFIX/bin/cadence-session-start --printLADSPA_PATH`"
export DSSI_PATH="$DSSI_PATH:`$INSTALL_PREFIX/bin/cadence-session-start --printDSSI_PATH`"
export LV2_PATH="$LV2_PATH:`$INSTALL_PREFIX/bin/cadence-session-start --printLV2_PATH`"
export VST_PATH="$VST_PATH:`$INSTALL_PREFIX/bin/cadence-session-start --printVST_PATH`"
```

Environment variables x user
~/.config/environment.d/99-xdg-ninja.conf

LightShaders
- Install configuration: "Debug"
-- Installing: /usr/lib64/qt5/plugins/kwin/effects/plugins/kwin4_effect_lightlyshaders.so
-- Installing: /usr/share/kwin/shaders/1.40/lightlyshaders.frag
-- Installing: /usr/lib64/plugins/kwin/effects/configs/kwin4_lightlyshaders_config.so
