JAVA VIRTUAL MACHINE: - Java Virtual Machine (JVM) is an engine that provides a runtime environment in which byte code can be executed. JVM is the heart of the 
entire JAVA program execution process. JVM is a part of the Java Runtime Environment (JRE). JVM is platform-dependent. It is responsible for taking .class file 
& converting each byte code instruction into the machine language instruction that can be executed by the microprocessor.

What JVM does-
1.	Loads the code.
2.	Verify the code.
3.	Execute the code.
4.	Provide runtime environment.

Steps Undertaken by JVM-
1.	First of all, it loads .class file into memory.
2.	Then it verifies whether the all-byte code instructions are proper or not. If find any instruction suspicious, the execution is rejected immediately.
3.	If the byte code instruction is proper, then it allocates the necessary memory to execute the program.
   
The architecture of JVM: - JVM architecture contains a class loader, memory area, execution engine, etc.
![image](https://github.com/akhilkumar2020/Java-Introduction/assets/142902709/ede97fc3-e13c-4216-a5e2-1662a148f278)

	Class loader: - Class loader is a subsystem of JVM that is used to load class files. Whenever we run the Java program, it is loaded first by the Classloader. 
There are three built-in Class loaders in Java.

1.	Bootstrap Class loader: This is the first-Class loader which is the superclass of the Extension Class loader. It loads the rt.jar file which contains all
                            class files of Java Standard Edition like java. lang package classes, and java. util package classes, java.io package classes,
  	                         java.sql package classes, etc.
  	
3.	Extension Class loader: This is the child Class loader of Bootstrap and parent Class loader of System Class loader. It loads the jar files located inside
                            the $JAVA_HOME/JRE/lib/ext. directory.
  	
5.	System/Application Class loader: This is the child Class loader of the Extension Class loader. It loads the class files from the classpath. By default,
                                      the classpath is set to the current directory. It is also known as an Application Class loader.

	Class (Method) area: - Method is the memory block, which stores the class code, code of the variable, and code of the method in the Java programs.

	Heap: - It is the runtime data area in which objects are allocated.
	Stack: - Java Stacks are the memory area where the Java methods are executed. While executing the method, a separate frame will be created in the Java stack.
           A frame is destroyed when its method invocation is complete.

	Program Counter Register: - The PC (program counter) register contains the address of the Java virtual machine instruction currently being executed.

	Native method stack: - It contains all the native methods used in the application.

	Execution Engine: - It contains:
1.	A virtual processor
2.	Interpreter: Read bytecode stream then execute the instructions.
3.	Just-In-Time (JIT) compiler: It is used to improve performance. 

	Java native interface: -	Java Native Interface (JNI) is a framework that provides an interface to communicate with another application written in another 
                            language like C, C++, Assembly, etc
