# 运行一个全数据节点

## 快速开始

### 步骤 1: 从源代码构建 `geneth`

请确认已经安装 Go 1.13 或以上版本，然后运行

```bash
# Clone the geneth repo
git clone https://github.com/genechain-io/geneth
# Enter the folder containing geneth source
cd geneth
# Compile
make geneth
```

### 步骤 2: 运行 `geneth` 来启动一个全数据节点

#### 主网 Genenet

主网 genenet 目前以上线。运行一个主网全数据节点，只需简单运行

```bash
build/bin/geneth console
```

这会启动一个连接到主网 genenet 的 `geneth` 客户端。

#### 测试网 Adenine

运行一个全数据的 Adenine 测试网节点，可以通过添加 `--adenine` 参数来完成

```bash
build/bin/geneth --adenine console
```

这会启动一个连接到主网 Adenine 的 `geneth` 客户端。

## 全数据节点优势

* 完整的区块链数据都存储在磁盘上
* 提供 RPC 服务
* 验证新的区块和交易数据
* 验证账户或者合约的状态

## Sync 模式

Sync 模式可以通过修改 `--syncmode "<模式>"` 参数达成，其中 `<模式>` 可以为：

* Full: 下载所有区块数据（包含区块头，交易，和收据）并通过执行每一个区块的数据来增量生成区块链状态数据。
* Fast \(默认\): 下载所有区块数据（包含区块头，交易，和收据），验证所有的区块头，根据区块头下载并验证区块量状态数据。
* Light: 下载所有区块数据（包含区块头，交易，和收据），随机验证。

