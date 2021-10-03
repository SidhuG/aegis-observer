# aegis-observer
Observes users, apps' and services' behaviour. Observer is one of the tools in aegis collection. The other key tools are:

* [AEGIS-IDENTITY](https://github.com/SidhuG/aegis-identity)
* [AEGIS-ENFORCER](https://github.com/SidhuG/aegis-enforcer)
* [AEGIS-ENGINE](https://github.com/SidhuG/aegis-engine.git)

# Introduction
Observer is a key tool that records the behaviour of running users, apps and services on a system under observation, with the objective that observed behaviour of these is used to detect anomalous behaviour in a production system.

**Aegis-Observer** records the actions of a running program/executable. During test cycle it records action at a very granual level and writes down a trail of those actions. These trails form the whitelist of actions. That is, this is what that executable/binary which is not compromised would do. In a production or live environment aegis-observer observes actions again, however, this time, it is meant for the purpose of monitoring those in order to allow only non-anomalous, secure operations and actions. Aegis-observer is dependent on the aegis-identity, however, it can be used standalone with no Aegis-engines. As a stand alone it can only flag when certain percentage of observable actions go out of track

When used along with enforcer, Aegis could be used either just to monitor and flag or to actively prevent anomalous behaviour on a production system.

