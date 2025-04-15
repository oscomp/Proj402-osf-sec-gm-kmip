### 项目名称
基于国密标准的KMIP协议客户端实现  

### 导师信息
霍文，huowen@ieisystem.com  

### 难度
高  

### 分类
信息安全/密码管理  

### 题目要求：  
- 使用 C/C++11 及以上标准开发，完整实现符合国密标准的 KMIP 协议客户端；  
- 遵循以下标准：  
  - GM/T 0110-2021《密钥管理互操作协议规范》  
  - OASIS KMIP V1.4 标准协议规范；  
- 实现密钥全生命周期管理功能，包括密钥生成、存储、检索、销毁、属性设置与获取、归档与恢复等；  
- 协议编码格式支持 TTLV、JSON、XML；  
- 客户端需以动态库（.so）、静态库（.a）形式输出，提供命令行测试工具；  
- 支持在 Linux 平台编译运行，并提供 gtest 自动化测试用例；  
- 兼容主流开源 KMIP 服务端（如 PyKMIP），完成互操作性测试；  
- 性能指标建议：单连接每秒支持处理 100+ 次请求；  

### 特征：  
- 编程语言：C/C++  
- 输出形式：动态库、静态库、测试命令行工具  
- 标准支持：KMIP 1.4、GM/T 0110-2021  
- 编码格式支持：TTLV / JSON / XML  
- 适配 Linux 平台，支持自动化测试框架（gtest）  
- 高性能设计，支持大并发、低延迟请求处理  

### 预期目标：  
- 实现 KMIP 协议核心编码解码模块，能正确解析/构造 GM/T 0110 报文；  
- 支持 SM2、SM3、SM4 等国密算法的密钥管理操作：  
  - `Create`、`Get`、`Locate`、`Destroy`、`Archive`、`Recover`、`Set/Get_Attributes` 等；  
- 提供完整的接口文档（API手册）、测试工具及编译指南；  
- 提供与开源 KMIP 服务端互操作性验证文档；  
- 提交完整源码（包含 include/src/test/tools 等目录结构）与使用说明文档；  

### License
Apache-2.0  

### 参考资料  
1. GM/T 0110-2021标准文本  
2. KMIP 1.4规范：http://docs.oasis-open.org/kmip/spec/v1.4/os/kmip-spec-v1.4-os.html  
3. 参考实现 PyKMIP：https://github.com/OpenKMIP/PyKMIP  
