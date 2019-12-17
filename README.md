# Generator
生成器：1.  代码生成器；2. 文件生成器。


安装好jdk之后，如下步骤：
1.首先打开src目录Generator.java，修改
`public static void main(String[] args){
		generateCode("/Users/junlv/Documents/cccProjects/YouPlayILearn/client/BabySoeasy/build/jsb-link/subpackages/", 50);
	}`
  
  
2.执行：
`javac /Users/junlv/Documents/Library/Generator/CodeGenerator/src/com/generator/Generator.java`

3.将生成的.class文件，拷贝到bin目录下generator文件夹中;

4.执行:
`java com.generator.Generator`
则会在对应目录生成一些列.h / .m文件

5.在项目中合适的位置导入：
`#include "../../../subpackages/InitCaller.h"` (比如我这里添加在Classes/AppDelegate.h头文件中)
