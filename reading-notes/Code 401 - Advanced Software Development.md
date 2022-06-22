# Reading Notes in Java
- Details below are bullet points for a fullstack class in Java.
## Relational DataBase
- From practicing the Database, I can see that R is similar to SQL Bolt in that grabbing information. The comparison is similar but not the same, but for my understanding, I see the resemblence and can be useful to understand how things are ordered in a database and its limitations from knowing a little bit about R.
- Prep Work For SQL below images:
[img1](public/prepImg/prepsql1.JPG)
[img2](public/prepImg/prepsql2.JPG)
[img3](public/prepImg/prepsql3.JPG)
[img4](public/prepImg/prepsql4.JPG)
[img5](public/prepImg/prepsql5.JPG)
[img6](public/prepImg/prepsql6.JPG)
[img7](public/prepImg/prepsql13.JPG)
[img8](public/prepImg/prepsql14.JPG)
[img9](public/prepImg/prepsql15.JPG)
[img10](public/prepImg/prepsql16.JPG)
[img11](public/prepImg/prepsql17.JPG)
[img12](public/prepImg/prepsql18.JPG)




****
## Reading Notes 1
1. Variables: these are the primitive types such as int, long, double, char, ... Further, there are arrays and Strings we may utilize in Java. 
2. Operators: logical operators (!, ?=, ==,  <,>, <=, >=), instance of are a few of the operators we may use.
3. an Expression is like a sentence in grammer. you must specify keywords and logic to create a sentence. 
4. the Control Flow can change the flow of reading a program by using inheritence , looping, and/or logic 
5. A compiler is a tool that is used to check for errors such as syntax and any throws needed. it also integrates the libraries(dependencies) needed along with unwinding the stack. Machine language kicks off(linux uses ARM/ASM or depends on distro). 

****

****
## Things I want to know about:
****

![](public/AndroidDrawing.jpg)

## Reading Notes: Application Fundamentals (Software Development Kit)
  - SDK is a collection of development tools to develop Android application that is combined in one package that compiles the code along with Android app bundle.
  - Android apps can be written using kotlin, java, and C++. In other words, uses JVM to generate a class file. 
  ![](public/jvm2.JPG)
  - C++ may remind me of Linker set up, source files (main.cpp) -> translators -> relocatable object files -> linker(libraries and symbols) -> executable. 
  - However, the process of JVM is takes over for Android development. Instead of compiled language format of linking process, the way Java Architecture takes a different approach. this approach is creating virtual machines isolated with their own operating system on without using local machines operating system.   
  ![](public/jvm1.JPG)
  - here the JVM architecture is not that much more complicated. first java creates a source code (.java) then bytcode as a (.class). in a nutshell thats it!
  - where it gets a bit more sophistacated is in the class loading process.
    - load process allocates the memory using libraries predefined.
    - linking takes care of dependencies, symbols, etc
    - intialization takes static and interfaces and handles them differently as they arent immediately implemented.
    ![](public/jvm3.JPG)
  - thus, the process is the same for all languages in Android Development apps. whether c++ or kotlin. with the power of JVM one can pull kotlin and convert it to bytecode, then reconvert it to java, or Kotlin! all because JVM handles them all the languages the same way. 

- Android is a operating system - stack based linux kernel(acts as a interface between hardware and software). it is a open source environment. some features are touchscreen and smart phone capabilities. 
- thus security is handled differently from other operating system. the goal is to be flexible to all users and developers. things like connectivity to all lan, bluetooth devices, gyroscopes.
- linux system is in each app which is a different user in each kit
- Virtual machin runs in isolation from other apps (very similar to jvm)

### App components
- four types of app components: 
- Activities:
  - entry point for interacting with the user.such as reading emails, sorting emails, etc for user
- Services: entry point for running app in the background. such as music running continuously and closing app.
- Content Providers: allows sharing of an application data with another application. can be a file or entire SQLite database.
- Broadcast receivers: allows an application to respond to a bradcast intent. broadcast is set to low battery, then the broadcast receiver will run a code that will notify user that it is on low battery for charging. 

### Activating components
- all three (activities, services, and broadcast receivers) are asynchronous  messages called "intent".
- Intent which defines a message  to activate either a specific component or a pecific type of component. 
- it is an object that activates in a activity or service such as display information or send information.
- content providers handle exchanging information differently. they use Content Resolvers.
- startActivity() or startActivityForResult() does the activation in activity
- you can initiate a broadcast by passing intent to methods such as sendBroadcast(), sendorderedbroadcast(), or sendstickybroadcast().


### Manifest
- contains files in which it describes informtation about your application, such as build tools, package name, application metadata, registered activities, intent filters, permissions, and more.

`<?xml version="1.0" encoding="utf-8"?>
<manifest ... >
    <application android:icon="@drawable/app_icon.png" ... >
        <activity android:name="com.example.project.ExampleActivity"
                  android:label="@string/example_label" ... >
        </activity>
        ...
    </application>
</manifest>`

