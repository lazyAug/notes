# Swift - 实现URL字符串的编码与解码（urlEncoded、urlDecoded）

我们的应用中常常需要发起 HTTP 网络请求，如果拼接的 URL 地址中包含有中文、空格、特殊符号时，我们就要对其转义。否则就会无法正确访问。

###  1. 扩展String，添加相关的转义方法

Swift3 新增的 addingPercentEncoding 方法实现了编码的功能，也就是将指定的字符集使用“%”代替。这里为方便使用，我们扩展 String，为其添加两个新方法：

- urlEncoded()：将原始的 url 编码为合法的 url
- urlDecoded()：将编码后的 url 转换回原始的 url

```swift
extension String {
    //将原始的url编码为合法的url
    func urlEncoded() -> String {
        let encodeUrlString = self.addingPercentEncoding(withAllowedCharacters:
            .urlQueryAllowed)
        return encodeUrlString ?? ""
    }
    //将编码后的url转换回原始的url
    func urlDecoded() -> String {
        return self.removingPercentEncoding ?? ""
    }
}
```

