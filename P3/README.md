## Practice 3(20)

**Object-oriented Programming**：The General Rankine Cycle Simulator 

Apply computational thinking to solve more complex problems

**Deadline:**  2019.05.19

## Contents and Requirements

Reference [PyRankine](https://github.com/PySEE/PyRankine), design a general energy balance software with Python to analysis the following cycles:

* [Example 8.1：An Ideal Regenerative Cycle](./rankine81.md)

* [Example 8.5：A Regenerative Cycle with Open Feedwater Heater](./rankine85.md)
 
* [Example 8.6：A Reheat–Regenerative Cycle with Two Feedwater Heaters](./rankine86.md) 

**注意**：练习不使用Jupyter Notebook；使用Visual Studio Code进行代码设计等工作，使用MS Word编写设计文档。

### 数据文件和Python3源码(12)

* 数据文件：建立描述循环系统和设备的json文件(2)

* Python3源码
 
   * 使用类描述循环中的设备(组件)、节点(5)

   * 编程读取系统描述json文件，解析其描述的循环系统，进行循环的能量平衡分析(4)

* 数据文件：输出分析结果到数据文件(1)
  
### 软件设计工作Word文档(8)

* 设计问题简要描述(1); 

* 程序设计方案简要描述(5)
  * 总体思路；   
  * 系统json文件描述；
  * 节点和设备类的设计；
  * 循环能量平衡计算过程；

* 设计工作小结(1)

* Word排版(1): 版面整洁，合理划分和组织文档段落；页眉：练习三 学号 姓名； 页脚：页码 

  * **无需** 封面和目录

## 提示

[Example 8.6：A Reheat–Regenerative Cycle with Two Feedwater Heaters](./rankine86.md) 比 `Example8.1，8.5`, 多了不同类型的设备(reheater, the closed feedwater heater, trap)。

需要在理解示例基础上，增加新设备类的json描述，计算分析Python类实现及相关代码，实现更通用的循环计算程序。

通用Rankine Cycle程序的泛化要点:

1.  设备

2.  设备间连接关系

3.  系统能量平衡计算方法

**Results for reference**

* Example 8.1: [rankine81-SP.txt](./rankine81-SP.txt)

* Example 8.5: [rankine85-SP.txt](./rankine85-SP.txt)

* Example 8.6: [rankine86-SP.txt](./rankine86-SP.txt)

**Download the ebook**

Michael J . Moran. Fundamentals of Engineering Thermodynamics (7th Edition).  John Wiley & Sons, Inc. 2011/(8th Edition) 2015

Please download the ebook from SEU: http://www.lib.seu.edu.cn/ （查找资源->外文电子书->Wiley电子教材->T(工业技术)->TK(能源与动力工程)->TK1(热力工程,热机)

## Directories and Files

```bash
 ├──<Practices>
     │ 
     |── <P3>
          │ 
          |── *.docx 设计工作Word文档
          |
          |── *.py  循环分析Python源码文件
          |
          |── <components> components包的源码文件
          │    |
          │    │ ── *.py
          │   
          |── <txtcycle> 各循环描述json文件
          │    |
          │    │ ── *.json
          │ 
          |── <output> 各循环分析结果文件
               |
               │ ── *.txt
``` 

## 提交：

* 1 电邮： cmh@seu.edu.cn
   * 主题：学号-姓名-3
   * 附件：工作目录压缩文件： **学号-姓名-3.zip**；

* 2 截至时间：2019.05.19
   * 截至时间后可补交，补交得分<=13. (2019.06.16)

* 3 改进更新：提交作业后可修改，修改截至时间：2019.06.16

## 参考资源：

* [PySEE/PyRankine: step4,step5](https://github.com/PySEE/PyRankine)

### PyThermo

* [RankineCycle OOP](http://nbviewer.ipython.org/github/PySEE/home/tree/S2019/notebook/Unit4-1-PyThermo-RankineCycle-OOP.ipynb)

* [RankineCycle General](http://nbviewer.ipython.org/github/PySEE/home/tree/S2019/notebook/Unit4-2-PyThermo-RankineCycle-General.ipynb)

* [Python: JSON](http://nbviewer.ipython.org/github/PySEE/home/tree/S2019/notebook/Unit4-3-PyThermo-Python-JSON.ipynb)

