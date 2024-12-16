# The Organization of Digital Information Systems

> "The fundamental problem of communication is that of reproducing at one point either exactly or approximately a message selected at another point." -- [Claude Shannon](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf)

> "To a great extent the act of coding is one of organization." -- [James Hague](https://prog21.dadgum.com/177.html)

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

Software systems are DIS. Their usefulness is conducted solely by their capacity to communicate, store and transform data. If a software system was replaced overnight with another software system that communicated, stored and transformed data in the same way as the first one, nobody would notice until the time came to actually modify the system. The actions performed by the system are ultimately valuable solely for their capacity to communicate, store and transform data.

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

Our contemporary attitude towards software is focused, perhaps naturally, on software itself, and not on the data which flows through it and which justifies the existence of software itself. But it is perfectly possible to see logic as the negative impression (just like a picture taken with film has a [negative](https://en.wikipedia.org/wiki/Negative_(photography))) of the data flows it enables.

When the data is not seen, the trivial becomes difficult and the nontrivial impossible.

Data itself is simple and can be directly seen. By using data to understand and make a DIS, we can find the simplest possible expression of the system that will get the job done.

This is the central thesis of this treatise. We'll explore now how to make this a reality through five practical concepts, fancily called *pillars*. Each pillar removes an obstacle to seeing the data flowing through an information system.

## The five pillars

1. **Single representation of data** (overcomes not being able to look and describe data in unambiguous terms).
2. **Single dataspace**. (overcomes having parts of the system floating around instead of being part of one whole picture).
3. **Call and response** (overcomes the invisibility of how data is transformed inside a DIS).
4. **Logic is what happens between call and response** (overcomes doubts about the shape of the solution for a clearly specified problem).
5. **Interface is logic** (overcomes separateness between system and user).

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
              isbn 978-0-394-42814-7
              title Orientalism
```

**A table in a [relational database](https://en.wikipedia.org/wiki/Relational_database)**

```
books 1 author "Edward Said"
        created 2024-10-23T20:24:15.936Z
        id 1234
        isbn 978-0-394-42814-7
        title Orientalism
      2 author "Michel Houellebecq"
        created 2024-10-23T20:25:22.411Z
        id 1235
        isbn 978-2-08-147175-7
        title Serotonin
      3 author "Paul Graham"
        created 2024-10-23T20:30:44.602Z
        id 1237
        isbn 978-0130305527
        title "On Lisp"
```

**The data in the registers of a [6502 processor](https://en.wikipedia.org/wiki/MOS_Technology_6502)**

```
Accumulator 00110100
X 01100001
Y 11001010
StackPointer 11110111
ProgramCounter 1100001010101011
StatusRegister 00100101
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
        created 2024-10-23T20:24:15.936Z
        id 1234
        isbn 978-0-394-42814-7
        title Orientalism
      2 author "Michel Houellebecq"
        created 2024-10-23T20:25:22.411Z
        id 1235
        isbn 978-2-08-147175-7
        title Serotonin
      3 author "Paul Graham"
        created 2024-10-23T20:30:44.602Z
        id 1237
        isbn 978-0130305527
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
                        created 2024-10-23T20:24:15.936Z
                        id 1234
                        isbn 978-0-394-42814-7
                        title Orientalism
                      2 author "Michel Houellebecq"
                        created 2024-10-23T20:25:22.411Z
                        id 1235
                        isbn 978-2-08-147175-7
                        title Serotonin
                      3 author "Paul Graham"
                        created 2024-10-23T20:30:44.602Z
                        id 1237
                        isbn 978-0130305527
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
"Main Database" books 3 isbn 978-0130305527
```

If this is still not clear, you could interpret it like this:

```
"Main Database" -> books -> 3 -> isbn -> 978-0130305527
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
contents 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
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
contents 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
path C:\Users\dmr\clang\hello.c
```

We can go even one step further and represent the file like this:

```
C:\Users\dmr\clang\hello.c 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
```

A better way to do it is to split the path into hashes (that is, into a path), and add the contents as the last item.

```
C Users dmr clang hello.c 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
```

Using this structure allows us to group files that are in the same directories in a way that's easy to see. For example, if we have a second file in the same directory, we could represent it like this:

```
C Users dmr clang hello.c 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
                  indefatigable.c 001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111001011100110100000111110000010100111011001101111011010010110010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111011101101000011010010110110001100101001000000010100000110001001010010010000001111011011111010111110100001010
```

Now, where *is* this main hard disk? Hard disks must be attached to a computer in order to be accessible. In the context of DIS, these computers are usually called [servers](https://en.wikipedia.org/wiki/Server_(computing)), to distinguish them from computers to which a user has direct physical access. Let's call this server the `Main Server`. Then, we can represent our two files like this:

```
"Main Server" C Users dmr clang hello.c 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
                                indefatigable.c 001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111001011100110100000111110000010100111011001101111011010010110010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111011101101000011010010110110001100101001000000010100000110001001010010010000001111011011111010111110100001010
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
"Main Server" C Users dmr clang hello.c 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
                                indefatigable.c 001000110110100101101110011000110110110001110101011001000110010100100000001111000111001101110100011001000110100101101111001011100110100000111110000010100111011001101111011010010110010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111011101101000011010010110110001100101001000000010100000110001001010010010000001111011011111010111110100001010
                          music hits1985.csv 01010010011000010110111001101011001011000101010001101001011101000110110001100101001011000100000101110010011101000110100101110011011101000010110001010111011001010110010101101011011100110010000001100001011101000010000000100011001100010000101000110001001011000100001101100001011100100110010101101100011001010111001101110011001000000101011101101000011010010111001101110000011001010111001000101100010101110110100001100001011011010010000100100000011001100110010101100001011101000111010101110010011010010110111001100111001000000100011101100101011011110111001001100111011001010010000001001101011010010110001101101000011000010110010101101100001011000011001100001010001100100010110001001100011010010110101101100101001000000110000100100000010101100110100101110010011001110110100101101110001011000100110101100001011001000110111101101110011011100110000100101100001101100000101000110011001011000101011101100001011010110110010100100000010011010110010100100000010101010111000000100000010000100110010101100110011011110111001001100101001000000101100101101111011101010010000001000111011011110010110101000111011011110010110001010111011010000110000101101101001000010010110000110011000010100000101000110100001011000100100100100000010101110110000101101110011101000010000001110100011011110010000001001011011011100110111101110111001000000101011101101000011000010111010000100000010011000110111101110110011001010010000001001001011100110010110001000110011011110111001001100101011010010110011101101110011001010111001000101100001100100000101000110101001011000100100100100000010001100110010101100101011011000010000001100110011011110111001000100000010110010110111101110101001011000100001101101000011000010110101101100001001000000100101101101000011000010110111000101100001100110000101000110110001011000100111101110101011101000010000001101111011001100010000001010100011011110111010101100011011010000010110001000100011000010111001001111001011011000010000001001000011000010110110001101100001000000010011000100000010010100110111101101000011011100010000001001111011000010111010001100101011100110010110000110010000010100011011100101100010101000110100001100101001000000101000001101111011101110110010101110010001000000110111101100110001000000100110001101111011101100110010100101100010010000111010101100101011110010010000001001100011001010111011101101001011100110010000001100001011011100110010000100000011101000110100001100101001000000100111001100101011101110111001100101100001100100000101000111000001011000100010101110110011001010111001001111001011000100110111101100100011110010010000001010111011000010110111001110100011100110010000001110100011011110010000001010010011101010110110001100101001000000111010001101000011001010010000001010111011011110111001001101100011001000010110001010100011001010110000101110010011100110010000001100110011011110111001000100000010001100110010101100001011100100111001100101100001100100000101000111001001011000100110101101111011011100110010101111001001000000110011001101111011100100010000001001110011011110111010001101000011010010110111001100111001011000100010001101001011100100110010100100000010100110111010001110010011000010110100101110100011100110010110000110011000010100011000100110000001011000100001101110010011000010111101001111001001000000110011001101111011100100010000001011001011011110111010100101100010011010110000101100100011011110110111001101110011000010010110000110001
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

While CSVs are a very expressive and widely used way of representing structured information, a great deal of structured information is nowadays stored in databases. Databases are *computer programs* that store data using files; but they do it in a more involved way that provides the following features:

- Efficiency: you can access a single value, rather than getting the entire file.
- Validation: you can check whether incoming data has a certain shape before storing it.
- Locking: if two users want to save a value at the same path at the same time, the database makes sure to process the requests one at a time.
- Queries: you can construct specific enquiries about data which will get you the right results efficiently.

For practical purposes, there are two families of databases: [relational databases](https://en.wikipedia.org/wiki/Relational_database) (also called SQL databases) and [non-relational databases](https://en.wikipedia.org/wiki/NoSQL).

Relational databases date from 1970 (!) and are tremendously powerful. Their power stems from their quite rigid structure, as well as from the possibility of creating *relations* between records. Overall, a relational database is composed of tables with rows and columns. This can be directly modeled in fourdata as follows:

- Table: list
- Row: hash

For example, taking some books from the example at the top:

```
"Main Database" books 1 author "Edward Said"
                        created 2024-10-23T20:24:15.936Z
                        id 1234
                        isbn 978-0-394-42814-7
                        title Orientalism
```

We could interpret `books` to be a table of "Main Database". We have here one row with five columns (`author`, `created`, `id`, `isbn` and `title`). Relational databases are called *relational* because they naturally express relationships between different tables. For example:

```
"Main Database" books 1 author "Edward Said"
                        created 2024-10-23T20:24:15.936Z
                        id 1234
                        isbn 978-0-394-42814-7
                        title Orientalism
                users 1 id fpereiro
                purchases 1 book 1234
                            created 2024-11-04T22:44:10.196Z
                            user fpereiro
```

If we look at `purchases 1`, we can see that the book purchased has `book 1234` and `user fpereiro`. Since we have a book with `id 1234` ("Orientalism") and a user with id `fpereiro`, relational databases can *join* this data to express the fact that this purchase involves both this particular book and this particular user. This can be done quite expressively using [SQL](https://en.wikipedia.org/wiki/SQL), which is a query language.

For now, it is enough to have a direct mapping from relational databases to fourdata: this allows us to put relational data at rest into our dataspace.

Non-relational databases can also be represented in dataspace. The most common one, [MongoDB](https://en.wikipedia.org/wiki/MongoDB), stores data in collections of [JSON](https://en.wikipedia.org/wiki/JSON) objects. To map this to fourdata, we can simply make each collection a list of items.

```
"Mongo Database" visitors 1 date 2024-11-11T16:42:01.322Z
                            ip 140.28.111.224
                          2 date 2024-11-11T16:42:02.299Z
                            ip 220.49.66.236
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

Sorted sets can be represented with a list of hashes, each containing a score and a value.

```
"sorted set" 1 score 1000
               value foo
             2 score 1001
               value bar
```

The above should be enough for almost all possible data that is at rest. In exceptional circumstances, it can be useful to represent lower level data. For example, we could use fourdata to represent the contents of memory addresses, if we're doing low level programming.

```
0x1A3F" 010010000110010101101100011011000110111100000000000000000000000
0x1A5F" 010101110110111101110010011011000110010000000000000000000000000
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

Earlier, we defined a DIS as something that communicates, transforms and stores digital data. In this pillar, the central one, we will find a way to express communication and transformation of data *using data itself*.

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

How this happens in a DIS can be quite involved. For example, nowadays a typical (though not at all universal) way to send messages between systems is to use the following stack:

1. Create a JSON payload with the data.
2. Wrap it in a HTTP request.
3. Send it through [TCP](https://en.wikipedia.org/wiki/Transmission_Control_Protocol).
4. Let TCP use [DNS](https://en.wikipedia.org/wiki/Domain_Name_System) to find system 2 and [IP](https://en.wikipedia.org/wiki/Internet_Protocol) to send the pieces of the message.

Despite its apparent complexity, communication between systems is essentially a solved problem. Most of the time, we can rely on system 1 being able to send messages to system 2 and system 2 receiving them.

We now have to deal with data transformation. The core idea is that we can understand a transformation as a combination of a *call* and a *response*. Let's extend the previous example:

```
call from "system 1"
     message hello
     to "system 2"
response "how are you?"
```

Note that the response doesn't contain `from` or `to`, since it's clear that they are the same as those of the call, only reversed. All that comes back is data.

**The combination of a call and a response can be used to express any data transformation**. In the example above, we could consider that the "hello" sent by system 1 gets converted into a "how are you?".

Now, Consider the following example:

```
call from "math formula"
     message 1 10
             2 10
     to +
response 20
```

Imagine that, rather than a system, we had a particular math formula that was in need of summing 10 and 10. The formula itself doesn't have the means to sum two numbers, but there's another part of the system (let's call it `+`) that knows how to sum a list of numbers and return that result.

In the example above, then, the math formula sends a call containing a list with two elements (10 and 10) to `+`. Then, `+` responds with `20`.

If computation is purposeful communication and transformation of data, we have stumbled on a simple way to represent computation: two-way communication. From now on, we will use the term *computation* to refer to the combination of communication and transformation.

Communication, as defined by Shannon at the top of this treatise, is one way. It is curious that we actually can express computation by adding communication on the way back. This also requires the response to contain data that is different from that originally sent in the call. The tranasformation happens between the call and before the response, *inside* the receiver of the call.

Let's simplify the representation of the call a bit more. In general, the "from" is already known, because we have the context of who's the caller. So we can remove that.

```
call message 1 10
             2 10
     to +
response 20
```

Let's now simplify it further: we could make the call to be a hash where its only key is the receiver, and its value is the content of the call. We can also shorten `response` to `res`.

```
call + 1 10
       2 10
res 20
```

Much trimmer. But we have a problem. The above could still be interpreted as just data at rest, not as computation. We need a *special character* to indicate communication and transformation -- that is, we need a special character to represent computation. So we are going to choose `@`.

```
@ + 1 10
    2 10
res 20
```

But we can make this even leaner by replacing `res` with `=`, which has [for centuries been associated to a result](https://en.wikipedia.org/wiki/Equals_sign). The response to the call is equivalent to its *result*, or its *value*. So this is how we will represent the call and its response:

```
@ + 1 10
    2 10
= 20
```

The structure of a call and a response, generally, is then:

```
@ destination message
= response
```

The message, also called *input*, *parameter* or *argument*, is the data that is passed along on the call: the message. The response (also called *result*) is the message that comes back from the destination to the source.

Most computation happening inside a DIS is opaque to those who design it: while working with the system, they usually have to place *logs* to show what the results are at certain places in the program. By using the call and response model, and being able to see the results of every call, we remove a major obstacle to understanding DIS: the implicitness of intermediate results. The traditional approach to computing is to feed an input to a program and then read its output. The intermediate steps are not shown, except in logs or a debugger.

In the approach we are prsenting here, every call and response is displayed as data, so there's no longer any need to guess (or find out, by putting a log and making the call again). The results, at every level, are right there in the dataspace.

How does this connect with the previous two pillars? Concerning pillar 1, we're representing communication and transformation of data within fourdata in all of the examples above, always using numbers, texts, lists and hashes. The connection with pillar 2, however, is more subtle. Let's illustrate:

```
"system 1" "math formula" @ + 1 10
                              2 10
                          = 20
```

The above computation then is in the dataspace, inside `system 1` and `math formula`. In this model, computation does not float around without a context or a place, but rather is always embedded in the dataspace, at a particular location.

Now, what would happen if one of the values we pass to `+` wasn't always `10`, but rather was a reference to another part of the dataspace? We could represent it like this:

```
"system 1" "math formula" @ + 1 @ widgets
                                = 100
                              2 10
                          = 110
           widgets 100
```

Note that `@ widgets` is a reference to the `widgets` variable inside `system 1` - this is a useful convention. The value of widgets is `100`. We then see that the math formula makes a call to `+` sending both `@ widgets` (which is `100`) and `10`. That produces the result `110`.

Also note that we convert calls into values going right to left. The detail is always to the right, while the context is to the left.

Using the call and response model, we can represent any of the following:

1. A reference to a variable:

```
"system 1" value @ widgets
                 = 100
           widgets 100
```

2. A function call

```
"system 1" "math formula" @ + 1 10
                              2 10
                          = 20
```

3. A database query:

```
"system 1" users @ "Main Database" "select * from users"
                 = 1 id 1
                     username deadmau5
                   2 id 2
                     username faxingberlin
```

4. An HTTP call:

```
"system 1" books orientalism @ http headers Accept application/json
                                            User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
                                    host example.com
                                    method GET
                                    path /api/books/1234
                                    type HTTP/1.1
                             = code "200 OK"
                               headers Content-Length 83
                                       Content-Type application/json
                               body author "Edward Said"
                                    id 1234
                                    isbn 978-0-394-42814-7
                                    title Orientalism
```

5. An [operative system call](https://en.wikipedia.org/wiki/System_call).

```
"system 1" "hello world" @ os readFile encoding utf-8
                                       path C Users dmr clang hello.c
                         = 0010001101101001011011100110001101101100011101010110010001100101001000000011110001110011011101000110010001101001011011110010111001101000001111100000101001101001011011100111010000100000011011010110000101101001011011100010100000101001001000000111101100001010001000000111000001110010011010010110111001110100011001100010100000100010010010000110010101101100011011000110111100101100001000000101011101101111011100100110110001100100001000010010001000101001001110110000101000100000011100100110010101110100011101010111001001101110001000000011000000111011000010100111110100001010
```

6. The beginning of a TCP handshake.

```
@ SYN client_ip 192.168.1.100
      client_port 12345
      server_ip 192.168.1.200
      server_port 80
      seq 1000
= ACK pending
```

7. An [assembler instruction](https://en.wikipedia.org/wiki/Assembly_language).

```
@ mov eax 0x1A3F
= 00100001
```

8. A [microcode instruction](https://en.wikipedia.org/wiki/Microcode).

```
@ store eax ALU_input
= 00100001
```

The eight examples above show different levels of a DIS, with each level being increasingly detailed compared to the previous one. Note, however, that the concept of call and response, together with fourdata and the unified dataspace, can describe the essence of each of its operations. Using this model, we can let go of the distinctions between function calls, remote service calls and even user interactions. The same model can describe them all.

Quite interestingly, the concept of a call and a response requires both space and time. Space is required because there is a distance between the caller and the responder, which separates them.

Time is required for the call to reach the responder, as well as for the responder to transform the call into a response, and then its response to be received by the caller. Call and response traverse both space and time; from a philosophical perspective, we could perhaps intuit that if data creates the space, calls and responses create time. Time, in this framework, is the process of change within the dataspace. Each call initiates a transition from one state to another, and each response finalizes that transition. The dataspace at rest defines a single moment in time, while a sequence of calls and responses reveals the flow of time through successive changes in the data.

More practically, if calls and responses are not instantaneous, then we might have to wait for them. We can then have calls that have not been (yet) responded, and represent them like this:

```
"system 1" books orientalism @ http headers Accept application/json
                                            User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
                                    host example.com
                                    method GET
                                    path /api/books/1234
                                    type HTTP/1.1
                             = PENDING...
```

That intermediate state which expresses an ongoing operation is as much a valid response as what will come afterwards. That intermediate result is placed there by the caller itself. Interestingly enough, when the response comes back, we can understand that it will overwrite `PENDING...`, since it will replace it completely in the dataspace. This is akin to *forgetting* a previous value that once was in the dataspace.

It is also possible to remember every single change that happened in the dataspace, effectively never forgetting anything. This is a decision to be taken as part of the design of a system. At this stage of the argument, what's important is to know that we can choose to selectively remember and to forget. A system that remembers accretes changes, while a system that forgets overwrites changes.

It is also possible to represent errors as responses.

```
"system 1" books orientalism @ http headers Accept application/json
                                            User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
                                    host example.com
                                    method GET
                                    path /api/books/1234
                                    type HTTP/1.1
                             = error code "404 not found"
                                     body "No such book"
```

Errors are valid responses, are also data, and are also part of the dataspace.

At every point in time, however, the dataspace is complete. Even if the system is "between" calls, those intermediate states are also valid. And if some call has encountered an error, those error states are also valid. Most digital information systems are in constant flux, so they are always in between calls: by thinking about these states with the same process with which we think about the system at rest (with no calls), we can more clearly understand flux.

It is interesting to think that what we normally call an *interface* is really a call: the start of an interaction. And what we normally call an *implementation* is what happens between the call and the response. The call is to the left, the implementation is to the right. We can also use the terms *downstream* and *upstream* to mean that calls go *downstream* and responses go back *upstream*.

In contrast with other conceptual frameworks to express computations, such as [CSP](https://en.wikipedia.org/wiki/Communicating_sequential_processes) or the [actor model](https://en.wikipedia.org/wiki/Actor_model), our framework doesn't consider certain operations (calls) as internal vs external from a global perspective. A call always sees its response as an external process, even if it happens on the same computer and even within the same program. If you zoom out and look at calls that are upstream of other calls, you are lumping the subcalls as part of one response. This is how you abstract the detail into a single value. In this way, the outside or inside only depends of your point of view. This also allows to go beyond the distinction between an event and a primitive process, treating everything to be a call and a response. In other words, in this framework, calls and responses are [fractal](https://en.wikipedia.org/wiki/Fractal) or [self-similar](https://en.wikipedia.org/wiki/Self-similarity). A call triggers a response that is itself made of calls. The advantage of this approach is that it is just simpler, requiring very few concepts and always having the same structure.

This framework also allows us to go beyond the concept of state as a special type of data. If the "system" is a part of the dataspace, the state of the system (or of a subsystem) is also a part of the dataspace. Everything exists within the same dataspace, so the data in the system is indistinguishable (or rather, integrated) with the rest of the system.

We have covered a lot of ground in this pillar. In a nutshell, we have found that the combination of a call and a response can express data change of any kind, just by using data itself.

In the next pillar, we will understand logic, which is what happens between a call and a response.

### Pillar 4: Logic is what happens between call and response

Armed with the pattern of call and response, we can now explore what happens between one and the other. Any call happening in a DIS will have a [deliberate](https://en.wikipedia.org/wiki/Teleology) response. The purpose of a call is to become a response. Logic is how this transformation happens. In other words, logic is intentional transformation of data.

The original definition of [logic](https://en.wikipedia.org/wiki/Logic) is concerned with correct reasoning. In the context of a DIS, logic is something rather more basic: given a purpose for a certain call, we want to be able to express it in terms of a number of simpler calls. Eventually, those simpler calls become tiny operations at the [CPU level](https://en.wikipedia.org/wiki/Central_processing_unit). At that point, the software people (the author included) shrug, declare "[here be dragons](https://en.wikipedia.org/wiki/Here_be_dragons)", and leave those details to the hardware makers.

Logic is also usually called *code*, a term which comes from [machine code](https://en.wikipedia.org/wiki/Machine_code) (which is a set of low-level calls that can be made in a computer). But we'll just call this logic, not code.

It is my contention that the main elements of logic, in the context of a DIS, are five:

1. Reference: the destination of a call.
2. Sequence: the calls made by a call.
3. Conditional: the choice between sequences.
4. Loop: the conditional repetition of a sequence.
5. Error: a special type of conditional response.

For all of us who are fearful of programming, even those of us who practice it daily, it can be liberating to discover that essentially all logic can be understood through these elements. The diverse and generally abstruse syntax of programming languages hides the fact that most logic is based on very few, intuitively understandable elements. I will spend the rest of this pillar showing how that is the case.

The first three elements are essential, [irreducible](https://en.wikipedia.org/wiki/Irreducibility_(mathematics)).
- Without *reference*, we have no way to represent the destination of a call. If every value in the dataspace refers only to itself, then we cannot establish relationships between parts of the system.
- Without *sequence*, without ["keeping on keeping on"](https://en.wikipedia.org/wiki/Keep_On_Keeping_On) and allowing a call to make multiple calls (calls which, themselves, will also make further calls) and collecting their responses, our DIS cannot go anywhere.
- Without being able to choose one path or the other based on a *conditional* (which is some data, a part of the dataspace), our DIS would always be doing the same calls, no matter what those calls responded. Without conditionals, our logic would always do the same thing, every time.

This can be readily seen in the [Turing Machine](https://en.wikipedia.org/wiki/Turing_machine), which is an universal model of computation.

The machine has an infinite tape divided in discrete pieces. If the tape is infinite in one way, we can represent it with a list, where each key is a position in the tape, and each value is the actual value written in the tape. For example:

```
1 ə
2 ə
3 0
4 ""
5 0
```

The machine is always scanning one particular part of the tape. We can represent this as its *current position*

```
"current position" 1
tape 1 ə
     2 ə
     3 0
     4 ""
     5 0
```

There's always a current *state of mind*, called the *current configuration*. You could think of this as a *sequence*. Any of these sequences will always do the following:

1. Write something to the tape (or write nothing).
2. Move the tape to the left or right (or keep it in place).
3. Change to another state of mind (or sequence).
4. Go back to step 1.

But what a sequence does depends on the symbol at the current position of the tape. That is, the writing, moving and calling behavior of the current configuration will be *conditional* to the symbol currently being scanned.

If we start with the Turing Machine just as it enters a new configuration, we'll start with a conditional: *what is the symbol on the current position of the tape?* Depending on that, the machine will execute one sequence or perhaps other. And when the sequence is complete, the machine will switch to *another configuration*: this can be seen as a call, where the new configuration is the destination. In a nutshell: conditional, sequence, reference.

The other two elements of computation, loops and errors, are niceties much in the same way as a roof and electricity are nice. Not absolutely essential for human life, but making it much easier and extending its capabilities. The essence of loops is conditional repetition of a sequence over a list or a hash; the essence of errors is conditional jumps through many levels, to avoid the burden of having to check each response to see if it is an error or not. Interestingly enough, errors are most useful as stoppers of sequences.

We'll now go element by element and explain it in more detail.

#### Reference

A reference is the destination of a call. We could think of destinations as [links](https://en.wikipedia.org/wiki/Hyperlink).

The simplest type of reference is that which points to a value that contains no calls. For example:

```
"copy of widgets" @ widgets
                  = 20
widgets 20
```

`copy of widgets` makes a call to `widgets`. `widgets` itself is no more than the value `20`. This has the effect of setting the value of `copy of widgets` also to 20.

Now, this type of reference is so simple that it doesn't require a message! If you remember, back in pillar 3, a call is defined by this structure:

```
@ destination message
= response
```

But when a reference points to a mere value, no message is necessary. If `widgets` is `20`, nothing we can say to it will make it change its value. This is because `widgets` itself contains no calls, just `20`. Therefore, for references to parts of the dataspace that do not contain calls, we can have this type of structure:

```
@ destination
= response
```

Calls without a message are also considered calls.

If we want to reference a part of the dataspace that is nested, we do need a message.

```
"copy of widgets" @ data widgets
                  = 20
data widgets 20
```

In the call above, we first reference `data`. The value of `data` is `widgets 20`. But the call is `data widgets`; the message of that call, `widgets`, is what makes the response `20`.

If we add a reference to `copy of widgets`, we will also get the same value.

```
"copy of copy" @ "copy of widgets"
               = 20
"copy of widgets" @ data widgets
                  = 20
data widgets 20
```

Things get more interesting when we reference a part of the dataspace that also contains a call.

```
@ + 1 10
    2 10
= 20
```

In the example above, the destination is `+`. Like with `widgets` above, `+` is not just the actual character `+`. Rather, `+` is a reference to another part of the dataspace.

```
+ ...
twenty @ + 1 10
           2 10
       = 20
```

We'll get to the value of `+` (currently represented as `...`) when we explain *sequence*.

In our framework, what in common parlance usually called *variable reference* and *function invocation* share the same mechanism: a call. It is `@` what transforms the value to its right into a reference.

How that reference is *resolved* is a matter of convention. "Resolving a reference" means "how to find its location". For now, we can use the following logic:
- From the place where the call is made, we go one level up (left) and try to find it. If it's not there, we repeat the process of going one more level up to find it.
- If we have gone all the way to the left and we can't find it, we obtain an empty text.

Here, the reference to `widgets` will go up one level until it finds `widgets`:

```
hello @ widgets
      = 20
widgets 20
```

Here, the reference to `widgets` will go up three levels until it finds `widgets`:

```
hello there handsome @ widgets
                     = 20
widgets 20
```

If there are multiple `widgets`, we will reference the closest one:

```
hello there handsome @ widgets
                     = 20
      widgets 20
widgets 30
```

Note that the outermost `widgets` wasn't reached!

Similarly, if `widgets` is not reachable by going outside from the call, it is unreachable.

```
hello @ widgets
      = ""
nested widgets 30
```

We have now dealt with *references*, which allow us to find a destination; we have also seen how, in simple cases, references can be turned into values. But what happens when we are referring to a more involved transformation, where other calls happen as a result of the call we are making? Enter sequence.

#### Sequence

A sequence is a *list of calls*. When a sequence is called, this list of calls takes place in order to create the response.

The concept of sequence, quite wonderfully, works at any level of abstraction. It can describe a large operation in terms of a list of steps that can intuitively be understood sequentially. And it can also describe what a computer does at its lower level: execute one instruction (call) after the other.

Alternative names for a *sequence of calls* are *function*, *flow*, *procedure*, *operation*, *definition*. They all refer to the same concept. The mathematical concept of a *function* is mostly concerned with establishing a relationship between a set of messages (inputs) and responses (outputs). Here we are interested in the calls inside the sequence that make it possible to respond with a certain value when another value (the message) is received by the call.

A good analogy to illustrate the concept of sequence is a recipe. A recipe of the cake is not a cake. Rather, it tells you how you can make a cake. A DIS will give you even more: not only the instructions on how to make the cake, but also the ingredients.

```
"make cake" 1 @ mix 1 @ chocolate 100
                    2 @ flour 500
                    3 @ butter 300
            2 @ bake degrees 200
                     ingredients @ 1
```

In the example above, you can notice that making a cake consists of two steps: mixing ingredients and baking them at 200 degrees (you can also notice that I've never baked a cake). There's two calls made here: `mix` and `bake`. Additionally, there are calls made to `chocolate`, `flour` and `butter` within the `mix` call, presumably to get the ingredients.

We now have a problem, because we don't want those calls to happen when we are writing the sequence. Instead, we want them to happen when another parts of the space calls this sequence. So we need to create a new operator which will "freeze" these calls and only let them happen when the sequence is called. We will use `:`, since it is normally associated with defining something.

```
"make cake" @ : 1 @ mix 1 @ chocolate 100
                        2 @ flour 500
                        3 @ butter 300
                2 @ bake degrees 200
                         ingredients @ 1
```

So `make cake` is not a cake, not even a frozen cake. It is a part of the dataspace that, when called, will respond with a cake.

Now, how do we get a cake when we call `make cake`? We can understand that whatever is responded by `bake`, we will get!

```
"make cake" @ : 1 @ mix 1 @ chocolate 100
                        2 @ flour 500
                        3 @ butter 300
                2 @ bake degrees 200
                         ingredients @ 1
"today's cake" @ "make cake"
               = "delicious chocolate cake"
```

More generally: the response of the last call of a sequence will be used as the response of the entire sequence.

A subtle detail: the call to `bake` references `@ 1`. This references to the first element of whatever list can be found outside of the place where that call is. By going a couple of levels to the left, `@ 1` finds whatever is responded by the call to `mix`. So it is perfectly possible (and actually, generally essential) that a call within a sequence can reference responses from previous calls of the sequence.

Another detail: `make cake` doesn't receive a message! It will always return the same cake. What if we wanted to send a message to it, perhaps specifying the amount of people that will eat it?

```
"make cake" @ : people 1 @ mix 1 @ chocolate @ * 1 @ people
                                                 2 25
                               2 @ flour @ * 1 @ people
                                             2 125
                               3 @ butter @ * 1 @ people
                                              2 75
                       2 @ bake degrees 200
                                ingredients @ 1
"today's cake for 8" @ "make cake" 8
                     = "delicious chocolate cake for eight!"
```

We just snuck in the name of the message in between `:` and the list. It's a bit terse, but feels better than creating something more longwinded.

We're now ready to see the expansion of the sequence, which is what happens between the call and the response. We'll omit the definition of `make cake` (since we've just provided it) and focus on how `today's cake for 8` comes into existence.

```
"make cake" @ : people 1 @ mix 1 @ chocolate @ * 1 @ people
                                                 2 25
                               2 @ flour @ * 1 @ people
                                             2 125
                               3 @ butter @ * 1 @ people
                                              2 75
                       2 @ bake degrees 200
                                ingredients @ 1
"today's cake for 8" @ "make cake" 8
                     : 1 @ mix 1 @ chocolate @ * 1 @ people
                                                   = 8
                                                 2 25
                                             = 200
                                 = "200 grams of chocolate!"
                               2 @ flour @ * 1 @ people
                                               = 8
                                             2 125
                                         = 1000
                                 = "A kilo of flour!"
                               3 @ butter @ * 1 @ people
                                                = 8
                                              2 75
                                          = 600
                                 = "600 grams of butter!"
                         = "A mix of 200g of chocolate, a kilo of flour and 600g of butter!"
                       2 @ bake degrees 200
                                ingredients @ 1
                     = "delicious chocolate cake for eight!"
```

In the example above, the expansion is the value of `"today's cake for 8" :` (notice the colon at the end). We use the colon for two things: for specifying what a sequence is; and also for showing the expansion of a sequence when it gets called. We use the same symbol because definition and expansion are both sides of the same coin. Definition makes expansion possible, and expansion is what makes definition useful.

No doubt the above is not immediately readable, but consider what it shows:
- The entire sequence of `make cake` when making the cake for 8 people.
- The intermediate responses obtained from each of the internal calls.

Note also what it doesn't show: the expansion of the calls to, say, `chocolate`, `mix` or `bake` (or even `+`). These could be shown if they were deemed relevant to what the user is looking at. There are two things that prevent us from showing the expansion to every single call:

- Some calls happen on a different system that doesn't share an expansion, but just returns a response. This can happen for either performance reasons or security reasons.
- The user doesn't care about expanding every call, but rather only those that they want to inspect.

A small trick that can help make expansions more readable is to interpret `@ foo` as if `foo` was a link: blue and underlined. A programming environment can provide this facility; when working in a blackboard, the references of calls can be underlined, to avoid writing so many `@`s.

Before we move to conditional, it is a good idea to realize that the expansion of a sequence is equivalent to computation. The nature of computation is sequential, doing one call, minding its response and then making another call.

We now turn to the third and last essential element of logic, conditional.

#### Conditional

A conditional is just a call. However, it is a special call because, depending on a condition, it will *choose* to expand a sequence depending on a condition.

A condition is something essentially binary: it is either yes or no. In traditional programming environments, these values are called `true` and `false`; but we have no room (nor need) for them. We can simply use `1` for yes and `0` for no.

The simplest conditional is one that has both a condition and a sequence. If the condition is true, then the sequence is called.

```
greeting @ if cond 1
              do @ "make cake" 8
                 = "delicious chocolate cake for eight!"
         = "delicious chocolate cake for eight!"
```

Note a few things:
- We use the call `if` to do the conditional.
- We pass a hash with `cond` (the condition) and `do` (the sequence to call if the condition is true).

Now, the conditional above is a bit silly, because its condition is always set to `1`. This is a bit less silly, particularly if you realize that `party` could change:

```
greeting @ if cond @ party
                   = 1
              do @ "make cake" 8
         = "delicious chocolate cake for eight!"
party 1
```

If `party` was set to `0`, no cake would be made!

```
greeting @ if cond @ party
                   = 0
              do @ "make cake" 8
         = ""
party 0
```

Note that `make cake` was not called! This is precisely why conditionals are essential: they allow us to *not* call a certain sequence.

A second sequence can be passed to `if`, to be called if the condition is *not* met.

```
greeting @ if cond @ party
                   = 0
              do @ "make cake" 8
              else @ "make random healthy dish" 2
                   = "A fresh batch of beetroot soup!"
         = "A fresh batch of beetroot soup!"
party 0
```

Conditionals can be nested:

```
greeting @ if cond @ party
                   = 0
              do @ if @ > 1 @ people
                            = 8
                          2 4
                      = 1
                   do @ "make cake" @ people
                                    = 8
                      = "delicious chocolate cake for eight!"
                   else @ "get more people"
              else @ "make random healthy dish" 2
         = "delicious chocolate cake for eight!"
party 0
people 8
```

Notice that we introduced another call, `>`, which compares two values, and responds with either `0` or `1` depending on whether the comparison was successful or not. In the case above, since we have more than four people, we can go ahead and make cake, instead of getting more people to join the party.

**DEAR READER: this treatise is in its [Hadean stage](https://en.wikipedia.org/wiki/Hadean); everything below this message has to undergo intense transformations to achieve a more stable shape. Below are very roughly sketched areas. They are quite unreadable. If they don't make sense to you, it's likely because they don't make sense at all, yet.**

Returns are necessary only with conditionals! With sequences without conditionals, all the steps are necessary and already in the right order, so all needs to be expanded.

#### Loop

- Calls can be self-referential: recursion. Avoid Whitehead and Russell's mistake.

#### Error

on errors: hickey on systems. error values.

- Dataspace: access vs control. Open access, use control to determine when to block.

#### Putting the five elements together

A wise man once joked that his troubles playing football amounted to two things. The first was his left leg. The second one, his right leg. In the same way, the problems with programming languages could be reduced to two:
- The problem with [expressions](https://en.wikipedia.org/wiki/Expression_(computer_science)): they are not automatically referenceable from outside of their immediate context. Pillar 3 solves this by embedding computation in the dataspace, making every call and response explicit and accessible.
- The problem with [statements](https://en.wikipedia.org/wiki/Statement_(computer_science)): they are not data. Pillar 4 addresses this by turning statements into first-class entities within the dataspace, unifying code and data.

The approach we present here also eliminates any distinction between expressions and statements. Both are considered calls, and therefore both have responses.

not separateness, you choose where to draw the boundaries. example: call to another service with a db, see the three calls. show replacement.
Height of level is determined by looking who calls who. Low level is usually called, high level is usually the caller.

Read is write. get is a call. consider the data at rest as a queryable surface. there's no data in itself, only data that you can query. a read is a write on the readers end. a transformation that is symmetric in the read and write perhaps.
side effect as a call that changes what you consider durable data that is somewhere else in the space where the response is written on the caller.

instead of imperative vs procedural: causal. with declarative: you're just making a call that specifies more calls, more high level. But even microcode ,the lowest conceivable level of programming, is also declarative, since it's not actually orchestrating the gates and clocks of the CPU to carry out the operations. Focus on at which level you're working, which is, what is the message that you send, and the response that you receive.

Let's look at a system that has three parts:

- A call to an HTTP endpoint, to get the book orientalism and store it at `books orientalism` in the dataspace.
- The definition of the HTTP endpoint, stored at `server`.
- A relational DB.

Let's start by adding the DB, containing just one book.

```
DB books 1 author "Edward Said"
           id 1234
           isbn 978-0-394-42814-7
           title Orientalism
```

Let's then add a server with an HTTP endpoint that will make a call to the DB.

```
DB books 1 author "Edward Said"
           id 1234
           isbn 978-0-394-42814-7
           title Orientalism
server @ listen host example.com
                method GET
                path /api/books/<id>
                call @ db 1 "SELECT * from books where id = "
                          2 @ id
                     = ""
       = ""
```

Somewhere in our system

```
books orientalism @ http headers Accept application/json
                                 User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
                        host example.com
                        method GET
                        path /api/books/1234
                        type HTTP/1.1
                 = PENDING...
```

- store the latest query, or not even. the innermost call doesn't have to be shown. the intermediate ones have to. that's where you have to see where the expansion is made. for http, do it in a list.

examples with machine code, assembler, c, hll and sql.

### Pillar 5: interface is code

interface is code, therefore data.
this is all great for backend, but what about interfaces?
An interface is a way for a human to interact with software - always through hardware.
interface mapped to state! see the data being displayed and the possible transformations.

reactivity comes here. @ is reactive, when the references change, things are re-run. internally this is implemented as a loop over subscribers.

reactivity is no mere gimmick, there's something deeper: autopoiesis. when our perception changes, everything that that perception is based upon also changes in ourselves.

no separateness between user and system. shell, unidirectional data flow. there are sources of change, we distinguish them only in the data they bring. and then we express those changes with the constraints we already set up. and those changes can also change the constraints themselves.

Identity is tackled here, because this is where you can have an entrypoint for humans. Identity as data.

reactivity and the dataspace solve the cache problem. you know what things you want to keep around, and then you keep them updated using the minimum number of operations. problem solved. this is the only good solution to the general problem.

The way I prefer to picture computation is like a yin yang process, where there's a permanent energy flow that constantly produces change. The change is determined by the current situation of the whole. Given the current situation, a new change takes place. That change modifies the situtation into a new one, different but still very related to the previous one. Based on the new situation, a new change comes in. The process keeps on repeating endlessly.

```
reality -> change -> new reality -> new change...
```

This perspective also connects DIS to life forms through the concept of [dissipative structures](https://en.wikipedia.org/wiki/Dissipative_system), but I digress.

## How to test the (hypo)thesis of this treatise

- inverse relationship between data hiding and system quality and ROI

This is why REST is better than non-REST, why microservices are more tractable than monoliths.
- Microservices give you more rest. Corba also. Vs rpc; rpc can be represented as data, but less contractual.



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

from an organizational perspective

- stores: at rest
- internal calls (inside org): change according to rules
- external calls (connections): uses calls to change own store, and also uses calls on systems of external orgs
- interfaces to perform internal calls & external calls

### Running systems

Logs are data. Keep them. Query them with the same mechanisms.

### Security

It is about data, not about perimeter; it's zero trust but naturally. And kerchoffs principle: no unnecessary layers.
Control is still key.

auth as extra info. zero trust as checking the auth credentials with someone you trust. yet, how do you know that someone you trust is there? if https, it's not zero trust. it'd have to be through a key exchange, but what about getting the keys in the first place? you need to trust. if you're in the same place and then you separate, then you had a trust network that then got partitioned.

### On scaling, consistency and parallelism

if we use it at this level, then we need both wait and return value. control is the wait, the return value is the data. but it's not control, it's causality. this would also be the case if we had multiple computers.

- Distributed and parallel: consistency. Scalability with that assured is trivial (throw more nodes in), except for the "inside api" problem that Hickey points out.

understanding CAP: when distributed surface (distributed as amenable to experiencing partitioning) receives data, it either rejects (rejection as the lack of upating and also reading, indicating that that's not data) and presents/maintains consistency, vs remains available and has either temporary or permanent inconsistency. consistent system, in a partition does not present or update state, only stores it.

Consistency is not about enough resources or not, it is about locking a part of the dataspace until an operation is done.

Locks can be implemented as calls on sections of the dataspace.

### On forgetting

definition of noise: data that you're better off ignoring.

### Tradeoffs

wait, you have the blockchain trilemma (security, scalability, distribution). That to me maps completely to CAP's consistency, availability (especially with the modified CAP theorem about latency). Perhaps the general pattern is perfection, cost (in time, space and energy) and distribution/resilience. PCR. It is interesting, because it breaks the typical dilemma between quality and cost. It's really about three things, not two.

### Quality

Implementing the Toyota Production System
- autoactivation
- flow backwards, with reactive

muri & mura as redraws that only hurt performance or also as inconsistencies (defects), respectively. muri is performance waste, mura is inconsistency.

testing
- convergence to mathematical proof
- to generate, you must understand the order of validations.
- see errors as valid outputs, validate all the way.

Simple systems are amenable to proof.

## License

TODIS is written by [Federico Pereiro](mailto:fpereiro@gmail.com) and released into the public domain.
