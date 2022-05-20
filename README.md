
# study
https://paper.seebug.org/632/#_6
https://github.com/ConsenSys/smart-contract-best-practices


# 漏洞
## 算法上下溢出
以太坊虚拟机（EVM）为整数指定固定大小的数据类型。这意味着一个整型变量只能有一定范围的数字表示。A uint8例如，只能存储在范围[0,255]的数字。试图存储256到一个uint8将导致0。如果不注意，如果不选中用户输入并执行计算，导致数字超出存储它们的数据类型的范围，则可以利用Solidity中的变量。


预防技术
防止溢出漏洞的（当前）常规技术是使用或建立取代标准数学运算符的数学库; 加法，减法和乘法（划分被排除，因为它不会导致过量/不足流量，并且EVM将被0除法）。

OppenZepplin在构建和审计Ethereum社区可以利用的安全库方面做得非常出色。特别是，他们的SafeMath是一个参考或库，用来避免漏洞/溢出漏洞。






