Chunks from Maven / Ivy repositories, used by coursier during its tests.

To update those, run JVM tests in coursier with `FETCH_MOCK_DATA=1` in the
environment.

```bash
$ FETCH_MOCK_DATA=1 ./mill 'tests.jvm[2.12.18].test.testOnly' coursier.tests.CentralTests
```

Then go to its `tests/metadata` directory (which is a git
submodule), (git) add the newly-created files, commit that, push the result
somewhere, open a PR here.
