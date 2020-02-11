# sample-modifier-plugin
A simple A4C plugin including a sample modifier.

This modifier :

* adds a compute in the topology
* define it's scalable max_instance property to 2
* add relationships between all nodes of the topology to this compute

Since this modifier add an abstract node that should be matched, this modifier must be added in a location having Compute resources configured, and you must setup it in phase `pre-node-match`


![Modifier Setup](doc/setupModifier.png?raw=true "Modifier setup")

At deployment phase you will see your modifier logs 


![Modifier Logs](doc/logs.png?raw=true "Modifier Logs")
