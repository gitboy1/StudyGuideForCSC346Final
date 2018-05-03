# StudyGuideForCSC346Final
## Open StudyGuideForCSC346Final feel free to contribute
## connecting to mysql database
### 1. Generally, what is the result set?
The result set is all of the records returned by a query made against (a) database table(s).
### 2. How is the result set used to move data from the rs to something useful like an object.
While traversing the result set via a while loop (while rs.next) objects may be constructed using rs.getString("columnName") and assigning those values to variables which may then be passed to an object constructor.
## connecting to a sqlite database
### 1. The main thing about sqlite is understanding what it is. SQlite is a full relational database. It represents a database as a single file and assumes it will be accessed from a single source.
### 2. One essential to understanding sqlite is knowing when it is appropriate to use, and when it is not appropriate. Once people see how useful it is, they have a tendency to use it when a server-based solution is more approrpriate.

### 1. What is Groovy? 
Apache Groovy is a Java-syntax-compatible object-oriented programming language for the Java platform. It is both a static and dynamic language with features similar to those of Python, Ruby, Perl, and Smalltalk. Apache Groovy is a Java-syntax-compatible object-oriented programming language for the Java platform. It is both a static and dynamic language with features similar to those of Python, Ruby, Perl, and Smalltalk. It can be used as both a programming language and a scripting language for the Java Platform, is compiled to Java virtual machine (JVM) bytecode, and interoperates seamlessly with other Java code and libraries. Groovy uses a curly-bracket syntax similar to Java's. Groovy supports closures, multiline strings, and expressions embedded in strings. Much of the Groovy's power lies in its AST transformations, triggered through annotations. (wikipedia)
### 2. What is the JDK? 
The Java Development Kit (JDK) is a software development environment used for developing Java applications and applets. It includes the Java Runtime Environment (JRE), an interpreter/loader (java), a compiler (javac), an archiver (jar), a documentation generator (javadoc) and other tools needed in Java development (wikipedia)
### 3. Does Groovy use the same JDK as Java? 
don't know
### 4. How are primitives like integers represented in Groovy? 
They are represented as objects. While Groovy declares and stores primitive fields and variables as primitives, because it uses Objects for everything, it autowraps references to primitives.
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
from s.o.: 
1. When we write a xml based layout in Android we use the string "xmlns:android="http://schemas.android.com/apk/res/android".
From the books I read it says that this is a namespace, but why do we use this? The link doesn't even exist. So what is the use of this?
#### Answers:
1. In general though, namespaces are used so that you don't have collisions between element names.
For example, if I created an XML schema that defined the element <person> and my friend created a separate XML schema that defined an entirely different element that also happened to be named <person>, we could have a collision. If I tried to reference both elements in an XML file, there would be no way to tell which one was which. If we use namespaces, however, myNamespace:person is clearly different than myFriendsNamespace:person.
The standard for defining a namespace is to use a URI, which is why you see that in the Android definition. It doesn't necessarily mean the schema exists at that location, it means that the URI is the unique name for that namespace
2. It is true that the link doesn't exists..But the string we are using is for declaring the Namespace... In XML,namespaces are used to avoid naming conflicts. You can refer to
#### from w3schools:
  XML Namespaces provide a method to avoid element name conflicts.
#### Name Conflicts
In XML, element names are defined by the developer. This often results in a conflict when trying to mix XML documents from different XML applications.
This XML carries HTML table information:
  
`<table>`

  `<tr>`
  
    `<td>Apples</td>`
    
    `<td>Bananas</td>`
    
  `</tr>`
  
`</table>`

to be cont'd...

### 3. What is the purpose of XML schemas and DTD? 
The purpose of an XML Schema is to define the legal building blocks of an XML document: 
* the elements and attributes that can appear in a document
* the number of (and order of) child elements
* data types for elements and attributes
* default and fixed values for elements and attributes
A document type definition (DTD) is a set of markup declarations that define a document type for an SGML-family markup language (SGML, XML, HTML). A Document Type Definition (DTD) defines the legal building blocks of an XML document.
### 4. What is the root of an XML document? Is one always needed? 
from w3schools:
#### XML Documents Must Have a Root Element
* XML documents *must* contain one root element that is the parent of all other elements

### 5. What is the DOM? 
The Document Object Model.
### 6. What are tags? 
Tags are markers that define the beginning and (typically) the ending of an element in an html or xml document.
* How are tags determined in XML (as compared to something like HTML)? 
In XML tags are defined by the developer as opposed to HTML which has standard-defined tags.
### 7. What are attributes? 
HTML attribute is a modifier of an HTML element type. An attribute either modifies the default functionality of an element type or provides functionality to certain element types unable to function correctly without them. In HTML syntax, an attribute is added to an HTML start tag. (wikipedia)
#### The href Attribute
HTML links are defined with the `<a>` tag. The link address is specified in the href attribute:
##### Example

 `<a href="https://www.w3schools.com">This is a link</a>`
 
 (from w3schools)
 
