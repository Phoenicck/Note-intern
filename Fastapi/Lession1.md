1. 同步与异步

​	i. 原生支持异步

​	ii. 自动生成一个可交互式的文档

​	iii. --reload 自动重启 修改完代码

```
@app.get("/author/{name}")
async def get_author(name:str = Path(...,min_length=2,max_length=10)):
    return {"message": f"The author name is {name}"}
```

3. 
