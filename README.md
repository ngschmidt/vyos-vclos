# VyOS Virtual Clos Topology Deployment Templates

## Synopsis

Provide a base configuration to "jump-start" a basic Clos topology composed of Vyos VMs

### This Will

- Set up interface `eth0` as a DHCP client
- Set up VRF `mgmt` to keep eth0 separate. This will allow consumers to keep an easy, automatically bootstrapped out-of-band point of administration.
- Set up SSH/API for remote administration once it's on-line
- Configure a "fat tree" of routers to connect to each other via eBGP

## To use these examples

- Perform a new VyOS installation: <https://docs.vyos.io/en/latest/install.html>
- Install the provided configuration into that virtual router
- Update VyOS (if applicable), and load any custom software.
- Package into OVA or VM Template
- Deploy configurations

From there, it's possible to perform get and post invocations.

## Tested Platforms

- VyOS Rolling

## Notes

- Set your own password - that is not included in this configuration.
- This doesn't set up any virtual topologies yet, or deploy images for you.

## Authors

- *Nick Schmidt*