### 8. Can you represent arrays in XML? 
Yes

`<numbers type="array">`

`    <value>3</value>`

`    <value>2</value>`

`    <value>1</value>`

`</numbers>`

* If you had an array, how would you simulate it? 
see: https://stackoverflow.com/questions/6098922/array-definition-in-xml

### 9. Can you use jsoup with XML? Yes. 
It seems jsoup is better suited to parsing HTML.

* Should you? 
There are XML parsers better suited to parsing XML.

### 10. What is StAX? 
**Streaming API for XML (StAX)** is an application programming interface (API) to read and write XML documents, originating from the Java programming language community.

Traditionally, XML APIs are either:

* DOM based - the entire document is read into memory as a tree structure for random access by the calling application
* event based - the application registers to receive events as entities are encountered within the source document.
Both have advantages: DOM, for example, allows for random access to the document, and event driven algorithm like SAX has a small memory footprint and is typically much faster.

These two access metaphors can be thought of as polar opposites. A tree based API allows unlimited, random access and manipulation, while an event based API is a 'one shot' pass through the source document.

StAX was designed as a median between these two opposites. In the StAX metaphor, the programmatic entry point is a cursor that represents a point within the document. The application moves the cursor forward - 'pulling' the information from the parser as it needs. This is different from an event based API - such as SAX - which 'pushes' data to the application - requiring the application to maintain state between events as necessary to keep track of location within the document. (wikipedia)

### 11. Coding with StAX. 
* You will probably want source code, but it is important that you understand what is going on in the sourcecode. 
* be able to read and extract inner text 
* be able to extract attributes 
* What is the general procedure for creating an XML document in StAX? 
* How do you go about adding elements and attributes in StAX? 
## json 
### 1. What are the similarities and differences between XML and Json? 
Both JSON and XML can be used to receive data from a web server.

The following JSON and XML examples both defines an employees object, with an array of 3 employees:
**JSON example:**

`{"employees":[`

`    { "firstName":"John", "lastName":"Doe" },`

`    { "firstName":"Anna", "lastName":"Smith" },`

`    { "firstName":"Peter", "lastName":"Jones" }`

`]}`

**XML example:**
`<employees>`

`    <employee>`

`        <firstName>John</firstName> <lastName>Doe</lastName>`

`    </employee>`

`    <employee>`

`        <firstName>Anna</firstName> <lastName>Smith</lastName>`

`    </employee>`

`    <employee>`

`        <firstName>Peter</firstName> <lastName>Jones</lastName>`

`    </employee>`

`</employees>`

### JSON is Like XML Because
* Both JSON and XML are "self describing" (human readable)
* Both JSON and XML are hierarchical (values within values)
* Both JSON and XML can be parsed and used by lots of programming languages
* Both JSON and XML can be fetched with an XMLHttpRequest

### JSON is Unlike XML Because
* JSON doesn't use end tag
* JSON is shorter
* JSON is quicker to read and write
* JSON can use arrays

### The biggest difference is:
 XML has to be parsed with an XML parser. JSON can be parsed by a standard JavaScript function. 
 
### Why JSON is Better Than XML
* XML is much more difficult to parse than JSON.
* JSON is parsed into a ready-to-use JavaScript object.
### For AJAX applications, JSON is faster and easier than XML:
Using XML
* Fetch an XML document
* Use the XML DOM to loop through the document
* Extract values and store in variables
Using JSON
* Fetch a JSON string
* JSON.Parse the JSON string
 (w3schools)
### 2. Key:value Mapping 
### 3. nested objects 
### 4. array representation 
## a bit about api’s and keys. 
### 1. Why did we store the key in a credentials file? 
### 2. Why did we put the credentials files in the .gitIgnore? 
## git 
### 1. What is git? 
Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people (wikipedia)
* What is the difference between git and github? 

While GitHub is place where all the codes managed with GIT are hosted. "GitHub is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features." ... GitHub is a hosting service for Git repositories. (quora)
### 2. What are the benefits of using GIT? 
* Revert the code files back to their previous state
* Recall and revert the entire project back to its previous state
* Compare code changes over specific durations of time
* Find who last modified a piece of code that might be causing an issue or a problem
* Who introduced a particular issue and when

#### What are the problems? 

