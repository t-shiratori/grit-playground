---
tags: [optional, tags, here]
---
# Console.log message foo to bar

console.log()のメッセージを"foo"を"bar"に書き換えます。

```grit
`console.log('$message')` => `console.log('bar')` where {
    $message <: "foo"
 }
```

## テストケース

入力用のコードを書きます。

```typescript
console.log('hello');
console.log('foo');
```

期待するアウトプットのコードを書きます。

```typescript
console.log('hello');
console.log('bar');
```

