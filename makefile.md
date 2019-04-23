参考资料https://www.cnblogs.com/wang_yb/p/3990952.html  </br>
参考资料http://bbs.chinaunix.net/forum.php?mod=viewthread&tid=408225
## Makefile文件是什么
要想成为一个专业人士，那必须学会makefile来组织大型project,makefile关系到了整个工程的编译规则</br>
无论是C、C++、还是pas，首先要把源文件编译成中间代码文件，在Windows下也就是 .obj 文件，UNIX下是 .o 文件，即 Object File，这个动作叫做编译（compile）。然后再把大量的Object File合成执行文件，这个动作叫作链接（link）。</br>
链接时，主要是链接函数和全局变量，所以，我们可以使用这些中间目标文件（O文件或是OBJ文件）来链接我们的应用程序。链接器并不管函数所在的源文件，只管函数的中间目标文件（Object File），在大多数时候，由于源文件太多，编译生成的中间目标文件太多，而在链接时需要明显地指出中间目标文件名，这对于编译很不方便，所以，我们要给中间目标文件打个包，在Windows下这种包叫“库文件”（Library File)，也就是 .lib 文件，在UNIX下，是Archive File，也就是 .a 文件。</br>
源文件首先会生成中间目标文件，再由中间目标文件生成执行文件。

