# Changelog

### **v1.0.0** (Current)

+ 🆕 **新特性**: 新增 `deleteWithBody` 参数支持
  - DELETE 请求现在可以选择使用请求体或查询参数
  - 默认行为遵循 HTTP 标准（使用查询参数）
  - 设置 `deleteWithBody: true` 可启用请求体支持
  - 解决了原本的`fly`使用 DELETE 请求无法传递`body(payload)`的问题

+ 🐛 **Bug 修复**: 修复了 DELETE 请求的数据处理逻辑
  - 修复了 DELETE 请求时 data 被强制转为 query 参数的问题
  - 改进了参数合并逻辑，避免数据丢失

+ ✨ **改进**: 优化了多端兼容性
  - 更好的 HTTP 标准遵循
  - 保持了向后兼容性

