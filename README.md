### 记录

1. sass 变量作用域

```css
$wdith: 100px;

.box {
    /* 编译后width为100px */
    width: $width;
    $wdith: 500px;
    /* 编译后height为500px */
    height: $width;
}

/* 如果是less，上面的width与height都为500px */
```

2. 单位不用之间的运算

### less 与 saa 的区别

1. sass 支持属性嵌套，less 不支持
2. less 属性相同且值也形同的话会自动保留一个，sass 没哟这个功能
3. sass 不能转 20xp / 3 这种格式的值，less 支持，需要保持 20px/2 这样的形式的值，需要通过~"20px/2"
4. sass 相对比较严谨，不同单位不能进行运算，less 比较灵活，less 可以，以第一个主要单位作为单位进性操作

5. sass 默认 / 为分隔符，不会进行运算，如果需要进行运算，可以用小括号括起来
6. sass 没有命名空间，less 才有
