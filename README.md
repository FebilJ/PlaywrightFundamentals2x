
# PlaywrightFundamentals2x

A small Playwright test repository for learning and experimenting with Playwright test automation.

## Project Overview

- Framework: Playwright
- Test runner: `@playwright/test`
- Test directory: `./tests`
- Example site: `https://playwright.dev/`
- Browser projects configured: `chromium`, `firefox`, `webkit`
- Reporter: HTML

## Setup

1. Install dependencies:

```bash
npm install
```

2. Verify installation by running the example tests:

```bash
npx playwright test
```

## Running Tests

- Run all tests:

```bash
npx playwright test
```

- Run tests in headed mode:

```bash
npx playwright test --headed
```

- Run a specific test file:

```bash
npx playwright test tests/example.spec.ts
```

- Open the HTML report after tests complete:

```bash
npx playwright show-report
```

## Project Structure

- `package.json` - project metadata and dependencies
- `playwright.config.ts` - Playwright configuration
- `tests/example.spec.ts` - sample end-to-end tests
- `playwright-report/` - generated Playwright HTML report output
- `test-results/` - generated test result artifacts

## Notes

- The tests currently navigate to Playwright's documentation site and verify page title and navigation.
- Update `playwright.config.ts` to add a base URL, custom reporters, or additional browser/device profiles.
- If running in CI, retries are enabled and worker count is adjusted automatically.
