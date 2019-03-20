# GQM
GQM (Global Queue Management) is an architecture for the provision of QoS in computer networks.

A paper proposing the GQM architecture was published by me in the "2016 17th International Telecommunications Network Strategy and Planning Symposium (Networks)" - https://ieeexplore.ieee.org/document/7751155.

The abstract reads as follows: "This paper describes an architecture for global queue management (GQM). Global refers to the set of all queues in routers present in some network flow path. The main idea of the architecture is the detection of some anomaly somewhere downstream and the propagation of the local decision to a set of upstream routers or switches. The upstream devices are free to act as they wish. GQM is useful to boost some QoS configuration, save network resources, and to provide some mechanism to mitigate network attacks. It's also possible to integrate GQM with SDN, specially with OpenFlow that provides a Controller that can act upon anomaly detection."

This repository will provide the code for the following elements implementing the GQM architecture:

- Anomaly Detector: It runs in kernel space - it's composed of: 
    -- a modified version of the SFB (Stochastic Fair Blue) linux kernel module
    -- some kernel modules 
- GQM Daemons: They run in user space and implement the DGF (discard greatest first) algorithm proposed in the paper as well.
- Miscelaneous: scripts, configuration files, flow rules, etc..


PLEASE VISIT https://gitlab.com/rossanx/gqm FOR UPDATES.
