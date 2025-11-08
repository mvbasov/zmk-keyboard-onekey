## About
[onekey keyboard](https://github.com/jibingeo/zmk-config-onekey) example redesigned as module according to actual ZMK documentation.

## Usage

Edit your west.yml file found in your zmk-config's config directory to add the akohekohe module. Example:

west.yaml needs to be looks like

```
manifest:
  remotes:
    - name: zmkfirmware
      url-base: https://github.com/zmkfirmware
    - name: mvbasov
      url-base: https://github.com/mvbasov
  projects:
    - name: zmk
      remote: zmkfirmware
      revision: main
      import: app/west.yml
    - name: zmk-keyboards-katori
      remote: mvbasov
      revision: main
  self:
    path: config
```
