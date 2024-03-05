An object that may hold resources (such as file or socket handles) until it is closed. The close() method of an AutoCloseable object is called automatically when exiting a try-with-resources block for which the object has been declared in the resource specification header.</br>
This construction ensures prompt release, avoiding resource exhaustion exceptions and errors that may otherwise occur.</br>
使用try-with-resources结构代替try finally结构。实现了关闭接口会自动调用这个方法释放资源
