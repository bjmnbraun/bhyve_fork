Fork of bhyve hypervisor for FreeBSD

Changes made:
 - Time in guest is tracked in stats
 - VM exits total count is tracked in stats
 - Both are exposed as sysctl
  (Not implemented - instead the time in guest
  and vm exits are dumped to console every second)

Note:
 - Multiple TODOs in code comments, all changes localized to bhyverun.c.

INSTALLING:
 - Check out this repository to a local directory
 - Build with `./run_make.sh`
 - In this directory, run `sudo ./vmrun.sh` as a replacement for
        `/usr/share/examples/bhyve/vmrun.sh`

 Note: bash shell is assumed for both of the above scripts.
