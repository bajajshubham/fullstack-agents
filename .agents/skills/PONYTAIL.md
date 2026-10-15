# Skill: Ponytail (Senior Dev Parsimony)

## Principle
Write only what the task strictly needs. Lazy means efficient, not careless.

## The Decision Ladder (Check in strict order before writing code)
1. Does this feature need to exist? If not, skip it (YAGNI).
2. Is it already in the repository? Reuse it, do not rewrite.
3. Does the language standard library do it? Use standard library.
4. Does the native browser/platform support it natively? (e.g. `<input type="date">` instead of a 300-line picker).
5. Does an already installed package handle it? Use it.
6. Can this logic be expressed in 1 to 3 clean lines? Keep it minimal.
7. Only write new custom code if steps 1 to 6 fail.

*Note:* Never cut validation, data sanitisation, error handling, or security to save lines.
