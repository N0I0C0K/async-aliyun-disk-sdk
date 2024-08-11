# Async AliyunDisk SDK

这是一个 async python 版本的阿里云盘 API 封装，原[官方文档](https://www.yuque.com/aliyundrive/zpfszx)

使用 **pydantic + aiohttp**

## Usage

```python
from aliyun import init_aliyun_api, get_file_list, login_use_redirect

async def main():
    init_aliyun_api(YOUR_CLIENT_ID, YOUR_CLIENT_SECRET)

    # login here
    access_token = ...
    files = await get_file_list(acess_token, parent_file_id='root')
    print(files)
```

## Doc

建议查看官方文档，如需此 SDK 的使用文档，请在 issue 提出