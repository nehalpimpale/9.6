# 9.6

Q1.Explain about the different complex data types in pig

Pig data types are classified into two types. They are:

1.Primitive

2.Complex

Primitive Data Types: The primitive datatypes are also called as simple datatypes. The simple data types that pig supports are: 

a.int : It is signed 32 bit integer. This is similar to the Integer in java.

b.long : It is a 64 bit signed integer. This is similar to the Long in java.

c.float : It is a 32 bit floating point. This data type is similar to the Float in java.

d.double : It is a 63 bit floating pint. This data type is similar to the Double in java.

e.chararray : It is character array in unicode UTF-8 format. This corresponds to java's String object.

f.bytearray : Used to represent bytes. It is the default data type. If you don't specify a data type for a filed, then bytearray datatype is assigned for the field.

g.boolean : to represent true/false values.

2.Complex Types: Pig supports three complex data types. They are listed below: 

a.Tuple : An ordered set of fields. Tuple is represented by braces. Example: (1,2)

b.Bag : A set of tuples is called a bag. Bag is represented by flower or curly braces. Example: {(1,2),(3,4)}

c.Map : A set of key value pairs. Map is represented in a square brackets. Example: [key#value] . The # is used to separate key and value.

Pig allows nesting of complex data structures. Example: You can nest a tuple inside a tuple, bag and a Map 



Q2.How can you interact with the shell in Apache pig

The shell in apache pig is called grunt shell. We can launch it by using simple command “pig” or “pig -x local”.

If we are interacting with linux terminal from pig’s grunt shell then use “sh” prefix followed by linux terminal commands in pig grunt shell.

For example we can list files in current directory from grunt shell as

grunt> sh ls -l

However, the latest version of pig as of now 0.16 supports a few commands even without using this prefix “sh”


Q3.Explain how pig differs from Map reduce

In simple terms Map Reduce is low level of programming and Pig is a high-level language for expressing data analysis programs which internally create sequence of Map Reduce Programs.

Pig is simple to learn and use as compared to Map Reduce.

Pig data flow language i.e pig Latin. For MapReduce, Java is by default supported programming language. However support for other language is also available.

Pig provides inbuilt optimization for MR jobs whereas in map reduce developer needs to take care of optimization.

Here are detail definition from official documentation:

Hadoop MapReduce is a software framework for easily writing applications which process vast amounts of data (multi-terabyte data-sets) in-parallel on large clusters (thousands of nodes) of commodity hardware in a reliable, fault-tolerant manner.

Pig's infrastructure layer consists of a compiler that produces sequences of Map-Reduce programs, for which large-scale parallel implementations already exist (e.g., the Hadoop subproject)


Q4.Explain how pig differs from sql

Pig Latin, looks similar to a Declarative language like SQL. One would find one-to-one corresponding operators. For Ex - Filter for where, Generate for select, Group for group by etc. But in reality, Pig Latin is far different from SQL. Pig Latin is a data flow procedural language, meaning we supply all the steps of "How" a task is to be accomplished, whereas in SQL we specify "What" is to be accomplished.

Another difference is that, SQL is query based and complex queries in SQL are written inside out - ie; queries required to be performed earlier are written as sub-queries of the ones required to be performed later. This can be confusing in terms of understanding. In Pig Latin, the script conveys the  data flow in  program execution order.

Pig Latin executes on massive data on a parallel distributed framework, originally Hadoop Map Reduce / HDFS. This is a batch mode execution good for streaming data access. SQL/RDBMS is not scalable like Hadoop, but is very good for individual record read / write.


Q5.Explain the scalar data types in pig

Scalar Data Types

a.int : It is signed 32 bit integer. This is similar to the Integer in java.

b.long : It is a 64 bit signed integer. This is similar to the Long in java.

c.float : It is a 32 bit floating point. This data type is similar to the Float in java.

d.double : It is a 63 bit floating pint. This data type is similar to the Double in java.

e.chararray : It is character array in unicode UTF-8 format. This corresponds to java's String object.

f.bytearray : Used to represent bytes. It is the default data type. If you don't specify a data type for a filed, then bytearray datatype is assigned for the field.

g.boolean : to represent true/false values.
