---
description: API
---

# 常用的API使用模版

### Create a LinkedList

```
class ListNode {
    constructor(data) {
        this.data = data
        this.next = null                
    }
}

class LinkedList {
    constructor(head = null) {
        this.head = head
    }
    size() {
        let count = 0; 
        let node = this.head;
        while (node) {
            count++;
            node = node.next
        }
        return count;
    }
    clear() {
        this.head = null;
    }
    getLast() {
        let lastNode = this.head;
        if (lastNode) {
            while (lastNode.next) {
                lastNode = lastNode.next
            }
        }
        return lastNode
    }
    getFirst() {
        return this.head;
    }
}

let node1 = new ListNode(2)
let node2 = new ListNode(5)
node1.next = node2;
```

### Create TreeNode

```
//treeNode 创建方法
function TreeNode(val, left, right) {
   this.val = (val===undefined ? 0 : val)
   this.left = (left===undefined ? null : left)
   this.right = (right===undefined ? null : right)
}
or:
class Node {
    constructor(val, leftChild, rightChild) {
        this.val = val;
        this.leftChild = leftChild;
        this.rightChild = rightChild;
    }
}
```

### Map的几种写法

<pre><code>//1.1 map用{}
let map = {};//临时储存位
map[key] = value; //存入
if (tmp in map) 检查

<strong>//ex, s is String:
</strong>let map = {};  
for (let char of s) {
    map[char] ? map[char]++ : map[char] = 1;
}
Object.entries(map)
const res = Object.keys(map).sort((a, b) => map[b]- map[a]);

let result = Object.keys(hash).sort((a,b)=>{
    let countCompare = hash[b] - hash[a];
    if (countCompare == 0) return a.localeCompare(b);
    else return countCompare;
}   
);

//1.2 用new Map()
//ex:
let map = new Map();
map.set(p[i], (map.get(p[i]) || 0) + 1);
map.get(s[i]);
map.set(s[right], (map.get(s[right]) || 0) - 1);
for (const [key, value] of map1)
for (const value of map1.values())
for (const key of map1.keys())
let arr = Array.from(map.entries()).sort((a,b) => {
    return a[1] === b[1] ? a[0].localeCompare(b[0]) : b[1]-a[1];
})
</code></pre>

### set的变种用法

```
//用array存
const set = new Array(256);
set[s.charAt(start)] = false;
```

### String的常用API

```
s.charAt(i);
s[i];
```

### &#x20;number overflow

```
Math.pow(2, 31)
```

### &#x20;

##

二分法
