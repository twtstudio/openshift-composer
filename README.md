# OpenShift Composer Cartridge

## Installation - OpenShift Online

Runs Composer on OpenShift using downloadable cartridge support. To install to OpenShift from the CLI, create your app and then run:

```
rhc add-cartridge http://cartreflect-claytondev.rhcloud.com/reflect?github=twtstudio/openshift-composer
```

## Installation - OpenShift Origin

```
curl -L https://github.com/twtstudio/openshift-composer/archive/master.tar.gz | tar zxv
oo-admin-cartridge -d -a install -s ./openshift-composer-master/ --mco
oo-admin-broker-cache --console 
```

Then add composer cartridge to your app via `rhc` cli or web console.

## Markers

| marker | control |
|--------|---------|
| `composer_off` | skipping `composer install` when build |
| `force_clean_build` | clean vendors but not cache |


