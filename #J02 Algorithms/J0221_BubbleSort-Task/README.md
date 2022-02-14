# Bubble sort 冒泡排序法

前置知識：[#for...loop]()、[#swap]()

## Explain

冒泡排序是反覆進行「由右往左，將相鄰的數兩兩相比後重新排列」的操作。因為數由右往左移動時，很像水中的氣泡浮起來的樣子，因而得名(亦稱泡沫排序、氣泡排序)。

## Code

###### 助記碼
```
i∈[0,N-1)               //循环N-1遍
   j∈[0,N-1-i)           //每遍循环要处理的无序部分
     swap(j,j+1)          //两两排序（升序/降序）
```

###### 虛擬碼
```
function bubble_sort (array, length) {
    var i, j;
    for(i from 0 to length-1) {
        for(j from 0 to length-1-i) {
            if (array[j] > array[j+1])
                swap(array[j], array[j+1])
        }
    }
}
```

###### 實作範例

|程式語言|目標                         |狀態  |
|:-----:|:---------------------------|:----:|
|C      |[Bubble sort for C](https://github.com/WaylonYuen/learn-c-basic/tree/Master/%23J02%20Algorithms/%23J0221_BubbleSort-Solved)       |Solved  |
<!-- |C++    |[Bubble sort for C++]()     |Task  |
|C#     |[Bubble sort for C#]()      |Task  |
|Java   |[Bubble sort for Java]()    |Task  |
|Python |[Bubble sort for Python]()  |Task  | -->
