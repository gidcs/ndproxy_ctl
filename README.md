# ndproxy_ctl
ndproxy_ctl is a tool designed for simplifing the job of setup ndp proxy. This tools is designed for proxmox, but it should works on other distributions. You need to add post-up and post-down manually after your network interfaces configuration in order to make the rules always loaded.

## Usage
	
	ndproxy_ctl load
	ndproxy_ctl unload
	ndproxy_ctl reload
	ndproxy_ctl list
	ndproxy_ctl add <in_interface> <out_interface> <ipv6>
	ndproxy_ctl del <in_interface> <out_interface> <ipv6>

## Example
	ndproxy_ctl list
	ndproxy_ctl add vmbr0 eth0 1234:1234:56:7890::1
	ndproxy_ctl del vmbr0 eth0 1234:1234:56:7890::1

## License

Copyright year [guyusoftware]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

[guyusoftware]: https://www.guyusoftware.com/