# Changelog

## 0.35.21 - 2026-08-03

- Keeps the SuperApp AI sign-in separate from personal Codex credentials and
  stops importing personal credentials into the app.
- Makes AI sign-in repair crash-safe without logging out or revoking the
  user's personal Codex sign-in.
- Routes authentication recovery to the connection mode used by the failed
  run, including SuperApp, API-key, and personal Codex modes.
- Preserves the privacy behavior from 0.35.17: no recurring balance or hosted
  history polling, and downloaded run history remains local.

This release supersedes 0.35.18. It is a signed and Apple-notarized Apple
silicon macOS release.

## 0.35.18 - 2026-08-02

- Tests the AI engine end to end during new setup and on demand in Settings,
  instead of treating a saved login as proof that the model can respond.
- Explains account, plan, quota, region, model, rate-limit, and timeout failures
  in plain language.
- Warns when a real run receives no model activity and keeps probe results
  entirely local.
- Makes one deliberate model request per test and never loads On-Page.ai or
  other SuperApp connectors during that test.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.17 - 2026-08-02

- Removes unapproved pricing and credit promotional copy from the On-Page.ai
  onboarding step.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.16 - 2026-08-02

- Stops recurring background balance checks and keeps monitoring local by
  default.
- Stores downloaded scheduled-scan history locally in the SuperApp.
- Repairs valid On-Page.ai connections whose local scan connector did not
  finish setup.
- Leads first-time setup directly into the first SEO report.
- Explains when a report cannot run because a required page URL is missing.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.15 - 2026-07-31

- Updates On-Page.ai onboarding for the one-time $1 activation.
- Explains that activation includes $10 in credits, or $20 with a business
  email.
- Updates Setup Center and connection calls to action to match the production
  signup flow.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.14 - 2026-07-25

- Keeps follow-up conversations at the latest response instead of jumping back
  to the top.
- Keeps draft messages and attachments isolated to the task where they were
  added.
- Allows the next follow-up to be drafted while the current run finishes.
- Improves modal dismissal, keyboard handling, and draggable window placement.
- Improves report behavior in narrow windows and prevents completed progress
  animations from replaying.
- Makes runtime errors selectable so diagnostic details can be copied when
  support is needed.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.12 - 2026-07-24

- Improved On-Page.ai credit handling across workflows and setup.
- Detects real provider billing failures, including failed MCP tool responses
  returned inside otherwise successful AI runs.
- Keeps validation and runtime errors separate from billing issues.
- Preserves connection management while offering a clear way to get more
  credits.
- Displays fractional balances accurately and treats low credits as attention,
  not a disconnected account.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.11 - 2026-07-24

- Restored Google Search Console token refresh for existing connections.
- Restored authenticated Search Console requests such as sitemap submissions.
- Kept Google OAuth credentials bundled inside the signed app so users do not
  need to provide a client ID or client secret.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.10 - 2026-07-24

- Fixed first-run AI connection failures caused by stale or incompatible
  personal Codex model configuration.
- Isolated SuperApp-managed AI setup from personal Codex settings while
  preserving an existing ChatGPT or Codex sign-in when available.
- Prevented local configuration paths and parser details from appearing in
  onboarding errors.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.9 - 2026-07-23

- Removed a shared desktop OAuth secret from distributed application builds.
- Added release-time checks for credentials, private repository references, and
  local build paths.
- Removed local build paths from compiled release metadata.
- Updated in-app support links to this public repository.

This is a signed and Apple-notarized Apple silicon macOS release.

## 0.35.8 - 2026-07-23

- Added the current SEO, monitoring, browser, indexation, and personal-indexer
  workflows.
- Improved onboarding, setup, recipe discovery, settings, and agency project
  navigation.
- Added current usability, delivery, and security hardening.
- Routed in-app support to this public support repository.

This is a signed and Apple-notarized Apple silicon macOS release.
