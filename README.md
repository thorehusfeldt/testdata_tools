# Testdata Tools

`gen.sh` contains bash helper functions for working with problems for the
Kattis format, particularly ones that use multiple test groups.

See `generator_example.sh` or `generator_example_acm.sh` for example usage,
and `examples/` for complete example problems.

There used to be CMS support. If you need that, look at the repo history.

`gen.sh` (or the whole repo, whatever is most convenient) is intended to be
copied into your contest's repo and committed. `gen.sh` may be changed freely
if needed.

`analyzetestgroups.py` performs some checks based on the log generated by `Kattis/problemtools/verifyproblem`, allowing submissions to hint at expected grades using a comment line like `@EXPECTED_GRADES@ AC WA TLE TLE` to indicate that the grader should produce, _e.g._, `WA` on secret test group 2. Run
```sh
   python3 analyzetestgroups.py examples/arithmetic2
```
for an example.

License: CC0
