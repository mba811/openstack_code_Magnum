### service.py
提供 prepare_service 方法，加载 Magnum 项目的配置信息，在 API 初始化的过程中被调用。
```python
def prepare_service(argv=[]):
    cfg.CONF(argv[1:], project='magnum')
    logging.setup(cfg.CONF, 'magnum')
```
