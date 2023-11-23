# JavaScript学习笔记



## 1. JavaScript基本语法



### 1.1 变量声明和赋值

在JavaScript中，可以使用关键字 `var`、`let` 或 `const` 来声明变量。与C语言中的变量声明相似。

**例子：**
```javascript
// JavaScript
var message = "Hello, World!";
let count = 42;
const pi = 3.14;
```
```c
// C语言
#include <stdio.h>

int main() {
    char message[] = "Hello, World!";
    int count = 42;
    const float pi = 3.14;
    return 0;
}
```

### 1.2 条件语句

JavaScript中的条件语句与C语言类似，使用 `if`、`else if` 和 `else`。

**例子：**
```javascript
// JavaScript
let money = 25;

if (money > 39) {
    console.log("来杯星巴克！");
} else if (money > 20) {
    console.log("来杯瑞幸！");
} else {
    console.log("来杯幸运咖！");
}
```
```c
//c
#include<stdio.h>
int main()
{
	int money = 25;
	if (money > 39)
	{
		printf("来杯星巴克！");
	}
	else if (money > 20)
	{
		printf("来杯瑞幸！");
	}
	else
	{
		printf("来杯幸运咖！");
	}

	return 0;
}
```

## 2. JavaScript数据类型

### 2.1 字符串（String）

在JavaScript中，字符串是由字符组成的，与C语言中的字符数组相似。

**例子：**
```javascript
// JavaScript
let greeting = "Hello, World!";
console.log(greeting);
```
```c
// C语言
#include <stdio.h>

int main() {
    char greeting[] = "Hello, World!";
    printf("%s\n", greeting);
    return 0;
}
```

### 2.2 数字（Number）

JavaScript中的数字可以是整数或浮点数，与C语言中的整数和浮点数类似。

**例子：**
```javascript
// JavaScript
let integerNumber = 42;
let floatNumber = 3.14;
console.log(integerNumber, floatNumber);
```
```c
// C语言
#include <stdio.h>

int main() {
    int integerNumber = 42;
    float floatNumber = 3.14;
    printf("%d %f\n", integerNumber, floatNumber);
    return 0;
}
```

### 2.3 布尔（Boolean）

JavaScript中的布尔类型表示真（true）或假（false），类似于C语言中的布尔类型。

**例子：**
```javascript
// JavaScript
let isSunny = true;
let isRainy = false;
console.log(isSunny, isRainy);
```
```c
// C语言
#include <stdio.h>

int main() {
    int isSunny = 1;  // 1表示真
    int isRainy = 0;  // 0表示假
    printf("%d %d\n", isSunny, isRainy);
    return 0;
}
```

### 2.4 Null 和 Undefined

在JavaScript中，`null` 表示一个空值，`undefined` 表示一个未定义的值。与C语言中的 `NULL` 和未初始化变量类似。

**例子：**
```javascript
// JavaScript
let nullValue = null;
let undefinedValue;
console.log(nullValue, undefinedValue);
```
```c
// C语言
#include <stdio.h>

int main() {
    int* nullValue = NULL;
    int undefinedValue;  // 未初始化的值是不确定的
    printf("%p %d\n", nullValue, undefinedValue);
    return 0;
}
```

## 3. 对象（Object）

在JavaScript中，对象是键值对的集合，可以类比C语言中的结构体。

**例子：**
```javascript
// JavaScript
let Studen = {
    Name: "laimaxgg",
    sex:"male"
    age: 18
};
console.log(Studen.Name, Studen.sex, Studen.age);
```
```c
// C语言
#include <stdio.h>

struct Studen {
    char Name[20];
    char sex[20];
    int age;
};

int main() {
    struct Studen Studen1 = {"laimaxgg", "male", 18};
    printf("%s %s %d\n", Studen.Name, Studen.sex, Studen.age);
    return 0;
}
```

## 4. 数组（Array）

JavaScript中的数组可以包含不同类型的元素，类似于C语言中的数组。

**例子：**
```javascript
// JavaScript
let fruits = ["Apple", "Banana", "Orange"];
console.log(fruits[0], fruits[1], fruits[2]);
```
```c
//c
#include<stdio.h>
int main()
{
	char fruits[50] = { "Apple ""Banana ""Orange" };
	printf("%s", fruits);
	return 0;
}

```



##  5.HTML、CSS、JavaScript之间的关系
这三者协同工作，构成了现代web开发的基础，被广泛应用于创建丰富、动态且具有吸引力的网页。

HTML定义网页结构： 定义页面的基本结构，包括文本、图像、链接等，但并不涉及页面的样式和行为。

CSS定义网页样式： 通过选择器和规则，控制HTML元素的外观和布局，使页面更具吸引力并易于阅读。

JavaScript提供交互性： 使网页具有动态性，可以根据用户的行为实时更新内容，处理用户输入，以及与服务器进行通信。 JavaScript可以与HTML和CSS交互，实现更丰富的用户体验。