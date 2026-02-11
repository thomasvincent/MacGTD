# CLAUDE.md

Getting Things Done automation workflows for 8 productivity platforms on macOS.

## Stack
- AppleScript (Automator workflows)
- Bash scripts
- Alfred workflow

## Validation
```bash
# AppleScript syntax
./tests/test_applescript_syntax.sh

# Automator bundle validation
./tests/test_automator_loading.sh

# Natural language parser tests
./tests/test_natural_language_parser.sh

# Full validation
./tests/validate_repo.sh
```

## E2E Testing
```bash
# Local Mac Mini
./infra/local/setup-local-runner.sh

# Trigger E2E
gh workflow run e2e.yml -f test_suite=all
```
