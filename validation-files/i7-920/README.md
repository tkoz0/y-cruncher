# i7-920 PC

See system specification in the main README.md

Below is a list of computations performed on this machine:

Computation 1: "e - 20200120-235640.txt"
- e: 100B digits, ~23 hours (on 2020-01-20)
- This computation ran smoothly without interruption and finished sooner than I
was expecting.

Computation 2: "e - 20200124-111110.txt"
- e: 300B digits
- Started on 2020-01-21, completed on 2020-01-24
- Since the previous computation went smoothly, I decided to compute e again,
but to as much precision as disk space will allow. This also completed without
issues.

Computation 3: "Golden Ratio - 20200611-024046.txt"
- Golden Ratio: 25B digits, ~85 minutes (on 2020-06-10)
- This was run to test the new setup with 12 hard drives

Computation 4: "e - 20200615-010201.txt"
- e: 500B digits
- Started on 2020-06-11, completed on 2020-06-15
- One of the 320GB drives had a read error which interrupted the computation.
  Resuming was attempted, but another read error occurred on the same drive. The
  drive was replaced with a 500GB drive after copying over the checkpoint files.
- Computation finished after about 4 days and digits were correct

Computation 5: "Pi - 20200628-044855.txt"
- pi: 500B digits
- Started on 2020-06-15, completed on 2020-06-28
- Digits match known results, no interruption during all 13 days

Computation 6: "Euler's Constant - 20200818-033117.txt"
- euler-mascheroni: 100B digits
- Started on 2020-06-28, completed on 2020-08-18 (almost 2 months)
- This computation would run for a long time, raising concern with the old hard
  drives in use, about half of which have SMART stats indicating problems.
- 4 power failures occurred during the computation, y-cruncher successfully
  recovered each time. Checkpoint files were backed up on 2020-07-28 which was
  right after the 3rd power failure and 1 month into the computation.
- Almost 1PB of disk IO occurred, about 80TB per hard drive. For the smaller
  drives (250GB), this is about 320 times their capacity.
- The computation was able to finish successfully without any hard drive issues
  and the digits match known results.

Computation 7: "e - 20200901-105206.txt"
- Run from 2020-08-26 to 2020-09-01, about 6 days without interruption
- Successful first computation with the newer hard drives (12x500GB)
- CPU utilization ~79%, up from 64% with the slower hard drives

Computation 8: "y-cruncher Checkpoint File (Pi 1T 20200916).txt
- Run from 2020-09-01 to 2020-09-15
- y-cruncher encountered a read error
- The disk mounted at /mnt/y07 failed during operation, data is unreadable
- Computation cannot continue, must restart from beginning
