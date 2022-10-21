# Obfuscator-LLVM

此处介绍，可以用于iOS代码混淆的工具：`Obfuscator-LLVM`

* `Obfuscator-LLVM` = `ollvm`
  * 是什么：基于LLVM的**代码混淆工具**
  * 谁开发的：瑞士伊夫尔东莱班的应用科学与艺术大学信息安全小组
  * 什么时候：2010年6月
  * 目的：增强软件代码安全
    * 基于LLVM的编译套件
    * 通过防篡改(tamper-proofing)和代码混淆(code obfuscation)
  * 支持语言
    * `C`, `C++`, `Objective-C`, `Ada`和`Fortran`
  * 支持架构
    * `x86`, `x86-64`, `PowerPC`, `PowerPC-64`, `ARM`, `Thumb`, `SPARC`, `Alpha`, `CellSPU`, `MIPS`, `MSP430`, `SystemZ`和`XCore`
  * 代码混淆方式
    * `control flow flattening`=`控制流扁平化`=`控制流平坦化`
      * 语法：`-mllvm -fla`
    * `instruction substitution`=`指令替换`
      * 语法：`-mllvm -sub`
    * `bogus control flow`=`控制流伪造`=`虚假控制流程`
      * 语法：`-mllvm -bcf`
  * 资料
    * GitHub
      * obfuscator-llvm/obfuscator
        * https://github.com/obfuscator-llvm/obfuscator
      * 文档入口
        * Home · obfuscator-llvm/obfuscator Wiki
          * https://github.com/obfuscator-llvm/obfuscator/wiki
      * 快速上手
        * obfuscator/GettingStarted.rst at llvm-4.0 · obfuscator-llvm/obfuscator
          * https://github.com/obfuscator-llvm/obfuscator/blob/llvm-4.0/docs/GettingStarted.rst
