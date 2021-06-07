# 验证人指南

想要成为一个验证人，你首先需要运行一个挖矿\(mining\)模式的节点，并且这个节点绑定了已解锁的挖矿账户。然后将改账户注册\(register\)成为验证候选人。注册之后，你需要获得足够的质押权中来成为活跃节点或者进入头部候选人列表。

本文内容覆盖了前两个步骤，[质押挖矿](../user-manual/staking.md)页面讲解了最后一个步骤，你可以在该页面了解质押权重的计算方式。如果你想了解更多关于 GeneChain 共识验证机制，可以参考 [Ribose 共识机制](../for-developers/ribose-consensus-protocol.md)一文。

## 以挖矿模式运行节点

### 步骤 1: 创建挖矿账户

开始挖矿之前需要创建一个挖矿账户，该账户默认被用来生产区块并获取挖矿奖励，你之后也可以设置一个不同的账户来收取挖矿奖励。

你可以导入一个已经存在的账户，通过如下方式：

```bash
build/bin/geneth account import <path/to/private_key_file>
```

或者生成一个新的账户，通过运行：

```bash
build/bin/geneth account new
```

### 步骤 2: 启动一个挖矿模式的节点

挖矿模式可以通过执行 `geneth` 客户端时使用 `--mine` 和 `--unlock` 标识。请记得 `--unlock` 标记中使用在步骤1中提到的账户地址。

```bash
# For mainnet
build/bin/geneth --mine --unlock <your_miner_account>

# For Adenine testnet
build/bin/geneth --adenine --mine --unlock <your_miner_account>
```

请记得输入密码来解锁账户。你也可以通过`--password`标识来制定一个密码文件来解锁。

现在，当你的节点追上最新的区块数据之后，你就有了一个准备好生产区块的节点了。下一步骤就是注册你的挖矿账户为验证人候选节点来接受质押。

## 注册成为验证候选人

验证人注册是通过调用 Ribose 系统合约的 `register` 方法来完成的。你可以在合约的[源代码](https://github.com/genechain-io/system-contract/blob/master/contracts/Ribose.sol)了解到更多的信息。你可以通过 web3 客户端或者[区块链浏览器页面](https://scan.genechain.io/address/0x0000000000000000000000000000000000001000/write-contract)来完成注册。

**注意:** 你需要用挖矿账户来调用`register`方法，因为抵用账户会被注册为候选人。

## 其他

### 设置区块奖励领取账户

为了更好的保护挖矿账户，我们强烈建议你设置一个其他账户作为区块奖励收取人。

`setProfitTaker` 可以用来设置区块奖励收取人.

**注意:** 只有当前的区块奖励收取人可以调用该方法，其他任何人都无法修改，甚至包括挖矿账号。

### 提取矿工奖励

区块奖励首先会被分配到矿工的待定收益\(pending profit\)中，待定收益可能会因不端行为被罚没。

每 86400 个区块，约 72 小时，待定收益的一半会被结算，被结算收益可以提取，结算后会记录最后一次结算的区块号，直到下一个86400区块才能再次结算。

矿工每生成一个区块，都会尝试自动结算待定收益到可领取收益，在领取收益的时候也会尝试进行结算。

`getCandidateState` 可以用来查询待结算和可结算的数量详情。

`withdrawMinerProfits` 可以用来领取已结算收益。

