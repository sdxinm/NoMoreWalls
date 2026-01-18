# 配置片段

这里存放了一些从 `list.meta.yml` 中拆分出的配置片段，用于将本项目提供的一些配置整合到其它配置中。

# 文件说明

## Proxy Providers 规则集

- [nodes.meta.yml](./nodes.meta.yml)：适用于 Meta (mihomo) 内核的节点列表。
- [nodes.yml](./nodes.yml)：适用于原版 Clash 内核的节点列表，注意**不要**和下文的 `proxy.yml` 搞混了。
- nodes_地区码.meta.yml：相应地区的节点列表，根据名称识别，不保证准确性，也不保证使用第三方服务时是否会被判断为国区。对于原版 Clash 内核 (不推荐)，请去掉 `.meta`。
<!-- - [nodes_redir.yml](./nodes_redir.yml)：在多个地区中转的节点列表，其余同上。 -->

## Rule Providers 规则集

- [adblock.yml](./adblock.yml)：广告屏蔽域名列表。
- [proxy.yml](./proxy.yml)：需要走代理的域名列表。
- [direct.yml](./direct.yml)：需要直连的域名列表。
- [region.yml](./region.yml)：存在锁区的域名列表。

注意：广告拦截列表中的域名不会出现在需要走代理的域名列表中，因此即使您没有使用广告屏蔽规则，仍有一些广告会无法加载。

# 配置示例

见 [example.yml](./example.yml)。

# 加速链接（以 Meta 节点列表为例）

- 原始链接: `https://raw.githubusercontent.com/peasoft/NoMoreWalls/master/snippets/nodes.meta.yml`
- GhProxy.net: `https://ghproxy.net/https://raw.githubusercontent.com/peasoft/NoMoreWalls/master/snippets/nodes.meta.yml`
- 此处不公开部分私有镜像站

以下链接可能不是最新，但绝对不会被封：
- JsDelivr 默认 (当前 Fastly)：`https://cdn.jsdelivr.net/gh/peasoft/NoMoreWalls@master/snippets/nodes.meta.yml`
- JsDelivr Fastly CDN: `https://fastly.jsdelivr.net/gh/peasoft/NoMoreWalls@master/snippets/nodes.meta.yml`
- JsDelivr Cloudflare CDN: `https://testingcf.jsdelivr.net/gh/peasoft/NoMoreWalls@master/snippets/nodes.meta.yml`
- JsDelivr GCore CDN: `https://gcore.jsdelivr.net/gh/peasoft/NoMoreWalls@master/snippets/nodes.meta.yml`
