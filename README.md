# log4shell-payloads
This repo is providing collected JAVA .class files which are dropped by log4shell exploit attempts.

## Disclamer
Do not use these for yourself. Educational purposes only!

**joke** you know what this is about :)

## Remove duplicates

```
comm -1 -2 \
  <(ls) | \
  <(md5sum * | \
    sort -k1 | \
    uniq -w 32 | \
    awk '{print $2}' | \
    sort) \
xargs rm
```

Replace MD5 with hash algo of whish to avoid hurting butt.
