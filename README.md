# free-proxy-list.net API

Get a list of free proxies from [free-proxy-list.net](https://free-proxy-list.net/) to use in your Python3 requests!

## Usage

Follow the example

```python3
proxies = get_proxy_list()

print(proxies[0])

#  Proxy IP       Port  Code  Country Name     Anonymity    Google  HTTPS  Last Check
# ['192.168.0.1', '80', 'US', 'United States', 'anonymous', 'no',   'no',  '5 secs ago']
```
set `show_msg` to False to supress output

set `http_mode` with the following:
- "all": both http and http proxies
- "http": just get http proxies
- "https": just get https proxies
```python3
proxies = get_proxy_list(show_msg=False, http_mode="https")
# No output and just https proxies
```
