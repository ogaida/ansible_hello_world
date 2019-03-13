# Komplettes Matching mit optionalem String

Die regex soll alle Zeilen finden in denen nur "Oliver" oder "Oliver Gaida" steht. Hier die Lösung:

Naheliegend und gut lesbar ist:

```regex
^(Oliver|Oliver Gaida)$
```

Interessanter ist die folgende Variant, die dann auch Sinn macht wenn die Strings länger werden:

```regex
^Oliver(?m: Gaida)?$
```

Die Erläuterungen dazu kann man sich auf [regex101](https://regex101.com/) anschauen.

[HOME]./index.html