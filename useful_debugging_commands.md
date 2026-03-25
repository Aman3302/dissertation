# Commands for debugging Latex Output

## Undefined References
After compiling, use this to parse out a list of any undefined refernces

```bash
grep "undefined" main.log | grep -oP "(?<=\`)[^']*" | sort -u
```
