RFC16 - Standardize Dict
========================

- 提出时间: 2019-04-20
- 当前状态: 已采纳

## Motivation
Scope 作为一等公民, 需要允许被嵌入字典中.

## Design

```arc
a: {
	(b)
	c : 0
	<d>
	& [1, 2, 3]
}
```

等价于:

```arc
(a/b)
c : 0
<a/d>
& [1, 2, 3]
```
