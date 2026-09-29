# Linux Cybersecurity Labs

Hands-on Linux practice and cybersecurity lab exercises.

## Day 1 — Linux Command-Line & Log Analysis

### Topics Practiced

- Linux directory navigation
- File and directory management
- Viewing file contents
- Text searching with `grep`
- Pipes (`|`)
- Output redirection (`>` and `>>`)
- Basic log analysis

### Commands Practiced

```bash
pwd
cd ..
mkdir
cd
touch
cat
echo
ls -a
grep -i
tail

### Log Analysis Exercise

Used `grep` to identify failed login entries from a log file:

```bash
grep -i "failed" security.log
```

Counted the failed-login entries:

```bash
grep -i "failed" security.log | wc -l
```

Displayed the 10 most recent matching entries:

```bash
grep -i "failed" security.log | tail
```

Saved the matching entries into a separate file:

```bash
grep -i "failed" security.log > failed.log
```

## Learning Goal

Build practical Linux and cybersecurity skills through hands-on exercises and document my progress.