### Android template architecture
- manifest handles infromation about application.
- java folder contains java files which can be things like mainactivity class. this is where the main activities should derive from.
- resource folder contains all useful things for application to use
  - drawable has things like images, gifs, etc
  - layout is the template in which our application will look like (front end kind of thing)
  - values are static variables that we can use.


 ### Shared Preferences API
 - SharedPreferences allows key value pairs to be used from a file. 
 - to store and retrieve, use getSharedPreferences() from a Context. use case if is you are using multiple preference files identified by name. specify with the first parameter.
 - getPreferences() usage for an Activity. to use for one shared preference file of the activity.
 - For example, the following code accesses the shared preferences file that's identified by the resource string R.string.preference_file_key and opens it using the private mode so the file is accessible by only your app:

  ```
  Context context = getActivity();

  SharedPreferences sharedPref = context.getSharedPreferences(getString(R.string.preference_file_key),
  Context.MODE_PRIVATE);

  //use case for an Activity for one preference file
  SharedPreferences sharedPref = getActivity().getPreferences(Context.MODE_PRIVATE);

  ````

- naming convention for shared prefernce files should be done as follows `com.example.myapp.PREFERENCE_FILE_KEY` 

***

## Activity Lifecycle

- Creating lifecycle methods for users to stop and play are useful features to have.
- if used correctly, lifecycles can avoid buggy instances.
  * Crashing when a phone call is made or switches to another app while on current app.
  * Consuming system resources when not using the app
  * losing the users progress if returned later on
  * crash when rotating screen
- 
 
[Android Shared preferences](https://developer.android.com/training/data-storage/shared-preferences)

<a href="https://developer.android.com/training/testing/espresso" _target="blank">Espresso Testing (read Overview, Basics, and Recipes, plus any others that look interesting)</a>

<a href="https://developer.android.com/studio/test/espresso-test-recorder">Ridiculous superpower: the Espresso Test Recorder</a>

<a href="https://developer.android.com/guide/components/activities/tasks-and-back-stack" _target="blank">Android Tasks and the Back Stack</a>
***

## RecyclerView for displaying lists of data

<a href="https://developer.android.com/guide/topics/ui/layout/recyclerview#java" _target="blank">RecyclerView for displaying lists of data</a>



## Hashing 

- Hashing can be implemented a few ways to avoid collision.
  - LogFile style of implementation. using `unorderd list`
    - add to end - O(1)
    - delete Search and delete O(n)
    - disadvantage not the fastest
  - Compression Maps
    1. Division
    - converts a integer `[negative infinity , infinity]`
    - so division will never exceed `[0, N -1]` where N is array size.
    - compressionMap(key) = y mod N
    - collision is minimized but the disadvantage is that it still does collision quite frequently.
      - reason being is that we receive strings(keys) -> (101, 202, 303),
      - suppose N was multiplied by prime number and N -1(never exceed array size)
      - then y mod N will be 101 mod 101 is 0, 201 mod 101 is 0, 301 mod 101 is 0
      - but, something exist at 101. thus collision occurs
    2. Multiply add divide
      - to do this method the algo will look like `cmp(y) = ((ay+b) % p) % N` and N is a Prime integer, p is a prime integer < N, a, b are non zero constants
      - thus, if strings is (101, 202, 303) and N is 101,
        - then 101: 303 + 3 % 5 = 306 % 5 = 1, then 1 % 101 = 1
        - further 202: 202 x 3 + 3 = 609 % 5 = 4 = 4% 101 = 4
        - finally, 303: 909 + 3 = 912 % 5 = 2 = 2 % 101 = 2
        - All keys are different and prevents collison
    3. The best instance of Compression Maps is Multiply, Add, divide.
  - Seperate Chaining
    - uses a linked list data structure to store same hashed value in bucket array.
    - disadvantage is O(N) for searching in linked list but O(1) for insertion
  - Linear Probing
    - collision handling is placing values in seperate circular table set
    - when there are duplicate hash keys, it will place duplicates to the next available index.
    - disadvantage of linear probing is clustering. clustering is accumulation of elements in consecutive cells.
    - Which means that linear probing is O(N)
  - Quadratic Probing
    - similar to Linear Probing but differnece is in insertion where (hashing(key) + i**2) mod N
    - this will place key at i**2 index.
    - disadvantage, we cant access some elements in bucket array because it is being used from jumping quadratically.
  - Bloom Filter
    - uses two hashings x mod N and (2x +3 ) mode N.
    - disadvantage, false positives because a number can be present even though it was never inserted.
  - Double Hashing
    - hash1(k ) + j hash2(k) where hash1 = k mod N and hash2 = k mod N/2
    - uses a loop to iterate j and fills at j
    - similar to quadratic probing
  - Rehashing
    - load factor is entries/buckets in bucket list which  entries must be less than buckets. load factor must be less than 1
    - thus, the bucket array is resized almost double at times. this gaurantees that there is no collision
    - but at a cost of space complexity.
  - Bucket Array - Array of N elements. thus, An element with key and value pair will be stored at Array of N elements.
    - adding will be O(1)
    - deleting will be O(1)
    - disadvantage keys have to be integers and know what keys before hand. need to know the N amount of keys present.
  - HashTables -
    - Hash Function
    - bucket array
    - removes the assumption that keys have to be integers by turning all into an integer and map it to a value into a unique hashcode.
    - thus, the hashing returns a integer between 0 and N-1
    - Hashing method will be O(1)
  - after understanding few types of hashing implementations.
  - HASHING - to discuss what is a good hashing method
    - minimize collision where key1 != key2
    - thus hashing(key1) == hashing(key2)
    - hashing(key) should return value data. for example hashing(key) return unique value for hashcode
    - Memory address
      - hashing(key) returns memory address
      - disadvantage, not uniform.
    - Integer cast
      - int a = (int) T data
      - disadvantage, loss of data accuracy for data structure T data. for example T is a double.
      - thus, collision happens
    - Component Sum
      - partitioning bits into two components. for example 32 bits num2, 32 bit num2 and a 64 bit key will be passed to num1 and num2. then hashcode = num1 + num2
      - disadvantage, collisions occur because for example pots, spot, tops, spot, have the same strings characters in different orders.
    - Polynomial Accumulation (Horner's Rule)
      - different segments at 32 bits of our string. then do Ascii value of character x index of element where p is storeed + ...
      - then key will be unique. `for(int i = n -1; i >= 0; --i){sum = (sum*a) + arr[i]}`
