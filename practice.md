## 任务描述
在两行中分别输入一个字符串s和一个整数n，定义一个函数将字符串s循环移动n位。其中，n为正数时，循环向右移动n位；n为负数时，循环向左移动n位。
若s为空字符串，则不论n为多少，均输出空字符串。


        def f(s,n):
        if s == "":
            return ""
        l = len(s)
        k = n % l
        return s[-k:] + s[:-k]
    s=input()
    n=int(input())
    print(f(s,n))

