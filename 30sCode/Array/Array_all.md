# Array all

校验数组中所有元素是否满足指定条件

## Concept

Returns `true` if the provided predicate function returns `true` for all elements in a collection, `false` otherwise.

Use `Array.prototype.every()` to test if all elements in the collection return `true` based on `fn`. Omit the second argument, `fn`, to use `Boolean` as a default.

如果集合中所有元素都满足所给出的判断条件则返回 `true`，否则返回 `false`。

使用 `Array.prototype.every()` 去测试，如果每个元素，省略第二个参数，即省略函数 `fn`，则使用布尔值作为默认条件

## Code

``` js
const all = (arr, fn = Boolean) => arr.every(fn);
```

## Example

``` js
all([4, 2, 3], x => x > 1); // true
all([1, 2, 3]); // true
all([1, 2, true]); // true
all([1, 2, false]); // false
```

## Application