# y-cruncher

y-cruncher is a program written by Alexander J. Yee. More information can be
found at numberworld.org. In this repository, I keep the validation files for
computations I have run. I may also put small portions of the digits or
properties computed from the digits (since uploading many GB/TB of digits is
infeasible and not appropriate for a git repository).

The machine I am currently using to compute digits is described below. Many of
the components were found recycled.

Last date system was modified: 2020-06-10

- OS: Ubuntu Server 18.04 with Linux kernel 4.15.0
- System board: Asus P6T Deluxe V2 (found recycled)
- CPU: i7-920 @ 2.67 GHz (4C / 8T) (found with system board)
- Memory: 6x 4 GiB triple channel PC3-12800U (DDR3-1600) running at 1066 MHz
(taken from a few recycled Dell Optiplex 7010 computers)
- GPU: some old ATI Radeon card (found recycled)
- PSU: Corsair HX850 (borrowed from a PC I built years ago)

Previous disk setup (starting out):

- Scratch space disks:
  - 6x 250GB SATA, connected to SATA ports, various models found recycled
  - 6x 320GB SATA, connected to Dell PERC H200, various models found recycled
  - 6x 320GB was added later on for larger computations (500 billion digits)
  - 1 of the 320GB drives had to be replaced due to read errors
- Output space disks:
  - 3x 250GB IDE, found recycled
  - 1 connected to system board IDE, 2 connected to a 2x IDE PCI card

Current disk setup (larger HDDs available for 1 trillion digit computations):

- Scratch space disks:
  - 12x 500GB SATA, all model ST500DM002
  - 8 connected to Dell PERC H200, 4 connected to SATA ports
- Other disks:
  - 2x 500GB SATA, both ST500DM002, mdadm RAID-0 for output
  - 1x 250GB IDE, for the OS/boot device
- Notes
  - 6.0 MiB/seek gives better far memory tuning results for the IO performance
    analysis
