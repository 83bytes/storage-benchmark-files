# Benchmark data dump

- The file tree is rooted at the devices that are being benchmarked.
- Inside each directory there are directories of different systems on which the benchmarks were run.
- Inside there directories we have the output from fio itself.
- We also have screenshots from netdata.
- We have directories labelled `4M` which have the reports and images of the test run with block_size=4M
- the bench.sh script has some very shit code that will go through the destinations and run the same tests (write, then read).

# setup
- use parted to create the partitions
- use `mkfs` to build the btrfs and ext4 filesystems
- use cryptsetup to create the encrypted drives.

# DO NOT USE THE SCRIPT AS IS.
# READ IT.
# UNDERSTAND IT.

# ANY MISTAKE WILL DESTROY YOUR SYSTEM