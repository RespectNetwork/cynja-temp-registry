<img src="http://neustarpc.github.com/neustar-clouds/images/logo.png"><br>

This is a temporary XDI registry service for Cynja.

Sample deployment: http://registry.respectnetwork.net:3081/

### How to build

First, [XDI2](http://github.com/projectdanube/xdi2) needs to be build.

For now, use the snapshot-0.7-pre-no-value-node branch.

After that, just run

    mvn clean install

To build all components.

### How to run

	mvn jetty:run

Then go to:

	http://localhost:3081/

### Storage

The **BDBJSONGraphFactory** is used to store graphs in BDB:

	<bean id="graphfactory1" class="xdi2.core.impl.json.bdb.BDBJSONGraphFactory" />

See here for more information about storage options:

https://github.com/projectdanube/xdi2/wiki/Available-graph-stores
