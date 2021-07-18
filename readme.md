# RPC 文档问题

## 样例

部分样例在主网下无法运行，现在大部分无法运行的已经更改为可运行的版本了，但目前仍有部分样例无法运行 / 样例意义较小, 之后需要再进行构造

- `cfx_call` 当前样例无法运行
- `cfx_getDepositList` `cfx_getVoteList` 当前样例只会返回空值
- `getLogs` 参数的 `topics` 字段当前置空

## 文档部分内容出错/遗漏

- clientVersion 返回参数类型应为 string 而不是DATA
- `cfx_getBlockByHash` 等 返回的 Block 对象中缺少 custom 字段
- estimate 接口返回的对象中包含 gasLimit 字段

## 文档缺失报错部分内容

现在缺少报错的错误码相关说明

例如 `cfx_getCode` `cfx_call` `cfx_getLogs` `estimate` 等
