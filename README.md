# ci-smoke-lab-33
Throwaway sandbox for release-readiness CI smoke test of contribution + CI loop (fallback name)

## Build artifact

This repository Smoke-tests the contribution + CI loop end to end.

- The GitHub Actions workflow (`.github/workflows/ci.yml`) is dispatchable via `workflow_dispatch` and runs a single `build` job on `ubuntu-latest`.
- The job writes a short text file (`demo-build.txt`) and uploads it as a build artifact named exactly **demo-build** using `actions/upload-artifact@v4`.
- A pull request titled "Add artifact documentation to README" documents this artifact flow in the README.
- This change was reviewed with a comment review (not an approval) as required for self-authored pull requests.
