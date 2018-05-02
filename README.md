# StudyGuideForCSC346Final
## Open StudyGuideForCSC346Final feel free to contribute
## connecting to mysql database
### 1. Generally, what is the result set?
### 2. How is the result set used to move data from the rs to something useful like an object.
## connecting to a sqlite database
### 1. The main thing about sqlite is understanding what it is. SQlite is a full relational database. It represents a database as a single file and assumes it will be accessed from a single source.
### 2. One essential to understanding sqlite is knowing when it is appropriate to use, and when it is not appropriate. Once people see how useful it is, they have a tendency to use it when a server-based solution is more approrpriate.

### 1. What is Groovy? 
Apache Groovy is a Java-syntax-compatible object-oriented programming language for the Java platform. It is both a static and dynamic language with features similar to those of Python, Ruby, Perl, and Smalltalk. Apache Groovy is a Java-syntax-compatible object-oriented programming language for the Java platform. It is both a static and dynamic language with features similar to those of Python, Ruby, Perl, and Smalltalk. It can be used as both a programming language and a scripting language for the Java Platform, is compiled to Java virtual machine (JVM) bytecode, and interoperates seamlessly with other Java code and libraries. Groovy uses a curly-bracket syntax similar to Java's. Groovy supports closures, multiline strings, and expressions embedded in strings. Much of the Groovy's power lies in its AST transformations, triggered through annotations.
### 2. What is the JDK? 
The Java Development Kit (JDK) is a software development environment used for developing Java applications and applets. It includes the Java Runtime Environment (JRE), an interpreter/loader (java), a compiler (javac), an archiver (jar), a documentation generator (javadoc) and other tools needed in Java development
### 3. Does Groovy use the same JDK as Java? 
The Java Development Kit (JDK) is a software development environment used for developing Java applications and applets. It includes the Java Runtime Environment (JRE), an interpreter/loader (java), a compiler (javac), an archiver (jar), a documentation generator (javadoc) and other tools needed in Java development
### 4. How are primitives like integers represented in Groovy? 
They are represented as objects.
### 5. How are arrays represented in Groovy? 
def testArray = new String[3]
testArray[0] = "A"
testArray[1] = "B"
testArray[2] = "C"
### 6. Be able to code a for loop that iterates an array

## jsoup and scraping web pages 
### 1. What is scraping? 
Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.[1] Web scraping software may access the World Wide Web directly using the Hypertext Transfer Protocol, or through a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying, in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.
### 2. Is scraping ethical? 
It depends on the use of the data and the volume. Demanding too much data from a server such that it slows down and causes problems for other users is not right, nor is scraping data for malicious purposes. Using data for an simple homework assignment shouldn't be a problem.
### 3. One way to scrape files is to read the page and just use regular expressions to find the parts you are interested in. Why is Jsoup likely to be a better solution in most cases? 
Jsoup is designed to specifically 
### 4. Using JSoup: 
* Be able to extract inner text 
* What are selectors? 
* What is the relationship to CSS? 

## xml 
### 1. What are the two main uses of XML? 
XML is a "lingua franca" used for exchanging data between two systems that don't have the same "native" language.
### 2. What is the namespace problem? 
Basically the namespace problem exists because separate technologies use similar names for things (e.g. Document) and so they have to be imported to keep the various names distinct.
* Why are namespaces important in things like Android development? 
### 3. What is the purpose of XML schemas and DTD? 
The purpose of an XML Schema is to define the legal building blocks of an XML document: 
* the elements and attributes that can appear in a document
* the number of (and order of) child elements
* data types for elements and attributes
* default and fixed values for elements and attributes
A document type definition (DTD) is a set of markup declarations that define a document type for an SGML-family markup language (SGML, XML, HTML). A Document Type Definition (DTD) defines the legal building blocks of an XML document.
### 4. What is the root of an XML document? Is one always needed? 
### 5. What is the DOM? 
### 6. What are tags? 
* How are tags determined in XML (as compared to something like HTML)? 
### 7. What are attributes? 
### 8. Can you represent arrays in XML? 
* If you had an array, how would you simulate it? 
### 9. Can you use jsoup with XML? 
* Should you? 
### 10. What is StAX? 
### 11. Coding with StAX. 
* You will probably want source code, but it is important that you understand what is going on in the sourcecode. 
* be able to read and extract inner text 
* be able to extract attributes 
* What is the general procedure for creating an XML document in StAX? 
* How do you go about adding elements and attributes in StAX? 
## json 
### 1. What are the similarities and differences between XML and Json? 
### 2. Key:value Mapping 
### 3. nested objects 
### 4. array representation 
## a bit about api’s and keys. 
### 1. Why did we store the key in a credentials file? 
### 2. Why did we put the credentials files in the .gitIgnore? 
## git 
### 1. What is git? 
* What is the difference between git and github? 
### 2. What are the benefits of using GIT? 
* What are the problems? 

