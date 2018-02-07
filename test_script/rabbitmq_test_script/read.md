## 测试脚本的使用方法

- 在装饰器参数中加入需要测试的次数参数

```python
@test_nums(100)  # 测试100次
def test_topic_exchange(client, channel,name):
    client.topic_exchange(channel,name)
```

- 多线程测试

- 在test_threads函数中传递测试函数，线程数，函数参数。