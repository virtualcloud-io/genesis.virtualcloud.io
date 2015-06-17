**Status: DEV**

Genesis.VirtualCloud.IO
=======================

When applications are distributed some important questions arise:

  * Where does the application originate from?
  * Which resources and APIs does the application access?
  * Has the application been modified?
  * How are the root encryption keys managed and rotated?
  * How are new releases distributed?
  * How are bugs reported and traced?
  * How is the distribution infrastructure for the application designed?
  * How many operational people is the application dependent on?
  * Which geographic region is the application dependent on?
  * Which technologies is the application dependent on?

All these factors and many more impact the extent to which an application is **Sound & Robust**.

**VirtualCloud** is an effort to make applications **Sound & Robust** by providing:

  * Namespaces suitable for a global architecture and distribution
  * A root JSON config object for the entire distribution
  * Declared contracts for all outside resources and APIs
  * Hash-based integrity verification
  * Cryptographic-based identity verification & security
  * Nested & linked JSON configurations to accomodate complexity
  * Pluggable visualisation of the resulting Semantic Web using Web Components

[Genesis.VirtualCloud.IO](https://github.com/virtualcloud-io/genesis.virtualcloud.io) provides an implementation for [genesis.pinf.org](https://github.com/pinf/genesis.pinf.org) based systems.


Use
===

This project is not yet ready for independent use although that is the goal.

To see it in action visit [genesis.virtualcloud.io](http://genesis.virtualcloud.io) for templates and install (core.open.genesis.ginseng.io)[http://core.open.genesis.ginseng.io] which provides a visual UI for VirtualCloud and access to all available features.


FAQ
===

Why JSON and not JavaScript
---------------------------

You cannot *declare* javascript. You have to code and run it.

The fastest way to modify something is to change a declaration (map to something already existing), not to code it (state that something exists). If our configuration language does not embody this property we have no hope in achieving sound abstractions in our systems.

Even if you use JavaScript to generate your configurations, you *should be generating JSON* and you *should be using JSON* to control the generation. *Using JSON* means being able to persist your controlling context and your generated result in JSON for every iteration.

Thus JSON precedes all.


