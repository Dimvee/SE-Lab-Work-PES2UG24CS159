
# Lab 5 – Static Code Analysis

| Issue | Type | Original Location | Description | Fix Approach |
|---|---|---|---|---|
| Unsafe XML parser | Security | Lines 3, 18 | XML parsing may allow XML attacks | Replaced ElementTree with defusedxml |
| Hardcoded password | Security | Line 13 | Password stored directly in source code | Removed unused hardcoded password |
| Shell command execution | Security | Line 63 | os.system() may allow command injection | Replaced with HTTPConnection and IP validation |
| Mutable default argument | Bug | Line 42 | Empty dictionary is shared across function calls | Changed {} to None |
| Invalid naming conventions | Code quality | Multiple lines | CamelCase names reduce readability | Changed names to snake_case |
| Missing docstrings | Code quality | Multiple lines | Functions lacked descriptions | Added docstrings |
| Unused argument | Code quality | Line 50 | currency was not used | Removed unused argument |
| Missing encoding | Code quality | Line 57 | File opened without explicit encoding | Added encoding="utf-8" |
| Formatting errors | Style | Lines 22, 44, 72, 76 | Blank lines, whitespace and line length problems | Corrected PEP 8 formatting |
