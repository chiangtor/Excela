# Excela
xlsx2csv



### Download the poi extension

-----poi-----
[Index of /dist/poi/release/bin](https://archive.apache.org/dist/poi/release/bin/)


```
git clone 
mkdir -p lib 
wget   https://archive.apache.org/dist/poi/release/bin/poi-bin-3.17-20170915.tar.gz lib
cd lib
tar xzvf poi-bin-3.17-20170915.tar.gz & rm poi-bin-3.17-20170915.tar.gz
```

### ant build

```
ant build
```


### demo

```
java -jar build/jar/XLSX2CSV.jar  myexcel.xlsx > myexcel.csv

###  todo

split the sheet& index from myexcel.csv


### reference
The main XLSX2CSV.java class is copied from https://coderanch.com/t/552660/java/Java-find-load-class
