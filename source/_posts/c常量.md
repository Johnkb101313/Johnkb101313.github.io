---
title: c常量
date: 2023-12-14 13:43:12
tags: c 語言
---

# C 語言中的常量種類

## 1.字面常量 (Literal Constants)

示例:
```c
int main()
{
    // 以下語法是錯誤的, 這樣寫只是為了方便展示
    3.14 // float
    10 // int
    'a' // char
    "Hello world" // char arr[12]
    10L // long
}
```

## 2.const 修飾的常變量

示例:
```c
int main()
{
    const int num = 100; // 使用了 const 修飾符的變量 num
}
```

## 3.符號常量
符號常量實際是預處理指令
只是在預處理階段進行文本替換
```c
#define NUM 100

int main()
{
    int n = NUM; // 預處理階段 NUM 會被替換成 100 即為字面常量, datatype為int
}
```
