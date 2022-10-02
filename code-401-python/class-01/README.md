# Big O notation
**Big O notation** is a particular tool for assessing algorithm efficiency. Big O notation is often used to show how programs need resources relative to their input size.
![O notation](https://miro.medium.com/max/1200/1*HwLR-DKk0lYNEMpkH475kg.png)

**Common types of Big-O notations are:**

* O(1) — Constant time complexity

Execution time of constant time algorithm is independent of the size of input and will always take constant time for execution
![constant type](https://miro.medium.com/max/720/1*cW276oHDXDZUfFr6C-58WA.png)
* O(n) — Linear time complexity

Execution time of linear time algorithm is proportional to the input size (n). Examples include: traversing an array, a linked list; linear search; comparison of two strings, palindrome check, bucket sort, and etc.

![Linear](https://miro.medium.com/max/640/1*LICcHh0dtM-JgRJNN5xmog.png)
* O(n²) — Quadratic time complexity

Execution time of quadratic time algorithm is proportional to the input size (n²). Examples include nested loop, bubble sort, insertion sort, selection sort, and etc.

![Quadratic](https://miro.medium.com/max/720/1*BT8W5Uv48Ukd50saIQ1KdQ.png)

* O(log n) — Logarithmic complexity

Execution time of logarithmic time algorithm is proportional to the input size (log n). Examples include simplified loop version of binary search algorithm.

![Logarithmic](https://miro.medium.com/max/640/1*FvZ77-nfpc7YOm3VIfdHDg.png)

____

# Names and Values in Python
* Many names can refer to one value.
* Names are reassigned independently of other names.
* Values live until nothing references them.
*  Assignment never copies data.
*  Changes in a value are visible through all of its names. (Mutable Presto-Chango)
* Python passes function arguments by assigning to them.
*  Values can’t be deleted, only names can.
*  Names have no type, values have no scope.


# Things I need to know about more

## Referances:
1.  [O notation for beginner](https://medium.com/@changminlim/big-o-notation-for-beginners-ae17e8f70414#:~:text=Common%20types%20of%20Big-O%20notations%20are%3A%20O%20%281%29,computers%20have%20to%20use%20in%20order%20to%20execute.)
2. [A friendly intro to Big O Notation](https://www.codenewbie.org/basecs/8)
3. [Facts and myths about Python names and values video](https://www.youtube.com/watch?v=_AEJHKGk9ns)
4. [Facts and myths about Python names and values](https://nedbatchelder.com/text/names.html)