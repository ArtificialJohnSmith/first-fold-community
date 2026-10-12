# Volunteer testing checklist

Use fictional, disposable, non-sensitive sample data. Public reports must not contain private files, financial data or secrets. Test your own sample data only; do not probe accounts or services belonging to others.

## Before testing
- [ ] Choose one tool and read its stated scope and limitations.
- [ ] Record the tool URL, test date, browser/version, operating system, device type and approximate viewport size.
- [ ] Keep backups outside the tool. Use a fresh sample workspace where possible.
- [ ] Define an expected result you can check independently.

## Core behavior
- [ ] Complete one small typical task and compare the output against the expected result.
- [ ] Try empty input, malformed input, supported boundaries and a reasonable unsupported case.
- [ ] Check that errors explain what to fix and do not silently produce misleading output.
- [ ] Where supported, import a synthetic sample, edit it, export it and inspect the actual downloaded file.
- [ ] Reopen exported files in a suitable independent viewer; verify content, format and size.
- [ ] Test Cancel, repeated clicks, undo/redo and restart where the tool offers them.
- [ ] Check reload and local save/restore with disposable records; distinguish an intentional clear from unexpected data loss.

## Usability
- [ ] Try keyboard navigation, visible focus, labels and error messages.
- [ ] Check zoom, long text and a narrow viewport. State whether this was a real device or an emulated viewport.
- [ ] Try a second browser or physical device if available; report exactly what was tested.
- [ ] For print features, inspect native print preview and the saved/printed output if you can. Do not call an HTML preview a verified print result.

## Report
- [ ] Search existing issues for the same problem.
- [ ] Provide numbered reproduction steps, expected behavior and actual behavior.
- [ ] Include only a minimal synthetic sample, sanitized error text and redacted screenshots.
- [ ] Mark results passed, failed or not tested; do not equate untested with passed.
- [ ] Note whether the issue reproduces consistently and whether it risks incorrect output or data loss.

Testing is voluntary. No response time, fix date or completeness guarantee is promised. This checklist is manual guidance; it does not run CI or authorize invasive security testing.
