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
