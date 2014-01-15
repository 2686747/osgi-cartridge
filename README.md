# OpenShift OSGI cartridge

This cartridge embeds Apache Felix runtime as a base for OSGI based applications on OpenShift.

## How to

Just create new gear with this cartridge

```
http://cartreflect-claytondev.rhcloud.com/reflect?github=openshift-cartridges/osgi-cartridge
```

## Control

At this time, there is not functionality exposed by default. When you start the cartridge, OSGI environment is started for you, however there is no public facing interface. To control the cartridge, you need to SSH inside your gear and manage the environment using the provided telnet server.

```
rhc ssh <your app name>
telnet ${OPENSHIFT_OSGI_IP} 15026
```
