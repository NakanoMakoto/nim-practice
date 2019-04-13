# 識別子等

## リテラルについて
String　文字列はダブルクォートで囲まれる  
特殊文字エスケープは \ で行える  


```
r"C:\program files\nim"
```

複数行に渡って文字列を入力する場合は以下  
この場合はバックスラッシュもエスケープ文字とならない  
HTMLコードの埋め込みなどに有効
```
""" ... """;
```

## コメント

コメントは#で  
ドキュメントは## で始まる

```
# A comment.

var myVariable: int ## a documentation comment
```

複数行に渡るコメントはこのように囲む #[ and terminated with ]#.  
これらはネストする必要がある。

```
#[
You can have any Nim code text commented
out inside this with no indentation restrictions.
      yes("May I ask a pointless question?")
  #[
     Note: these can be nested!!
  ]#
]#
```

ブロックコメント用にdiscord句が使える
```
discard """ You can have any Nim code text commented
out inside this with no indentation restrictions.
      yes("May I ask a pointless question?") """
```

## 数字

数字は可読性の為にアンダースコアが使用できる
```
1_000_000
```

小数点や'e' や 'E' が含まれるものは浮動小数点型になる
```
1.0e9
```

16進数は0x、2進数は0b、8進数は0oがそれぞれ先頭に付く。  
先頭に0を付けたとしても、8進数には出来ない。