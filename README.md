# nocoredump

nocoredump是一个可用于捕捉程序中出现严重的错误的程序,它能够捕捉到如下引起程序崩溃的严重bug,同时能够跳过出问题的程序,继续运行程序。同时在出问题的地方会打印出问题堆栈帮助调试:
    
    信号      值       动作      说明
    SIGILL    4       Core	    非法指令(程序错误、试图执行数据段、栈溢出等)
    SIGFPE    8	      Core	    算术运行错误(浮点运算错误、除数为零等)
    SIGSEGV	  11      Core     无效内存引用(试图访问不属于自己的内存空间、对只读内存空间进行写操作)