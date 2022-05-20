
# study
https://paper.seebug.org/632/#_6
https://github.com/ConsenSys/smart-contract-best-practices


# 漏洞
## 算法上下溢出
以太坊虚拟机（EVM）为整数指定固定大小的数据类型。这意味着一个整型变量只能有一定范围的数字表示。A uint8例如，只能存储在范围[0,255]的数字。试图存储256到一个uint8将导致0。如果不注意，如果不选中用户输入并执行计算，导致数字超出存储它们的数据类型的范围，则可以利用Solidity中的变量。









