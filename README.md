Project I needed this for is temporarily archived, so this is too.

---

## Mappy String Line Diff

- simple string line diffing and diff application in javascript/typescript
- single ~25-line class, made as part of a different project, and npm'd for my convenience (and maybe someone else's?)
- no docs, just two functions `MSLDiff.diff(string1, string2)` and `MSLDiff.edit(originalString, diff)` and `MSLDiff.lineSeparator` can be set to change the line separator
- not made for performance but should be θ(n) time wise and θ(n) space wise for both functions, and it happens to also compress duplicate lines in diffs
- how does it work? look in `MSLDiff.ts`, it's called "Mappy" for a reason (it uses JS's Map)
- made in ~<10 minutes so it might break, but probably wouldn't

blobbybilb 2024, MIT License

---

Note to self & Possible TODO: Option to return generated map in diff() and pass it to edit(), and a list to generated base string from it, since storing that effectively compresses the base string similar to how it compresses duplicate lines in diffs.
