# **DFS**
```
'''用栈实现'''
def DFS(root):
    if root == None:
        return None
    stack = []
    stack.append(root)
    while(stack):
        node = stack.pop()
        print(node.val)
        if(node.right):
            stack.append(node.right)
        if(node.left):
            stack.append(node.left)
```
# **BFS**
```
'''用队列实现'''
def BFS(root):
    if root == None:
        return None
    queue = []
    queue.append(root)
    while(queue):
        node = queue.pop(0)
        print(node.val)
        if(node.left):
            queue.append(node.left)
        if(node.right):
            queue.append(node.right)
```