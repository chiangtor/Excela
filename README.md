# Excela
xlsx2csv



### Download the poi extension

[Index of /dist/poi/release/bin](https://archive.apache.org/dist/poi/release/bin/)


```
git clone 

mkdir -p lib 

wget   -P  lib https://archive.apache.org/dist/poi/release/bin/poi-bin-3.17-20170915.tar.gz 
cd lib
tar xzvf poi-bin-3.17-20170915.tar.gz & rm poi-bin-3.17-20170915.tar.gz
```

### ant build

```
$ant
Buildfile: /private/tmp/Excela/build.xml

clean:

compile:
    [mkdir] Created dir: /private/tmp/Excela/build/classes
    [javac] /private/tmp/Excela/build.xml:24: warning: 'includeantruntime' was not set, defaulting to build.sysclasspath=last; set to false for repeatable builds
    [javac] Compiling 1 source file to /private/tmp/Excela/build/classes

jar:
    [mkdir] Created dir: /private/tmp/Excela/build/jar
      [jar] Building jar: /private/tmp/Excela/build/jar/XLSX2CSV.jar

run:
     [java] Use:
     [java]   XLSX2CSV <xlsx file> [min columns]

main:

BUILD SUCCESSFUL
Total time: 1 second
```


### demo

```
java -jar build/jar/XLSX2CSV.jar  fixtures/Workbook1.xlsx

Sheet1 [index=0]:
"head1","head2"
"value1","value2"

Sheet2 [index=1]:
"head3","head4"
"value3","value5"


```

###  todo

split the sheet& index from myexcel.csv


### reference
The main XLSX2CSV.java class is copied from https://coderanch.com/t/552660/java/Java-find-load-class
