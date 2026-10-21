# pdx206-apt

Signed flat apt repository with the latest CI release of each package in
[`packages.list`](packages.list), for Droidian on the Sony Xperia 5 II (pdx206).
Rebuilt every 15 minutes (GitHub runs schedules late at times), on every push, and on `gh workflow run publish.yml -R panxiao81/pdx206-apt`.

`adaptation-sony-pdx206-extras` ships the source entry, the key and a pin of
1100, so these builds win over Droidian's (1002) and archiemeng's (1010):

```
deb [signed-by=/usr/share/keyrings/pdx206-apt.gpg] https://panxiao81.github.io/pdx206-apt ./
```

Key: `pdx206-apt.gpg`, fingerprint `A825 F324 7BE9 C38D 6B3E  95F4 612B 0C1A 1E10 5FC4`.
