1. 从生命周期中可以看到在mounted之前会由一个Watcher去代理执行渲染函数

2. Watcher会先将自己作为全局Dep.target的变量，当响应式数据被访问时就会将其添加到自己的Dep框中

3. 当响应式数据发生改变的时候，会由Watcher去代理执行_update(_render())方法，将VNode给patch到真实DOM上