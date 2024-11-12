# The Organization of Digital Information Systems

> "The fundamental problem of communication is that of reproducing at one point either exactly or approximately a message selected at another point." -- [Claude Shannon](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf)

> "To a great extent the act of coding is one of organization." -- [James Hague](https://prog21.dadgum.com/177.html)

## tl;dr

TODO

## Purpose

We currently live in the [Information Age](https://en.wikipedia.org/wiki/Information_Age). The revolution of digital technology has made information pervasive and central to human economy, politics, society and culture.

The dual revolution of the [transistor](https://en.wikipedia.org/wiki/Transistor) and [information theory](https://en.wikipedia.org/wiki/Information_theory) allowed humans to store, transmit and transform information with incredible speed, precision, and at a very small cost.

The main challenge posed by an information society is to make sense of it. The information that makes up our digital world is vast and grows and changes at a vertiginous rate.

Our digital world is run by **digital information systems**. Digital information systems (DIS) are what we use when we interact with a digital device connected to the internet, such as as a smartphone or computer.

We call DIS by many names: apps, (web)pages, services, websites, programs, even servers. Unless you are an expert, they can blend into each other. What is clear about them is that these systems are:

- **digital**: you need a phone or computer to interact with them.
- **interconnected**: you need an internet connection to access them.
- **concerned with information**: all that these systems do is to store, transform and communicate information.

A fast-growing minority is tasked with designing, implementing and operating DIS. This is challenging work. For makers of information systems, the main challenge is also to make sense of the systems they interact with, and also of the systems that they create themselves.

The purpose of this treatise is to provide a novel and systematic way to understand DIS. Through this novel perspective, based on concepts, it should be much easier to understand existing DIS, as well as designing, implementing and operating new ones.

My hypothesis, which I'm actively testing as of the time of writing, is that the approach presented here can increase the speed of development of a DIS by an order of magnitude (~10x), while having very significant improvements (50-200%) in quality and the value of its features. The success or failure of these tools should be measured by whether they bring at least a 10x improvement to the speed, quality and value delivered by a team producing a DIS.

My hope is that, by making DIS radically easier to understand and implement, more humans will be empowered to bring their best to the world.

## Information as data

Information is usually defined as contextualized data - that is, data that, thanks to context, is invested with meaning. In other words, information is data that you understand. Data without context is not information, just mere data.

However, I will contend that, with the proper conceptual tools to understand data, anyone that sees value in that data will be able to quickly understand it, and therefore, convert it into information by providing the proper context. The conceptual tools we are after are the very thing that can help us transform data into information, because they are what enables us to understand any data that we care about.

What is information to someone might be mere data to someone else; it is a matter of interpretation. And, equally important, information is also itself data. Keeping data and information separate is outright harmful to one's understanding of any DIS.

**Therefore, I will use the terms "data" and "information" interchangeably throughout this treatise.**

## What are digital information systems and why do they exist?

An information system is any system that is capable of doing three things:

1. Communicate data
2. Store data
3. Transform data

Software systems are DIS. Their usefulness is conducted solely by their capacity to communicate, store and transform data. If a software system was replaced overnight with another software system that communicated, stored and transformed data in the same way as the first one, nobody would notice until the time came to actually modify the system. The code that composes the system is ultimately valuable solely for its capacity to communicate, store and transform data.

The vast hardware systems - nowadays referred to as "the cloud" - that run a great deal of our software are also chiefly concerned with communicating, storing and transforming data. Like software, they have no other purpose than that. This is what explains their central importance, and what justifies the vast economic resources devoted to them.

Through their capacity to communicate, store and transform data, DIS can be used for multiple purposes: telecommunications, education, entertainment, commerce, scientific research, etc. But these manyfold applications and the ultimate human purposes they enable are powered by the straightforward act of communciating, storing and transforming data.

What sets *digital* information systems different apart their non-digital predecessors is their incredible speed, accuracy and low cost of operation. Prior to the advent of [digital electronics](https://en.wikipedia.org/wiki/Digital_electronics), information systems were billions of times slower, less accurate and expensive.

Digital information systems, like their non-digital counterparts, are still physical. Only that instead of representing data with carvings on a stone or ink on paper, they use electrons within electronic devices.

## Why organization is the key to digital information systems?

Organization of information is a problem of abundance; when you have just a little bit of information, it's not a big deal to organize it. If you only have five shirts, you don't need a great organization system. The problem is when you have a lot of it. We now handle billions (or trillions) the amount of information we did before, but we still have the same brains.

The main challenge in building, maintaining and replacing information systems is to understand how data should flow through it. That is: how is its data going to be communicated and transformed? Storage usually doesn't pose a challenge, since it essentially consists of creating and maintaining copies of the data at different points in time, in a number of separate physical locations.

The challenge of communicating and transforming data is compounded by the fact that most information systems are alive and must be constantly adapted. When changing the system, the existing data flows should not be broken; and the new data flows should be coherent with the existing ones. So, designing an information system can never be a singular tour de force that, when successful, succeeds for all time; rather, the system must constantly be adapted and improved, even if it was well-designed the first time around.

The challenge to understand an information system is subtle, because most of the software that runs our world is composed of straightforward - even trivial - data transformations. What makes a system challenging to understand is not a single, thorny part of it. But rather: how do all the parts fit together with each other? The parts of an information system are closely and subtly interrelated; and most information systems are comprised of a large number of parts. Therein lies the difficulty in fully understanding the system: how each of the parts work, and how do they relate to each other?

Occasionally, there's a thorny algorithmic problem that's critical to an information system; these are hard and they are fun to tackle. Most of them have efficient solutions that you can just use off the shelf. What's distinctly difficult to pull off the shelf is a way to turn a complex system, made of many trivial parts, into a simple one.

Simple systems are easier to understand than complex systems. Rich Hickey [brilliantly defines simplicity](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/SimpleMadeEasy.md) as something that is not intertwined or entangled with other things; whereas complex things are things that are "folded together", therefore requiring you to understand them not just in isolation, but in all their possible interrelations.

According to [Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks), complexity can be divided into two: essential complexity, which is the minimum possible complexity of a system that implements a set of features; and accidental complexity, which is complexity that can be avoided by a better design. In other words, essential complexity is the minimum possible complexity of a given system.

Whether you pick Hickey's or Brooks' definition, the art of system design is the making of systems that are as simple as possible. For Fred Brooks, the main quality of simple systems is conceptual integrity. Conceptual integrity is an emergent property of a system that is designed by either one person or a small group of persons who have an unified vision of how the system should be. The notion of the concepts of the system being "integral" resonates deeply with Christopher Alexander's notion of strong centers as the main quality of good architectural designs. These two authors may well be talking about the same thing: a good system is composed of consistent parts that are organized harmoniously.

Fred Brooks' recommendation to tackle conceptual integrity was to try to fit the design in the head of a single architect, or of a small and highly coordinated group of architects. I am intrigued by the possibility of going beyond this, and finding conceptual tools that allow information workers to co-create information systems that evolve towards simplicity and create a harmonious whole, not unlike what workmen did five hundred years ago when building a cathedral.

**The limiting factor for those who create information systems is complexity**. Data transformations, by themselves, are extremely cheap (in terms of the time and the energy used by the computer resources required to do them) and have extremely low error rates. It is the making and maintaining of a coherent information system that can make or break an organization, an institution, and even perhaps the global economy.

This is quite interesting, because in pre-information economies, it was energy, not organization, that was the limiting factor of the creation of wealth. Therefore the search for simplicity is not merely an interesting or reasonable pursuit: it is the central way in which complexity, the limiting factor of an information economy, and therefore of wealth creation, can be tackled.

## The main thesis: to organize the system, always focus on the data

The main contention of this treatise is that *the* way to design simple DIS is to focus on the data that they communicate, transform and store. It is as simple as that.

Designing DIS is already a complex task. However, it becomes exponentially harder when those responsible for building or understanding a system are distracted by everything except the data it handles.

What is this everything else that holds the attention of makers of DIS? Here are a few examples:

- Programming languages.
- Programming paradigms.
- Type systems.
- Libraries.
- Communication protocols.
- Operating systems.
- System architectures.
- Performance.
- Availability.
- Cost.
- AI.

(We could call this *The List*)

All of the above are necessary, but they are merely tools - means to an end. And that end is always about the data: how it's communicated, transformed, and stored. The game is data.

But, at the time of writing, this is not the prevalent paradigm. The way I see it, those making DIS are painters that only look at their their brush or their palette; only rarely do they give a fleeting glimpse to the picture that they are painting.

New developments such as generative AI or big data don't change these facts; the paradigm is neutral towards them.

If you take away one thing from this treatise, it should be this one: **if you are working with a DIS, look at the painting (the data) as much as possible. And ignore as much as possible the brush and the palette (The List).**

Why not look at data and focus on The List? Normally, nobody asks this question. When I happen to raise it, I obtain two arguments against just focusing on the data:

1. There's too much data, so we cannot look directly at it. That's why we have programming languages, programming paradigms, libraries, etc. (The List).
2. Data is just a detail. We should be focused on bigger, deeper things, not on low-level things.

This entire treatise is built on toppling these two myths with the following (hypo)theses:

1. Once we decide to look at the data directly, there are ways in which we can abridge it without losing descriptive power. And these ways are much simpler than The List. "These ways" is what fills up the rest of this treatise.
2. Makers of DIS are in dire need of humility. Simple data is powerful, even exciting. The details matter. They can be joined into harmonious wholes. But to eschew details because they are beneath oneself is *exactly* what's keeping us mired in a mess of our own making.

Our contemporary attitude towards software is focused, perhaps naturally, on software itself, and not on the data which flows through it and which justifies the existence of software itself. But it is perfectly possible to see code as the negative impression (just like a picture taken with film has a [negative](https://en.wikipedia.org/wiki/Negative_(photography))) of the data flows it enables.

When the data is not seen, the trivial becomes difficult and the nontrivial impossible.

Data itself is simple and can be directly seen. By using data to understand and make a DIS, we can find the simplest possible expression of the system that will get the job done.

This is the central thesis of this treatise. We'll explore now how to make this a reality through five practical concepts, fancily called *pillars*. Each pillar removes an obstacle to seeing the data flowing through an information system.

## The five pillars

1. **Single representation of data**
2. **Single dataspace**
3. **Call and response**
4. **Code is data**
5. **Interface is code**

### Pillar 1: single representation of data

To see data, we must find a good way to represent it. The data that goes through our digital systems is binary, consisting of [bits](https://en.wikipedia.org/wiki/Bit). Bits can be represented by zeroes and ones. Working with zeroes and ones, however, is not at all practical or desirable. In programmer parlance, they are too *low-level* for humans to read and write.

Here I will propose a data representation based on *text*. While data representations can also be graphical (though always using text), I've chosen to go with the portability and compactness of text. Text is also much easier to communicate between computers because it is *linear*, but I'm getting ahead of myself.

Whether you use this data representation or some other representation, it is my contention that without a *determined* and *sufficient* data representation, you cannot directly look at the data in a DIS. **Therefore, the first step towards seeing the data is to have a single representation of data** and use it for *everything*.

A data representation requires us to define two things:

- Ways to set boundaries between one *value* and another value. Values are discrete units of data.
- Specify basic *types* of data.

Here I'll introduce *fourdata*, a data representation that is purely based in text and has four types of data:

1. Number
2. Text
3. List
4. Hash

Because there are only four types of data in this representation, we call this representation *fourdata*. The first two data types, number and text, are the *single* data types. That means that they represent a *single value*. For example:

```
1234
```

```
Hi
```

Single data types, however, need to be organized into structured wholes. Fourdata also provides two *multiple* data types, where one value can hold multiple values *inside* itself. The first multiple data type is the *list*, which is a sequence of ordered values.

```
1 Eggs
2 Butter
3 Lettuce
```

In the list above, each item has a number next to it. This is its *key*, which is always a number. Note how each value goes in its own line.

The second multiple data type is the *hash*. In a hash, the keys are texts:

```
born 1959
firstName Gustavo
lastName Cerati
```

Hashes don't have a particular order to their keys; however, fourdata orders them alphabetically, so that two equivalent hashes are represented in the exact same order. This allows us to have the exact same text representing two hashes that we consider to be equal.

In the example above, we see how the values of a hash can be of different types: `born` is number, `firstName` and `lastName` are text.

We can have a hash or a list inside another hash or list. For example:

```
1 born 1959
  firstName Gustavo
  lastName Cerati
2 born 1962
  firstName John
  lastName Squire
```

The list above has two hashes, each of them representing a (great) musician. We say that those hashes are *nested* into the list.

It's a good moment how we use empty spaces (*whitespace*, in programmer parlance) to convey nestedness. In the list above, item number 1 is

```
born 1959
firstName Gustavo
lastName Cerati
```

And item number 2 is

```
born 1962
firstName John
lastName Squire
```

When we want to make a list out of these two, the starting point of each hash is going to be to the *right* of the keys of the list (`1`, `2`). The leftmost part of each hash (its own keys) are going to be aligned one character to the right of the end of the key after which it comes.

```
1 born 1959
  firstName Gustavo
  lastName Cerati
2 born 1962
  firstName John
  lastName Squire
```

If we want to name this list, we can do this as follows:

```
musicians 1 born 1959
            firstName Gustavo
            lastName Cerati
          2 born 1962
            firstName John
            lastName Squire
```

Note how we indented `1` and `2` to the right of `musicians`. Now, we have a single hash which contains a list, which in turn contains two hashes, each of them containing three texts.

Simple as it is, this data representation can be used to represent any data relevant to an information system. Here are a few examples:

**An [HTTP](https://en.wikipedia.org/wiki/HTTP) request and response pair**

```
request headers Accept application/json
                User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
        host example.com
        method GET
        path /api/books/1234
        type HTTP/1.1
response code "200 OK"
         headers Content-Length 83
                 Content-Type application/json
         body author "Edward Said"
              id 1234
              isbn "978-0-394-42814-7"
              title Orientalism
```

**A table in a [relational database](https://en.wikipedia.org/wiki/Relational_database)**

```
books 1 author "Edward Said"
        created "2024-10-23T20:24:15.936Z"
        id 1234
        isbn "978-0-394-42814-7"
        title Orientalism
      2 author "Michel Houellebecq"
        created "2024-10-23T20:25:22.411Z"
        id 1235
        isbn "978-2-08-147175-7"
        title Serotonin
      3 author "Paul Graham"
        created "2024-10-23T20:30:44.602Z"
        id 1237
        isbn "978-0130305527"
        title "On Lisp"
```

**The data in the registers of a [6502 processor](https://en.wikipedia.org/wiki/MOS_Technology_6502)**

```
Accumulator "00110100"
X "01100001"
Y "11001010"
StackPointer "11110111"
ProgramCounter "1100001010101011"
StatusRegister "00100101"
```

**The [HTML](https://en.wikipedia.org/wiki/HTML) of a small page**

```
head title "Welcome to my site"
body 1 h1 "Hello World!"
     2 p 1 class text
         2 "This is my site"
```

Now, where does this data "go"? That's what we tackle in the next pillar.

### Pillar 2: single dataspace

We just established a single representation of data, so we can see any piece of data in a consistent manner. At this point, our main obstacle to "seeing the entire picture" is that the data of the system is not grouped together. So we'll tackle that by creating a single dataspace where all the data is available as a coherent whole.

In this pillar we will focus on data "at rest" - that is, data that is stored and ready to be accessed, rather than actively flowing between different parts of the system. Changes in data (communication and transformation) will come in pillar 3.

The [world wide web](https://en.wikipedia.org/wiki/World_Wide_Web) is the prime example of an unified dataspace. What makes an unified information space powerful is that you can potentially address all the information in the world from it. This is why the web is powerful: because it is a single dataspace.

In the web's dataspace, every document is represented by a URL (uniform resource locator) that tells you "where" that document is. For example, Wikipedia's page for the world wide web is located at `https://en.wikipedia.org/wiki/World_Wide_Web`. This URL tells you "where" the page is.

Our notion of a dataspace will replace URLs with *paths*. A path is a sequence of texts and numbers. Let's illustrate with an example by going back to the book data we saw in pillar 1:

```
books 1 author "Edward Said"
        created "2024-10-23T20:24:15.936Z"
        id 1234
        isbn "978-0-394-42814-7"
        title Orientalism
      2 author "Michel Houellebecq"
        created "2024-10-23T20:25:22.411Z"
        id 1235
        isbn "978-2-08-147175-7"
        title Serotonin
      3 author "Paul Graham"
        created "2024-10-23T20:30:44.602Z"
        id 1237
        isbn "978-0130305527"
        title "On Lisp"
```

How would you get or refer to the book "Orientalism"? We know it is inside `books`, which is a list, and that it is the first book in that list. The *path* to that book is `books 1`.

Similarly, the path to "On Lisp" is `books 3`. The path to the `isbn` of "On Lisp" is `books 3 isbn`.

Through a path, we can access any value we want. And values need not be just texts or numbers; they can be hashes or lists as well. Every value in the dataspace has a path to it. And, interestingly enough, paths are still data, because they can be represented as either hashes or lists. For example, the path `books 3 isbn` can be represented as either hash:

```
books 3 isbn
```

Or as a list

```
1 books
2 3
3 isbn
```

The first representation fits in a single line, so we will go with that one.

The core of an unified dataspace is that every part of the data has a path. There's no data "floating" anywhere. Every part of the data has a path, a place, a location. Rather than using *place* or *location*, we will use the term *path* to indicate where a value is.

How do we go from a small amount of data, like we saw above, to a larger whole? Let's expand on the previous example, and imagine that our `books` list is within our "Main Database". We can then express our dataspace like this:

```
"Main Database" books 1 author "Edward Said"
                        created "2024-10-23T20:24:15.936Z"
                        id 1234
                        isbn "978-0-394-42814-7"
                        title Orientalism
                      2 author "Michel Houellebecq"
                        created "2024-10-23T20:25:22.411Z"
                        id 1235
                        isbn "978-2-08-147175-7"
                        title Serotonin
                      3 author "Paul Graham"
                        created "2024-10-23T20:30:44.602Z"
                        id 1237
                        isbn "978-0130305527"
                        title "On Lisp"
```

So now "Main Database" is represented by a hash containing another hash, `books`. Now, the path to "On Lisp"'s `isbn` is `"Main Database" books 3 isbn`.

We can then add other values inside "Main Database", for example `users`, or `purchases`.

After this example, we can notice two things:

1. *Context* makes our dataspace grow towards the *left*, and detail makes our dataspace grow towards the *right*. For example, by going left from `books` to "Main Database", we acquire more context for the data we have; by going further to the right, we detail it further.


```
              "Main Database" books 1 author "Edward Said"

more context <--------------------------------------------> more detail
```

2. We can see the rightmost value of any path also as part of the path! Since a path is a sequence of texts and numbers, and rightmost values must also be texts and numbers (since they don't contain anything else), we can just simply put that value at the end of the path. If we did that, we could see something like this as a path:

```
"Main Database" books 1 author "Edward Said"
```

Or also this:

```
"Main Database" books 3 isbn "978-0130305527"
```

If this is still not clear, you could interpret it like this:

```
"Main Database" -> books -> 3 -> isbn -> "978-0130305527"
```

where each value on the left takes you to the next value.

We can then start to understand a dataspace as a collection of paths. The paths not only take you to the data: they **are** the data. This is highly suggestive of how brains work: the interconnections are not just a way to the data, but they actually *are* the data itself. There's no need for [metadata](https://en.wikipedia.org/wiki/Metadata) ("data that provides information about other data"). *All the data is in the data*.

Paths organize the data using only data. This stands in stark contrast with a spreadsheet, where the data is stored in cells named `A1`, `A2`, `B147`, etc. In those cases, you don't know what's in `B147` until you go see what really is in there. But in the dataspace above, when you see `"Main Database" books 3`, you already know you probably are looking at a single book.

This also stands in contrast with the traditional way of organizing memory in computers, which is memory addresses. Memory can be addressed through numbers, using the convention that each number represents a fixed amount of bits in the memory. In Ye Olden Days, each of the `books` would have been placed in a specific memory address.

Both spreadsheets and memory addresses have the same problem: they require data that is not in the dataspace to find values in the dataspace. But a dataspace that uses meaningful paths to organize information is free of that limitation.

While any implementation of a digital dataspace will rely on memory addresses, this can be left to the implementation. The dataspace, however, is our *interface* to data, and that interface - I contend - can be used to model anything, even low level representations that map to memory addresses.

With paths, [places](https://www.youtube.com/watch?v=-6BsiVyC1kM) become memorable, associative and even permanent.

Perhaps the most curious consequence of this approach is that we have no way of representing empty lists or hashes - no empty boxes! Every line in fourdata has a rightmost value that's either a text or a number. Contrast this with a spreadsheet, or with computer memory, which is full of cells or addresses that contain no value. In contrast, in this representation there are no empty spaces: all the data that is there represents something. Like [breadcrumbs](https://en.wikipedia.org/wiki/Breadcrumb_navigation), paths always point you somewhere.

Every DIS stores its data in two primary forms: files and databases. The rest of this section will show how we can put their data into this framework.

Files are the simplest of the two. They consist of a `path`, a `name` and `contents`. For example:

```
contents "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
name hello.c
path C:\Users\dmr\clang
```

Normally, files have other things associated with them, such as a creation time, a size, and other characteristics that are necessary for the [file system](https://en.wikipedia.org/wiki/File_system). We can safely ignore these features for the purposes of our discussion.

A few things to notice about the file above:
- The `path` starts with `C:`, which means the main [hard disk](https://en.wikipedia.org/wiki/Hard_disk_drive). Then, it has three more parts, subdivided by backslashes (`\`): `Users`, `dmr` and `clang`. All of these are texts.
- The `name` is also a text.
- The `contents` are an unreadable sequence of zeroes and ones. With files, we cannot jump to a specific section of its contents, or get a single part. When we get the file, we get the whole thing. But what's good about files is that they are quite close to the "real matter" of an information system: [binary data](https://en.wikipedia.org/wiki/Binary_data).

To simplify things, we could just put the name of the file at the end of the path and get rid of the `name` key.

```
contents "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
path C:\Users\dmr\clang\hello.c
```

We can go even one step further and represent the file like this:

```
C:\Users\dmr\clang\hello.c "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
```

A better way to do it is to split the path into hashes (that is, into a path), and add the contents as the last item.

```
C Users dmr clang hello.c "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
```

Using this structure allows us to group files that are in the same directories in a way that's easy to see. For example, if we have a second file in the same directory, we could represent it like this:

```
C Users dmr clang hello.c "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
                  indefatigable.c "001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111011010000011110100101000011010010110111001110100"
```

Now, where *is* this main hard disk? Hard disks must be attached to a computer in order to be accessible. In the context of DIS, these computers are usually called [servers](https://en.wikipedia.org/wiki/Server_(computing)), to distinguish them from computers to which a user has direct physical access. Let's call this server the `Main Server`. Then, we can represent our two files like this:

```
"Main Server" C Users dmr clang hello.c "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
                                indefatigable.c "001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111011010000011110100101000011010010110111001110100"
```

You might notice we haven't used a single list yet to represent files. Instead, we're using hashes for everything. The reason is simple: texts are much better names than numbers can be. While we could name directories, files and even servers using numbers, it would be almost impossible to remember what is what. Whereas names, expressed as text, are much more evocative and memorable.

With the approach above, we can now say that we have a *path* for each of the files in our system. For example, the *path* to the contents `hello.c` is:

```
"Main Server" C Users dmr clang hello.c
```

So the definition of *path* in a file system paths (`C:\Users\dmr\clang|hello.c`) and that from a web URL (`https://example.com/clang/examples/hello`) meld into one.

The contents of files have to be *interpreted* for them to have any meaning to us. Let's decode now the contents of `hello.c`. We assume this is a text file, therefore we will try to interpret it as such. This file is encoded with [UTF-8](https://en.wikipedia.org/wiki/UTF-8), a way to convert a sequence of zeroes and ones into a list of numbers.

```
1 35
2 105
3 110
4 99
5 108
6 117
7 100
8 32
9 60
10 115
11 116
12 100
13 105
14 111
15 104
16 62
17 10
18 105
19 110
20 116
21 32
22 109
23 97
24 105
25 110
26 98
27 40
28 41
29 32
30 123
31 10
32 32
33 32
34 112
35 114
36 105
37 110
38 116
39 102
40 40
41 34
42 72
43 101
44 108
45 108
46 111
47 44
48 32
49 87
50 111
51 114
52 108
53 100
54 33
55 34
56 41
57 59
58 10
59 32
60 32
61 114
62 101
63 116
64 117
65 114
66 110
67 32
68 48
69 59
70 10
71 125
72 10
```

Note that the column of numbers in the left only indicates the position of each number. The actual numbers that are in the sequence of zeroes and ones are the ones on the right column.

If we now use [Unicode](https://en.wikipedia.org/wiki/Unicode), we can convert these numbers into characters. Unicde is a way to map numbers into the characters used by the world's writing systems.

```
1  #
2  i
3  n
4  c
5  l
6  u
7  d
8
9  <
10 s
11 t
12 d
13 i
14 o
15 h
16 >
17 (newline)
18 i
19 n
20 t
21
22 m
23 a
24 i
25 n
26 b
27 (
28 )
29
30 {
31 (newline)
32
33
34 p
35 r
36 i
37 n
38 t
39 f
40 (
41 "
42 H
43 e
44 l
45 l
46 o
47 ,
48
49 W
50 o
51 r
52 l
53 d
54 !
55 "
56 )
57 ;
58 (newline)
59
60
61 r
62 e
63 t
64 u
65 r
66 n
67
68 0
69 ;
70 (newline)
71 }
72 (newline)
```

If we now join these characters into a text, we will get:

```
"#include <stdio.h>\nint main() {\n  printf(\"Hello, World!\");\n  return 0;\n  }"
```

That's a [C program](https://en.wikipedia.org/wiki/C_(programming_language))! It looks a bit mangled in a single line: a text editor would show the above as follows:

```
#include <stdio.h>
int main() {
   printf("Hello, World!");
   return 0;
}
```

Before we move on to databases, we can see the [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) file format. This type of file is usually used to hold tabular data.

Let's say we have a CSV file with the top ten hit songs of [1985](https://en.wikipedia.org/wiki/1985).

```
"Main Server" C Users dmr clang hello.c "001000110110100101101110011000110110110001110101011001000010000000111100011100110111010001100100011010010110111101101000001111100000101001101001011011100111010000100000011011010110000101101001011011100110001000101000001010000111101100001010111000011110100010010110110000001011000101100011101101001110110001011000010010000000101000010000101100001001110100010000000"
                                indefatigable.c "001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111011010000011110100101000011010010110111001110100"
                          music hits1985.csv "010100100110000101101110011010110010110001010011010000110110000101110010011001010110110001100101011100110010000001010111011010000110100101110011011100000110010101110010001011000010000001010101011011100110000101101101010000011010010100001110100110110100100101011011101000101001"
```

If we decode this `hits1985.csv` file in a text editor, we'll see this:

```csv
Rank,Title,Artist,Weeks at #1
1,Careless Whisper,Wham! featuring George Michael,3
2,Like a Virgin,Madonna,6
3,Wake Me Up Before You Go-Go,Wham!,3
4,I Want to Know What Love Is,Foreigner,2
5,I Feel for You,Chaka Khan,3
6,Out of Touch,Daryl Hall & John Oates,2
7,The Power of Love,Huey Lewis and the News,2
8,Everybody Wants to Rule the World,Tears for Fears,2
9,Money for Nothing,Dire Straits,3
10,Crazy for You,Madonna,1
```

This is much more readable. However, a better way to see this data could be this:

```
"1985 Hit Songs" 1 Rank 1
                   Title Careless Whisper
                   Artist "Wham! featuring George Michael"
                   "Weeks at #1" 3
                 2 Rank 2
                   Title "Like a Virgin"
                   Artist "Madonna"
                   "Weeks at #1" 6
                 3 Rank 3
                   Title "Wake Me Up Before You Go-Go"
                   Artist "Wham!"
                   "Weeks at #1" 3
                 4 Rank 4
                   Title "I Want to Know What Love Is"
                   Artist "Foreigner"
                   "Weeks at #1" 2
                 5 Rank 5
                   Title "I Feel for You"
                   Artist "Chaka Khan"
                   "Weeks at #1" 3
                 6 Rank 6
                   Title "Out of Touch"
                   Artist "Daryl Hall & John Oates"
                   "Weeks at #1" 2
                 7 Rank 7
                   Title "The Power of Love"
                   Artist "Huey Lewis and the News"
                   "Weeks at #1" 2
                 8 Rank 8
                   Title "Everybody Wants to Rule the World"
                   Artist "Tears for Fears"
                   "Weeks at #1" 2
                 9 Rank 9
                   Title "Money for Nothing"
                   Artist "Dire Straits"
                   "Weeks at #1" 3
                 10 Rank 10
                    Title "Crazy for You"
                    Artist "Madonna"
                    "Weeks at #1" 1
```

To get to the above, we did quite a bit of interpreting of our CSV file:

- From binary data to a sequence of numbers.
- From a sequence of numbers to a sequence of unicode characters.
- From unicode characters to lines of text divided by commas into columns.
- From the above into a list of hashes, each with four keys and four values.

While CSVs are a very expressive and widely used way of representing structured information, a great deal of structured information nowadays is stored in databases. Databases are *computer programs* that store data using files; but they do it in a more involved way that provides the following features:

- Efficiency: you can access a single value, rather than getting the entire file.
- Validation: you can check whether incoming data has a certain shape before storing it.
- Locking: if two users want to save a value at the same path at the same time, the database makes sure to process the requests one at a time.
- Queries: you can construct specific inquiries about data which will get you the right results efficiently.

For practical purposes, there are two families of databases: [relational databases](https://en.wikipedia.org/wiki/Relational_database) (also called SQL databases) and [non-relational databases](https://en.wikipedia.org/wiki/NoSQL).

Relational databases date from 1970 (!) and are tremendously powerful. Their power stems from their quite rigid structure. Overall, a relational database is composed of tables with rows and columns. This can be directly modeled in fourdata as follows:

- Table: list
- Row: hash

For example, taking some books from the example at the top:

```
"Main Database" books 1 author "Edward Said"
                        created "2024-10-23T20:24:15.936Z"
                        id 1234
                        isbn "978-0-394-42814-7"
                        title Orientalism
```

We could interpret `books` to be a table of "Main Database". We have here one row with five columns (`author`, `created`, `id`, `isbn` and `title`). Relational databases are called *relational* because they naturally express relationships between different tables. For example:

```
"Main Database" books 1 author "Edward Said"
                        created "2024-10-23T20:24:15.936Z"
                        id 1234
                        isbn "978-0-394-42814-7"
                        title Orientalism
                users 1 id fpereiro
                purchases 1 book 1234
                            created "2024-11-04T22:44:10.196Z"
                            user fpereiro
```

If we look at `purchases 1`, we can see that the book purchased has `book 1234` and `user fpereiro`. Since we have a book with `id 1234` ("Orientalism") and a user with id `fpereiro`, relational databases can *join* this data to express the fact that this purchase involves both this particular book and this particular user. This can be done quite expressively using [SQL](https://en.wikipedia.org/wiki/SQL), which is a query language.

For now, it is enough to have a direct mapping from relational databases to fourdata: this allows us to put relational data at rest into our dataspace.

Non-relational databases can also be represented in dataspace. The most common one, [MongoDB](https://en.wikipedia.org/wiki/MongoDB), stores data in collections of [JSON](https://en.wikipedia.org/wiki/JSON) objects. To map this to fourdata, we can simply make each collection a list of items.

```
"Mongo Database" visitors 1 date "2024-11-11T16:42:01.322Z"
                            ip "140.28.111.224"
                          2 date "2024-11-11T16:42:02.299Z"
                            ip "220.49.66.236"
```

[Redis](https://en.wikipedia.org/wiki/Redis), my favorite database, has many data types available. The most common ones can be readily mapped to fourdata. Lists and hashes map one to one with fourdata.

```
"redis list" 1 foo
             2 bar
"redis hash" id foo
             password bar
```

Sets can be represented as a list with no repeated elements or as a hash of which we only care about the keys.

```
"set as list" 1 foo
              2 bar
"set as hash" foo 1
              bar 1
```

Sorted sets can be represented with a list of hashes.

```
"sorted set" 1 score 1000
               value foo
             2 score 1001
               value bar
```

The above should be enough for almost all possible data that is at rest. In exceptional circumstances, it can be useful to represent lower level data. For example, we could use fourdata to represent the contents of memory addresses, if we're doing low level programming.

```
"0x1A3F" "0100100001100101011011000110110001101111000000000000000000000000"
"0x1A5F" "0101011101101111011100100110110001100100000000000000000000000000"
```

We could also use this representation to outline the [scope](https://en.wikipedia.org/wiki/Scope_(computer_science)) of the variables of a part of our program.


```
outerFunction "own variables" 1 a
                              2 b
middleFunction parent outerFunction
               "free variables" 1 a
                                2 b
               "own variables" 1 c
innerFunction parent middleFunction
              "free variables" 1 a
                               2 b
                               3 c
              "own variables" 1 b
                              2 d
```

Now that we can represent all the data of our system in a consistent and centralized way, we can see that this single dataspace doesn’t just represent data: it also organizes, contextualizes, and connects data. In short, it *is* the data. Now that we have mastered the data at rest, we're ready to tackle data communication and transformation in pillar 3, where the system comes to life.

### Pillar 3: call and response

Earlier, we defined a DIS as something that communicates, transforms and stores digital data. In pillar 3, which is the central pillar, we will find a way to express communication and transformation of data *using data itself*.

Let's start with data communication. We can understand communication as data flowing from one point of the system to another one. For example:

```
system 1 sends to system 2 a message "hello" -----------> system 2 receives from system 1 a message "hello"
```

We will name this a *call*. We can say that system 1 is making a call to system 2. The contents of that call are the message, in this case `hello`. Let's express it in fourdata:

```
call from "system 1"
     message hello
     to "system 2"
```

Two things must happen for us to consider the call as successful: 1) system 2 gets the message that system 1 sent; 2) system 2 must know that system 1 is the one that sent it.

How this is implemented is quite involved. For example, nowadays a typical (though not at all universal) way to send messages between systems is to use the following stack:

1. Create a JSON payload with the data.
2. Wrap it in a HTTP request.
3. Send it through [TCP](https://en.wikipedia.org/wiki/Transmission_Control_Protocol).
4. Let TCP use [DNS](https://en.wikipedia.org/wiki/Domain_Name_System) to find system 2 and [IP](https://en.wikipedia.org/wiki/Internet_Protocol) to send the pieces of the message.

Despite its apparent complexity, communication between systems is essentially a solved problem. Most of the time, we can rely on system 1 being able to send messages to system 2 and system 2 receiving them.

We now have to deal with data transformation. The core idea is that we can understand a transformation as a sequence of a *call* and a *response*. Let's extend the previous example:

```
call from "system 1"
     message hello
     to "system 2"
response "how are you?"
```

Note that the response doesn't contain `from` or `to`, since it's clear that they are the same as those of the call, only reversed. All that comes back is data.

We can see then that data transformation, or computation, can be modelled as two way communication.

**DEAR READER: this treatise is in its [Hadean stage](https://en.wikipedia.org/wiki/Hadean); everything below this message has to undergo intense transformations to achieve a more stable shape. Below are very roughly sketched areas. They are quite unreadable. If they don't make sense to you, it's likely because they don't make sense at all, yet.**

- We need to express change.
- See communication and transformation as one operation. Computing is communication and transformation. And communication and transformation blend into each other.
- Storage is just communication onto certain components that decide to keep the information. CPU registers are immediately reused, RAM also quickly deleted.
- Single model: call and response. Both the call and the response themselves are data. They are 1 to 1, one part makes the call and another one responds.
- Actually see it as a hash: call & res

```
call @foo
res bar
```

We remove a great obstacle to understanding computing: implicitness, being blind to the process of transformation.

Things that can be modelled as that:
- API call.
- Function call.
- TCP handshake.
- CPU call.
- OS call.

- see the data at every level: coming in, at each transformation, going out. That's why we use logs! That's why layers are helpful!
- the basic call is reference. everything is based on reference. we use a name (or rather, a path) to refer to something: whether data we want to get into another place (path), or where we want a result saved.
- there are other calls for basic operations.
- a call is a list of one or more calls.
- calls access data through reference calls.

   - @ as place
   - basic model: call and single response
   - communication and transformation as one
   - can pass a hash as path if the function is expecting a hash? or just prepend with @. Then no need for @foo@bar
   - @ generates more calls
   - understand how a computer works, this goes on top of the flat next, but a computer still has a notion of calls at the lowest level
   - State of a component is the data inside the component at a point in time.

calls are time that happen in the dataspace. the data is the space, the calls are the time and therefore transform space itself. data and space make each other.

tcp/ip

call waits, then gets a result. could be without waiting, without getting a result, or multiple things getting called. but we're going to go with this one.
- callres is interface, the stuff to the right is impl.

call expands to one or more calls.
how to have a nested path with @ and then pass more args? what about @ bla bla @, rather than @bla@bla? not sure. @ as an almost parenthesis. convention: always pass a single argument. but calls can access more data through calls. and they access their args also via a call.
lisp without parenthesis. single argument.
call happens inside the dataspace!
communication gives agency, even if it's on the same computer

problem: express change. we need an unified model for transformations.
all change happens through communication.
we assume that communication happens.
Communication in the Shannon sense is done one way. call and response model, it can all be understood like that.
no, not even. call.
call is data received by
call can be a function call, a call to the OS, over the network. it's all the same.
Requests and responses are done through the network; the network belongs to the "outside" of the system.

call represents transformation and communication.
call goes downstream, response goes upstream.

call changes data in receiver. can be 1 or n. then you have possible wait to acknowledgement. This is return; the acknowledgment is also information that changes something in the sender. Use this mechanism to express all computation. These calls represent change. Draw the line at computer instructions.

storage is a matter of timescale. while processing a call, data is stored in API. but that doesn't outlive the call.
side effect as a call that changes what you consider durable data that is somewhere else in the space where the response is written on the caller.

can see the final result of the call or can see all the intermediate calls.

call goes beyond csp and actor. more simple. three examples: computer instruction (without even assembler), function call inside a hll and an API call.

When you make a call, you allocate. Or rather, with the response, you call the storage.

the call gets expanded. nested calls also get expanded. but the expansion doesn't overwrite. rather, it creates a double entry of call and value (response as value). inside the call, you see what got called and the nested calls, including references. so the result really is more data, all expanded. there's no overwriting, there is expansion. implicitly, the system is looking for the value of the hash at that location, rather than the whole thing. literals are their own values.
in a nutshell: the expansion is also data.

the call is the essence of pillar 3: see the effects as 1) expansions; 2) the subcalls as part of the same mechanism.
the call is data that represents communication and transformation of data. from, to. can have multiple tos. A single to can be a dispatcher too.

if we use it at this level, then we need both wait and return value. control is the wait, the return value is the data.

The traditional approach: input, program and result. For now, let's ignore the program and focus on the input and result, which are data. The focus is generally on those two, at best. The intermediate steps are not shown, except in logs or debugger.

- Logs are necessary as long as we're doing "blind manipulation of symbols" (cannot remember the origin of that quote).

explicitness gives feedback at every step.

- REST is great because it is about sending data for changes. Changes represented as data.
- Microservices give you more rest. Corba also. Vs rpc; rpc can be represented as data, but less contractual.

This is why REST is better than non-REST, why microservices are more tractable than monoliths.

Calls are the transitions.


Communication as basis.
Read is write. get is a call. consider the data at rest as a queryable surface. there's no data in itself, only data that you can query. a read is a write on the readers end. a transformation that is symmetric in the read and write perhaps.

request model of data transformations:
- a component has a set of endpoints. component + endpoint give you an URL (universal resource locator).
- - there's then the request data itself.
   - http: request headers, body.
   - sql: query.
   - fs: operation + data.

responder or surface?

see turing machine; a cpu; a high level language.

You can see calls as time, and data as both space and matter. Space We don't care about empty memory, so we conflate space and matter. Change can only happen with time; so we can conflate change and time, and say that calls are time.

### Pillar 4: code is data

we already have code as data, because of call & res.
- the essence is sequence, the machine keeping on going. return/done makes it stop. then you have jump, which is cond. loop is repeated jumps. error/recover is a special pattern that's really a conditional. and voila, you have everything to express a procedure!
- a call is a sequence of calls.
- The name is sequence. Alternatives: program, function, flow. but it is sequence.
- sequence also maps perfectly well to what a computer does.

- Higher level languages let you focus on data at a human level.
- The data from the call changes the sequence into more calls.
- Calls can be self-referential: recursion. Avoid Whitehead and Russell's mistake.

Height of level is determined by looking who calls who. Low level is usually called, high level is usually the caller.
Levels where you draw lines have sublevels down to a single chip operation.

a flow as a sequence.

quote two problems are two legs:
the problem with expressions: they are not automatically referenceable from outside of their immediate context. solved by pillar 3.
the problem with statements: they are not data. solved by pillar 4.

- then there's what happens inside the component. only see what happens with regards to the other components. inner data mappings are irrelevant or fold. The essential computing model:
   - Call as sequence of calls.
   - Variable subsitution as call.
   - Conditional.
   - Loop as conditional.
   - Errors: the essence is that they jump up many levels, through a different channel than the return. It can be seen as a conditional return based on value.

- Dataspace: access vs control. Open access, use control to determine when to block.

### Pillar 5: interface is code

interface is code, therefore data.
this is all great for backend, but what about interfaces?
An interface is a way for a human to interact with software - always through hardware.
interface mapped to state! see the data being displayed and the possible transformations.

reactivity comes here. @ is reactive, when the references change, things are re-run. internally this is implemented as a loop over subscribers.

reactivity is no mere gimmick, there's something deeper: autopoiesis. when our perception changes, everything that that perception is based upon also changes in ourselves.

Identity is tackled here, because this is where you can have an entrypoint for humans. Identity as data.

## How to test the (hypo)thesis of this treatise

- inverse relationship between data hiding and system quality and ROI
- importance of observability
- security

## Applications of the theory

### Team organization

For creation of general DIS:
- Any analytically capable person can read and write these data sequences. Focus on analysis and [organizational principles](https://prog21.dadgum.com/177.html). These data sequences define 90-99% of the implementation and its tests. Working on the data sequences directly is the most effective way to create a simple and reliable system.
- Specialization works for certain areas: interface design, tool making, data science.

### Understanding existing systems

- put the dbs first into dataspace: the data itself, and the constraints too
- capture logs of operation, all inputs and outputs and put them in the space too. see the transitions. feel free to add more logging of the data.
- use the system for real, eschew unit tests. go with the real thing. unit tests are only useful in highly documented, high quality systems.
- network analysis to see who's who.
- go 80/20 rather than all in
- valuable code is only that that performs nontrivial operations, and can usually be isolated.
- feed data to an llm to find patterns for you too.
- to connect systems: see paths as relative.

### Designing and implementing new systems

- design data at rest
- design data transitions
- build up surfaces for those data transitions

### Running systems

Logs are data. Keep them. Query them with the same mechanisms.

### Security

It is about data, not about perimeter; it's zero trust but naturally. And kerchoffs principle: no unnecessary layers.
Control is still key.

auth as extra info. zero trust as checking the auth credentials with someone you trust. yet, how do you know that someone you trust is there? if https, it's not zero trust. it'd have to be through a key exchange, but what about getting the keys in the first place? you need to trust. if you're in the same place and then you separate, then you had a trust network that then got partitioned.

### On scaling, consistency and parallelism

- Distributed and parallel: consistency. Scalability with that assured is trivial (throw more nodes in), except for the "inside api" problem that Hickey points out.

understanding CAP: when distributed surface (distributed as amenable to experiencing partitioning) receives data, it either rejects (rejection as the lack of upating and also reading, indicating that that's not data) and presents/maintains consistency, vs remains available and has either temporary or permanent inconsistency. consistent system, in a partition does not present or update state, only stores it.

### Quality

Implementing the Toyota Production System
- autoactivation
- flow backwards, with reactive

testing
- convergence to mathematical proof
- to generate, you must understand the order of validations.
- see errors as valid outputs, validate all the way.

Simple systems are amenable to proof.

## License

TODIS is written by [Federico Pereiro](mailto:fpereiro@gmail.com) and released into the public domain.
