# Maestro – Wikipedia App E2E Tests

> 🚧 **Work in progress.** The structure and flows are still changing.

A practice project for end-to-end mobile test automation with [Maestro](https://maestro.mobile.dev/), using the Wikipedia Android app (`org.wikipedia`) as the app under test.

## Structure

```
flows/       Test flows grouped by feature (basic, search, auth…)
subflows/    Reusable steps (e.g. skipping onboarding)
scripts/     JS scripts for generating test data
samples/     Official Maestro sample flows, kept for reference
config.yaml  Workspace configuration
```

## Running

1. Install [Maestro](https://maestro.mobile.dev/getting-started/installing-maestro).
2. Have an Android emulator or device with the Wikipedia app installed (the APK is not included in the repo).
3. Run:

```bash
maestro test .                      # all flows
maestro test --include-tags smoke . # smoke tests only
```
