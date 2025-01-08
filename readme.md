# The Organization of Digital Information Systems

## [Click here for a Visual Summary](http://altocode.nl/todis/visual)

> "The fundamental problem of communication is that of reproducing at one point either exactly or approximately a message selected at another point." -- [Claude Shannon](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf)

> "To a great extent the act of coding is one of organization." -- [James Hague](https://prog21.dadgum.com/177.html)

## Purpose

We currently live in the [Information Age](https://en.wikipedia.org/wiki/Information_Age). The revolution of digital technology has made information pervasive and central to human economy, politics, society and culture.

Our digital world is run by **digital information systems**. Digital information systems (DIS) are what we use when we interact with a digital device connected to the internet, such as as a smartphone or computer.

The purpose of this treatise is to provide a novel and systematic way to understand DIS. Through this novel perspective, it should be much easier to understand existing DIS, as well as designing, implementing and operating new ones.

We call DIS by many names: apps, (web)pages, services, websites, programs, even servers. Unless you are an expert, they can blend into each other. What is clear about them is that these systems are:

- **digital**: you need a phone or computer to interact with them.
- **interconnected**: you need an internet connection to access them.
- **concerned with information**: all that these systems do is to store, transform and communicate information.

A fast-growing minority is tasked with designing, implementing and operating DIS. This is challenging work. For makers of information systems, the main challenge is also to make sense of the systems they interact with, and also of the systems that they create themselves.

My hypothesis, which I'm actively testing as of the time of writing, is that the approach presented here can increase the speed of development of a DIS by an order of magnitude (~10x), while having very significant improvements (50-200%) in quality and the value of its features. The success or failure of these tools should be measured by whether they bring *at least* a 10x improvement to the speed, quality and value delivered by a team producing a DIS.

The main challenge posed by an information society is to make sense of it. The information that makes up our digital world is vast and grows and changes at a vertiginous rate.

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

The dual revolution of the [transistor](https://en.wikipedia.org/wiki/Transistor) and [information theory](https://en.wikipedia.org/wiki/Information_theory) allow humans to store, transmit and transform information with incredible speed, precision, and at a very small cost.

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

Designing DIS is already a complex task. However, it becomes exponentially harder when those responsible for building or understanding a system are focused on everything *except* the data it handles.

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

This entire treatise topples these two myths with the following (hypo)theses:

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
5. **Interface is call and response** (overcomes separateness between system and user and between data and time).

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

In some cases, it is convenient to put dots instead of numbers for each of the keys of a list. For example, the data above could be represented as:

```
musicians . born 1959
            firstName Gustavo
            lastName Cerati
          . born 1962
            firstName John
            lastName Squire
```

In this case, dots are understood to be placeholders for the actual numbers that mark the position of each item in the list of `musicians`.

Simple as it is, this data representation can be used to represent any data relevant to an information system. Here are a few examples:

**An [HTTP](https://en.wikipedia.org/wiki/HTTP) request and response pair**

```
request headers Accept application/json
                User-Agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
        host example.com
        method GET
        path /api/books/1234
        type HTTP/1.1
response body author "Edward Said"
              id 1234
              isbn 978-0-394-42814-7
              title Orientalism
         code "200 OK"
         headers Content-Length 83
                 Content-Type application/json
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
ProgramCounter 1100001010101011
StackPointer 11110111
StatusRegister 00100101
X 01100001
Y 11001010
```

**The [HTML](https://en.wikipedia.org/wiki/HTML) of a small page**

```
head title "Welcome to my site"
body . h1 "Hello World!"
     . p . class text
         . "This is my site"
```

Fourdata then is a way to look and describe data in unambiguous terms. With text and a few rules, we are able to describe a very broad range of data. With it, we can directly and unambigously look at a piece of data.

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
                             = body author "Edward Said"
                                    id 1234
                                    isbn 978-0-394-42814-7
                                    title Orientalism
                               code "200 OK"
                               headers Content-Length 83
                                       Content-Type application/json
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

In this framework, actors or process can be described in terms of calls. This allows us to have a view of them that is both more flexible and more precise. More flexible because we can choose to draw the boundaries around different calls to define what an actor or process is; and more precise because the actual functioning of actors and processes relies on calls.

This framework also allows us to go beyond the concept of state as a special type of data. If the "system" is a part of the dataspace, the state of the system (or of a subsystem) is also a part of the dataspace. Everything exists within the same dataspace, so the data in the system is indistinguishable (or rather, integrated) with the rest of the system. Put in another way, the state of our system is [first class](https://en.wikipedia.org/wiki/First-class_citizen) and can therefore be considered to have an identity of its own.

We have covered a lot of ground in this pillar. In a nutshell, we have found that the combination of a call and a response can express data change of any kind, just by using data itself.

In the next pillar, we will understand logic, which is what happens between a call and a response.

### Pillar 4: Logic is what happens between call and response

Armed with the pattern of call and response, we can now explore what happens between one and the other. Any call happening in a DIS will have a [deliberate](https://en.wikipedia.org/wiki/Teleology) response. The purpose of a call is to become a response. Logic is how this transformation happens. In other words, logic is intentional transformation of data.

The original definition of [logic](https://en.wikipedia.org/wiki/Logic) is concerned with correct reasoning. In the context of a DIS, logic is something rather more basic: given a purpose for a certain call, we want to be able to express it as a sequence of simpler calls. Eventually, those simpler calls become tiny operations at the [CPU level](https://en.wikipedia.org/wiki/Central_processing_unit). At that point, the software people (the author included) shrug, declare "[here be dragons](https://en.wikipedia.org/wiki/Here_be_dragons)", and leave those details to the hardware makers.

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
- Without *sequence*, without ["keeping on keeping on"](https://en.wikipedia.org/wiki/Keep_On_Keeping_On) and allowing a call to make multiple calls (calls which, themselves, will also make further calls) and collecting their responses, our DIS cannot produce responses to the calls it receives.
- Without being able to choose one path or the other based on a *conditional* (which is some data, a part of the dataspace), our DIS would always be doing the same calls, no matter what those calls responded. Without conditionals, our logic would always do the same thing, every time.

This can be readily seen in the [Turing Machine](https://en.wikipedia.org/wiki/Turing_machine), which is an universal model of computation.

The machine has an infinite tape divided in discrete pieces. If the tape is infinite in one way, we can represent it with a list, where each key is a position in the tape, and each value is the actual value written in the tape. For example:

```
tape 1 ə
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

There's always a current *state of mind*, called the *current configuration*. You could think of this as a *sequence*.

```
"current position" 1
"current state of mind" 𝖇
tape 1 ə
     2 ə
     3 0
     4 ""
     5 0
```

Any of these sequences will always do the following:

1. Write something to the tape (or write nothing).
2. Move the tape to the left or right (or keep it in place).
3. Change to another state of mind (or sequence).
4. Go back to step 1.

But what a sequence does depends on the symbol at the current position of the tape. That is, the writing, moving and calling behavior of the current configuration will be *conditional* to the symbol currently being scanned.

If we start with the Turing Machine just as it enters a new configuration, we'll start with a conditional: *what is the symbol on the current position of the tape?* Depending on that, the machine will execute one sequence or perhaps other. And when the sequence is complete, the machine will switch to *another configuration*: this can be seen as a call, where the new configuration is the destination. In a nutshell: conditional, sequence, reference.

The other two elements of computation, loops and errors, are niceties much in the same way as a roof and electricity are nice. Not absolutely essential for human life, but making it much easier and extending its capabilities. The essence of loops is conditional repetition of a sequence over a list or a hash; the essence of errors is conditional jumps through many levels, to avoid the burden of having to check each response to see if it is an error or not. Interestingly enough, errors are most useful as stoppers of sequences.

We'll now go element by element and explain each of them in detail.

#### Reference

A reference is the *destination* of a call. We could think of destinations as [links](https://en.wikipedia.org/wiki/Hyperlink).

The simplest type of reference is that which points to a value that contains no calls. For example:

```
"copy of widgets" @ widgets
                  = 20
widgets 20
```

`copy of widgets` makes a call to `widgets`. `widgets` itself is the value `20`. This has the effect of setting the value of `copy of widgets` also to 20.

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

This would also be the case if we wanted to reference a list or hash.

```
"copy of hash" @ hash
               = username deadmau5
hash username deadmau5
```

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
"make cake" 1 @ mix . @ chocolate 100
                    . @ flour 500
                    . @ butter 300
            2 @ bake degrees 200
                     ingredients @ 1
```

In the example above, you can notice that making a cake consists of two steps: mixing ingredients and baking them at 200 degrees (you can also notice that I've never baked a cake). There's two calls made here: `mix` and `bake`. Additionally, there are calls made to `chocolate`, `flour` and `butter` within the `mix` call, presumably to get the ingredients.

Note that we use the dot notation inside `mix`. This makes the sequence more readable. What's important is to remember that those dots are just placeholders for `1`, `2` and `3`.

We now have a problem, because we don't want those calls to happen when we are writing the sequence. Instead, we want them to happen when another parts of the space calls this sequence. So we need to create a new operator which will "freeze" these calls and only let them happen when the sequence is called. We will use `:`, since it is normally associated with defining something.

```
"make cake" @ : 1 @ mix . @ chocolate 100
                        . @ flour 500
                        . @ butter 300
                2 @ bake degrees 200
                         ingredients @ 1
```

So `make cake` is not a cake, not even a frozen cake. It is a part of the dataspace that, when called, will respond with a cake.

Now, how do we get a cake when we call `make cake`? We can understand that whatever is responded by `bake`, we will get!

```
"make cake" @ : 1 @ mix . @ chocolate 100
                        . @ flour 500
                        . @ butter 300
                2 @ bake degrees 200
                         ingredients @ 1
"today's cake" @ "make cake"
               = "delicious chocolate cake"
```

More generally: the response to the last call of a sequence will be used as the response of the *entire* sequence.

A subtle detail: the call to `bake` references `@ 1`. This references to the first element of whatever list can be found outside of the place where that call is. By going a couple of levels to the left, `@ 1` finds whatever is responded by the call to `mix`. So it is perfectly possible (and actually, generally essential) that a call within a sequence can reference responses from previous calls of the sequence.

Another detail: `make cake` doesn't receive a message! It will always return the same cake. What if we wanted to send a message to it, perhaps specifying the amount of people that will eat it?

```
"make cake" @ : people 1 @ mix . @ chocolate @ * . @ people
                                                 . 25
                               . @ flour @ * . @ people
                                             . 125
                               . @ butter @ * . @ people
                                              . 75
                       2 @ bake degrees 200
                                ingredients @ 1
"today's cake for 8" @ "make cake" 8
                     = "delicious chocolate cake for eight!"
```

We just snuck in the name of the message in between `:` and the list. It's a bit terse, but feels better than creating something more longwinded. Having a name allows us to refer to the message received by the outer call from within the sequence.

By the way, the *outer call* is the call that defines the sequence; the *inner call(s)* are those that happen when the sequence is taking place.

We're now ready to see the expansion of the sequence, which is what happens between the call and the response. We'll omit the definition of `make cake` (since we've just provided it) and focus on how `today's cake for 8` comes into existence.

```
"make cake" @ : people 1 @ mix . @ chocolate @ * . @ people
                                                 . 25
                               . @ flour @ * . @ people
                                             . 125
                               . @ butter @ * . @ people
                                              . 75
                       2 @ bake degrees 200
                                ingredients @ 1
"today's cake for 8" @ "make cake" 8
                     : 1 @ mix . @ chocolate @ * . @ people
                                                   = 8
                                                 . 25
                                             = 200
                                 = "200 grams of chocolate!"
                               . @ flour @ * . @ people
                                               = 8
                                             . 125
                                         = 1000
                                 = "A kilo of flour!"
                               . @ butter @ * . @ people
                                                = 8
                                              . 75
                                          = 600
                                 = "600 grams of butter!"
                         = "A mix of 200g of chocolate, a kilo of flour and 600g of butter!"
                       2 @ bake degrees 200
                                ingredients @ 1
                         = "delicious chocolate cake for eight!"
                     = "delicious chocolate cake for eight!"
```

In the example above, the expansion is the value of `"today's cake for 8" :` (notice the colon at the end). We use the colon for two things: for specifying what a sequence is; and also for showing the expansion of a sequence when it gets called. We use the same symbol because definition and expansion are both sides of the same coin. Definition makes expansion possible, and expansion is what makes definition useful.

No doubt the above is not immediately readable, but consider what it shows:
- The entire sequence of `make cake` when making the cake for 8 people.
- The intermediate responses obtained from each of the internal calls.

Note also what it doesn't show: the expansion of the calls to, say, `chocolate`, `mix` or `bake` (or even `+`). These could be shown if they were deemed relevant to what the user is looking at. There are two things that prevent us from showing the expansion to every single call:

- Some calls happen on a different system that doesn't share an expansion, but just return a response. This can happen for either performance reasons or security reasons.
- The user doesn't care about expanding every call, but rather only those that they want to inspect.

A small trick that can help make expansions more readable is to interpret `@ foo` as if `foo` was a link: blue and underlined. A programming environment can provide this facility; when working in a blackboard, the references of calls can be underlined, to avoid writing so many `@`s.

Before we move to conditional, it is a good idea to realize that *the expansion of a sequence is equivalent to computation*. The nature of computation is sequential: making one call, waiting for a response, then making another call.

We now turn to the third and last essential element of logic, conditional.

#### Conditional

A conditional is just a call. However, it is a special call because, depending on a condition, it will *choose* to expand a sequence depending on a condition.

A condition is something essentially binary: it is either yes or no. In traditional programming environments, these values are called `true` and `false`; but we have no room (nor need) for them. We can simply use `1` for `true` and `0` for `false`.

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

Now, the conditional above is a bit silly, because its condition is always set to `1`. The following is a bit less silly, particularly if you realize that `party` could change:

```
greeting @ if cond @ party
                   = 1
              do @ "make cake" 8
                 = "delicious chocolate cake for eight!"
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

In the example above, `make cake` was not called! This is precisely why conditionals are essential: they allow us to *not* call a certain sequence.

A second sequence can be passed to `if` within the `else` key, to be called if the condition is *not* met.

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
              do @ if @ > . @ people
                            = 8
                          . 4
                      = 1
                   do @ "make cake" @ people
                                    = 8
                      = "delicious chocolate cake for eight!"
                   else @ "get more people"
                 = "delicious chocolate cake for eight!"
              else @ "make random healthy dish" 2
         = "delicious chocolate cake for eight!"
party 0
people 8
```

Notice that we introduced another call, `>`, which compares two values, and responds with either `0` or `1` depending on whether the comparison was successful or not. In the case above, since we have more than four people, we can go ahead and make cake, instead of getting more people to join the party.

A significant problem with the sequence above is that nested conditionals can be hard to read, even by experienced programmers. A way to mitigate this problem is to use the `res` call (short for *respond*), so that we can break out from a sequence without having to wait until the end.

```
greeting @ "greeting sequence"
         : 1 @ if cond @ "there is cake already"
                       = 1
                  do @ res ""
                     = ""
             = ""
         = ""
"greeting sequence" @ : 1 @ if cond @ "there is cake already"
                               do @ res ""
                        2 @ "make cake" 8
"there is cake already" 1
```

Note what happened above: if the condition is fulfilled (which in this case, it is), we will make the call `res ""`. This makes the entire `greeting` get a response of `""`. The critical bit to note is that the second step of the sequence, `make cake` is not at all expanded! This is what `res` does: it breaks out of the current sequence by responding with a given value.

This pattern is most useful to do away with branches that are either shorter or less likely (usually both). In traditional programming, the `res` call is described as a [*return*](https://en.wikipedia.org/wiki/Return_statement), because both data (in this case, empty text) and control (that is, the availability of the system to proceed with the expansion of the next call) are returned to whoever called the sequence. In this treatise, however, we will call this a *response*, because that's simply what it is: we explicitly respond with a value without having to expand the rest of the current sequence.

For those versed in programming, it is interesting to realize that returns are only necessary with conditionals! Neither reference nor sequence require them. Returns make sense only to conditionally break out of a sequence. If a sequence had no conditionals, why would we want to break out early? We could simply delete the calls that we don't need and always have the same definition.

Note that, in our last example, we had to specify the sequence to greeting in another place, "greeting sequence". The reason for this is that we want "greting" to get the response of the *last* call of the sequence; if we had merely put the sequence inside of it, it would have ended up with a list of two empty texts.

Now that we have set the third and last essential logic element, we can go to our first non-essential (yet incredibly useful) element: loops.

#### Loop

A loop is a way to conditionally repeat sequences. Loops put together everything we've seen so far: they reference data; they repeat a sequence; and they choose to stop or continue based on a conditional.

The most common kind of loop goes through the elements of a list, performs an operation to each of them, and returns a new list with the responses of each of the calls it did to each of the elements of the list.

```
@ loop data . 1
            . 2
            . 4
       do @ "plus ten"
= 1 11
  2 12
  3 14
```

This type of loop is usually called a [*for loop*](https://en.wikipedia.org/wiki/For_loop), but we'll just call it `loop` since they are the most prevalent type of loop. The meaning of *for* is: *for each* of these elements, do something (that's why others call these *do* loops ).

Now, let's fathom the work that this "non-essential" construct (`loop`) is doing for us:
- Set a part of the dataspace to keep the count of how many elements of the list we have processed.
- Set a part of the dataspace to become the list where we accumulate the results of each call to `plus ten`.
- Start calling `plus ten` for each of the elements in the list.
- Respond with the result list when the length of the received list equals the length of the list with results.

This simple type of loop will very likely be more than half of the loops you write in your logic. That is worth pondering.

If we add a conditional to the loop, we can make the loop stop before it runs out of data.

```
count 12
@ loop cond @ < . 10
                . @ count
       data . 9
            . 3
            . 6
       do @ : value @ set dest count
                          value @ + . @ count
                                    . @ value
= 1 9
  2 3
```

In the example above, we take a list with three numbers (`9`, `3` and `6`) and start adding them one by one to `count` (which, you must believe me, is `0` when we started):
- We first check whether count is less than 10; it is, therefore the loop adds first 9 to `count`, making it `9`.
- We check again that count is less than 10, which it still is. Then the loop adds `3`, making it `12`.
- At this point, we check again that count is less than 10; but since it is `12`, we're done!

Now, what does the *expansion* of a loop looks like? Let's find out.

```
count 12
@ loop cond @ < 1 10
                2 @ count
       data . 9
            . 3
            . 6
       do @ : value @ set dest count
                          value @ + . @ count
                                    . @ value
: 1 cond @ < . 10
             . @ count
               = 0
    do @ set dest count
             value @ + . @ count
                         = 0
                       . @ value
                         = 9
                   = 9
       = 9
    value 9
  2 cond @ < . 10
             . @ count
               = 9
    do @ set dest count
             value @ + . @ count
                         = 9
                       . @ value
                         = 3
                   = 12
       = 12
    value 3
3 cond @ < . 10
           . @ count
             = 12
       = 0
= . 9
  . 3
```

That's a non-trivial expansion and it is quite long. Note however that it captures all of what happens during the execution of the loop: the first two checks with their corresponding calls to `set`, and the third check which stops the loop.

The second type of loop is usually called a *while loop*. It is less common than the *for* variant, but still pervasive. In essence, what distinguishes the first type of loop from the second is that when we are going through an entire list, we know upfront how many times we will call what's inside `do`, whereas in the second type, we don't and don't particularly care: we'll keep on going until a condition is met.

Other mechanisms can be introduced into `loop`:

1. Filter: returning a list only with values that match a certain condition.

```
"only evens" @ loop data . 1
                         . 2
                         . 3
                         . 4
                    filter @ : value "is even" @ value
             = . 2
               . 4
```

2. Times: repeat a call a specified amount of times, without even passing in a list.

```
count 10
"make it ten" @ loop do @ set dest count
                              value @ + . @ count
                                        . 1
                times 10
```

3. Accumulator: a type of loop that processes a list and combines its elements into a single result by repeatedly applying a call. This call operates on the current accumulated value and the next element in the list.

```
"gimme ten" @ loop acc @ +
                   data . 1
                        . 2
                        . 3
                        . 4
             = 10
```

The power of loops, it is worth remembering, stems only from the use of references, sequences and conditionals.

Before we leave loops, it is good to explain *recursive calls*. A [recursive call](https://en.wikipedia.org/wiki/Recursion_(computer_science)) is a call that calls itself. While that sounds paradoxical (and can even be so), most of the time it is a practical and elegant solution.

Take the following humble problem: we have a list with lists inside (some very nested); eventually, the internal values of each list are all numbers; we want to get all of these numbers into a flat list. This can be elegantly accomplished through recursion.

```
"flat list"
flatten : value @ if cond @ type type list
                                 value @ value
                     do loop data @ value
                             do @ flatten
                     else @ add to "flat list"
                                value @ value
```

The recursive bit is `do @ flatten`: when `value` is a list, we will loop over its contents, calling `flatten` for each of them. If one of them happens to not be a list, we will add it to "flat list". Otherwise, the recursive (nested) call will deal with the nested list.

This is not an easy concept to master, but once you do, it will repay your efforts in spades. I recommend you work out the logic for yourself.

Recursive calls are like loops in that they combine the repetition of a sequence based on the result of a conditional. However, what recursive calls give us is the ability to express *loops with depth*. The loops we saw before recursion are quite *flat*: they go over a list, or repeat things a number of times, but have no depth. When there are loops within loops, and the level of nestedness is not known beforehand, it is usually best to tackle the problem with recursive calls.

How do recursive calls avoid going on forever? Quite simply, they have to be written in a way that will make them recurse conditionally; and that condition cannot always be true - if it is always true, then we will have an infinite loop. Although two great mathematicians were so concerned with recursion (self-reference) that they forbid it from [their logical system](https://en.wikipedia.org/wiki/Principia_Mathematica), over a century of experience with computing has taught us that recursion is not only possible, but essential.

We'll now tackle the fifth and last logical element: error.

#### Error

Errors are data that signal that something has gone wrong. They merit their own (non-essential) logic element because, almost always, when an error occurs we want to stop the sequence that produced it and deal with the error.

If we go back to the previous example about the cake, what would happen if you couldn't get the butter? If the butter was missing then it doesn't make sense to keep on baking the cake. Possible corrective actions are:

- Replace butter with another ingredient.
- Stop all cake making until you figure out why no butter is available.
- Replace the cake with something else entirely.

Now, all of these can be expressed with conditionals. But let's just try to do it and see what happens:

```
"today's cake for 8" @ "make cake" 8
                     : 1 @ mix . @ chocolate @ * . @ people
                                                   = 8
                                                 . 25
                                             = 200
                                 = "200 grams of chocolate!"
                               . @ flour @ * . @ people
                                               = 8
                                             . 125
                                         = 1000
                                 = "A kilo of flour!"
                               . @ butter @ * . @ people
                                                = 8
                                              . 75
                                          = 600
                                 = error "No butter available!
                         = error "An ingredient is missing!"
                       2 @ bake degrees 200
                                ingredients @ 1
                         = error "No ingredients found"
                     = error "No ingredients found"
```

Looking at the expansion above, we see that we couldn't get any butter. The shape of the error is a hash with key `error` and value `No butter available!`. This made `mix` fail, which in turn made `bake` fail.

Because we have the expansion available, we can trace back the error back to a lack of butter (if we didn't have the expansion, we'd have to put some logs and try to get cake once again). Still, not only we have to trace the error back, but we also have to write `mix` and `bake` in a way that perform error checking on their inputs. Imagine if `mix` and `bake` didn't do this:

```
"today's cake for 8" @ "make cake" 8
                     : 1 @ mix . @ chocolate @ * . @ people
                                                   = 8
                                                 . 25
                                             = 200
                                 = "200 grams of chocolate!"
                               . @ flour @ * . @ people
                                               = 8
                                             . 125
                                         = 1000
                                 = "A kilo of flour!"
                               . @ butter @ * . @ people
                                                = 8
                                              . 75
                                          = 600
                                 = error "No butter available!
                         = error "The spoon got stuck in the mix!"
                       2 @ bake degrees 200
                                ingredients @ 1
                         = error "The oven caught fire!"
                     = error "The oven caught fire!"
```

Not very safe! Now we have an oven on fire, which is a remarkably distinct outcome from the expected one (chocolate cake for eight people).

All of this highlights **the importance of catching errors as soon as possible**.

What if, instead, we did something like this?

```
"today's cake for 8" stop do @ "make cake" 8
                             : 1 @ mix . @ chocolate @ * . @ people
                                                           = 8
                                                         . 25
                                                     = 200
                                         = "200 grams of chocolate!"
                                       . @ flour @ * . @ people
                                                       = 8
                                                     . 125
                                                 = 1000
                                         = "A kilo of flour!"
                                       . @ butter @ * . @ people
                                                        = 8
                                                      . 75
                                                  = 600
                                         = error "No butter available!
                                 = error "No butter available!
                             = error "No butter available!"
```

What `stop` does is make the sequence inside `do` stop at the first error. Note that this call affects what happens inside `mix`, which is nested inside `make cake`. When `butter` responds with an error, `mix` stops and responds with that error, and `make cake` does the same thing. This yields the following benefits:

- We get the actual error that generated the problem.
- No spoons stuck on the mix or ovens on fire.

`stop` is analogous to a supervisor: when things go wrong, they're ready to step up, take responsibility and deal with the problem. Most of the time, however, there's no need for the supervisor to intervene.

We can also pass a `then` sequence to do something with the error.

```
"today's cake for 8" stop do @ "make cake" 8
                             : 1 @ mix . @ chocolate @ * . @ people
                                                           = 8
                                                         . 25
                                                     = 200
                                         = "200 grams of chocolate!"
                                       . @ flour @ * . @ people
                                                       = 8
                                                     . 125
                                                 = 1000
                                         = "A kilo of flour!"
                                       . @ butter @ * . @ people
                                                        = 8
                                                      . 75
                                                  = 600
                                         = error "No butter available!
                                 = error "No butter available!
                             = error "No butter available!"
                           then @ : error @ report @ error
```

We can then call `report` with the actual error received. If for some reason the supervisor interprets that it cannot deal with the error properly and must invoke any supervisor up the chain (to the left of the dataspace) it can do so by simply responding with an error, perhaps the same error it itself received.

The error element saves us a **lot** of conditional logic. In the example above, it saves us from writing every call to check every value to see if it is an error or not, and if it is, to call `report`. If we wanted to make that dynamic, we would have to pass a call to handle the error (`report`) into each of the calls, starting with `make cake`, then `mix` and `bake`, even `chocolate`, `flour` and `butter`! That will quickly turn a beautiful sequence into a brittle eyesore.

You might be thinking: if computesr are so fast and so precise, why do they have errors at all? That's a great question. I believe that we should have an asymptotic attitude towards error (which means that we're working to make them exponentially less likely as time goes by -- more on this in the Quality section below). However, errors are still a reality of DIS, particularly when you interact with less reliable DIS (which will happen a lot of the time).

Rich Hickey [takes it further](https://www.youtube.com/watch?v=ROor6_NGIWU&ab_channel=ClojureTV) and argues that what distinguishes a language from a system is that, in systems, errors are an unavoidable part of the landscape. Probably anyone with any practical experience writing systems will agree with that statement.

And we're done with logic! We have seen the five elements of logic that are present in DIS. These five elements will cover an overwhelming amount of the logic of any DIS you may encounter or write yourself.

#### Putting the five elements together

A wise man once joked that his troubles playing football amounted to two things. The first was his left leg. The second one, his right leg. In the same way, the problems with programming languages could be reduced to two:

1. The problem with [expressions](https://en.wikipedia.org/wiki/Expression_(computer_science)): they are not automatically referenceable from outside of their immediate context. Pillar 3 solves this by embedding computation in the dataspace, making every call and response explicit and accessible. We've seen an example of this with `bake` referring to `1`, which was the response to the previous call to `mix`.
2. The problem with [statements](https://en.wikipedia.org/wiki/Statement_(computer_science)): they are not data. Pillar 4 addresses this by turning statements into first-class entities within the dataspace, unifying code and data.

The approach we present here also eliminates any distinction between expressions and statements. Both are considered calls, and therefore both have responses.

Let's see how all the elements fit together in the following design:

- We will make a call to an HTTP endpoint, to get the book orientalism and store it at `books orientalism` in the dataspace.
- We will define an HTTP endpoint to serve this request by calling a database server.
- We will also have a database server that can allow us to get data.

```
"copy of orientalism" @ http call method get
                             path /api/books/1234
                      = body author "Edward Said"
                             id 1234
                             isbn 978-0-394-42814-7
                             title Orientalism
                        code 200
database books 1 author "Edward Said"
                 id 1234
                 isbn 978-0-394-42814-7
                 title Orientalism
         "get book" @ : id @ loop data @ books
                                  filter @ : value @ = . @ value id
                                                       . id
server @ http listen do @ : request 1 @ database "get book" @ request path 3
                                    2 @ if cond @ = . @ 1
                                                    . ""
                                           do 404 "Book not found"
                                           else 200 @ 1
                     method get
                     path /api/books/*
```

In the example above, we have:

- `database`, which has both the data and a call to get it.
- `server`, which defines an HTTP server with one endpoint, `get /api/books/*`. The `*` is a wildcard, which means that anything except a slash (`/`) will be matched.
- `copy of orientalism` makes an HTTP call to `server` and gets the book. Because it used the right id (`1234`), it will succeed in getting the book. Note it also gets a `200` status code, to indicate that the request was successful (this is a standard part of the HTTP protocol).

An interesting point happens with the expansion. Technically, we could see the expansion to the call to the HTTP server:

```
"copy of orientalism" @ http call method get
                             path /api/books/1234
                      : 1 @ database "get book" @ request path 3
                                                1234
                          = author "Edward Said"
                            id 1234
                            isbn 978-0-394-42814-7
                            title Orientalism
                        2 @ if cond @ = . @ 1
                                          = author "Edward Said"
                                            id 1234
                                            isbn 978-0-394-42814-7
                                            title Orientalism
                                        . ""
                                    = 0
                               else 200 @ 1
                                        = author "Edward Said"
                                          id 1234
                                          isbn 978-0-394-42814-7
                                          title Orientalism
                      = body author "Edward Said"
                             id 1234
                             isbn 978-0-394-42814-7
                             title Orientalism
                        code 200
```

But that might be too revealing. From a security standpoint, servers shouldn't expose too much of their internals, particularly if those internals carry secrets. For example, if the call from `server` to `database` contained a secret to prove to `database` that `server` is calling, that secret would be revealed in the expansion of the call to `server` to anyone that made a call to it. That would open up the database to anyone!

For that reason, it is best for servers (and databases) to not disclose their expansions, but instead put them in a part of their own dataspace where they store incoming requests and their expansions.

```
database expansions 2024-12-24T14:15:34.889Z @ "get book" @ loop data @ books
                                                                 filter @ : value @ = . @ value id
                                                                                        = 1234
                                                          = author "Edward Said"
                                                            id 1234
                                                            isbn 978-0-394-42814-7
                                                            title Orientalism
server expansions 2024-12-24T14:15:34.887Z 1 @ database "get book" @ request path 3
                                                                   1234
                                             = author "Edward Said"
                                               id 1234
                                               isbn 978-0-394-42814-7
                                               title Orientalism
                                           2 @ if cond @ = . @ 1
                                                             = author "Edward Said"
                                                               id 1234
                                                               isbn 978-0-394-42814-7
                                                               title Orientalism
                                                           . ""
                                                       = 0
                                                  else 200 @ 1
                                                           = author "Edward Said"
                                                             id 1234
                                                             isbn 978-0-394-42814-7
                                                             title Orientalism
```

Note that each expansion is a hash where each key is a timestamp. This can be invaluable for tracking issues by the maintainers of the database and the server.

If we consider what happened above, the call produces a response in each of the caller (`copy of orientalism` and `server`). It also produces data inside of `server` and `database` (the expansions, that we choose to record).

These expansions are sometimes called [side effects](https://en.wikipedia.org/wiki/Side_effect_(computer_science)), because they are considered to be not part of the "main" part of the information flow (which is the book in question, flowing from `database` back to `copy orientalism`). However, I propose that we let go of this distinction: expansions are also data and also happen through calls. What's the "main flow" vs a "side effect" really is in the eye of the beholder. Better to consider it all as calls and responses.

We can consider these expansions as the [negative](https://en.wikipedia.org/wiki/Negative_(photography)) of the calls through which data flows. They are every bit as important as the final results.

One more heresy before we move to our fifth and final pillar: there is an established practice of distinguishing between [imperative/procedural logic](https://en.wikipedia.org/wiki/Imperative_programming) (which "tells the computer what to do") and [declarative programming](https://en.wikipedia.org/wiki/Declarative_programming) (which "tells the computer what you want, leaving the details to the computer"). But where do we draw the distinction between micromanaging the computer and managing the computer? To me, this distinction is squarely in the eye of the beholder. Microcode could be seen as a declarative interface to a CPU ("I tell the CPU what operation I want and let the CPU actually manage its own logic gates"). Similarly, a line of a very high level program might be seen as imperative ("give me all the rows from this database where the creation time is less than three seconds ago"). I propose that we eliminate this distinction and instead focus on tools to create good abstractions: whether they specify the "what" or the "how" is a matter of how you see it. There will always be a "how" always underpining any "what". In other words, the "what" is the interface, the "how" is its implementation. And because they are layered, it makes no sense to call some of them "whats" and some of them "hows".

We're ready to move to our fifth and final pillar: interface as a response that makes calls.

### Pillar 5: interface is call and response

What is an interface? When most people (including DIS experts) talk about an interface, what they really mean is a *graphical user interface*. This is a good starting point to understand interfaces in general. Colloquially, then, an interface then has two distinguishing features:

1. It is meant for human users, not computers.
2. It displays something *graphical*, which means *not just plain text*: in a graphical interface there are boxes, tables, images, colors, buttons and menus.

By being graphical in nature, interfaces do two things:
- Reduce the mental overwhelm induced by glancing at a wall of text.
- Complement the power of text with the power of other graphical means.

The last point is best summarized by [Jack Rusher](https://jackrusher.com/strange-loop-2022/), when he reminds us that *the visual cortex exists*. This point is worth remembering! Just using text to represent data is not always the best way to represent it. Other graphical elements are **not** just handholding (and even some proper handholding can make a great difference!).

Despite interfaces being made of graphical elements besides text, they can still be represented with text or with zeroes and ones. For example, in modern web applications, all of the interface (with the exception of images) is created with text that represents graphical elements. Even icons are usually written using [SVG](https://en.wikipedia.org/wiki/SVG), which is a textual format.

Now, what can users do with interfaces? If we go back to our original definition of a DIS, we remember it is a system that can do three things: communicate, store and transform data. Interfaces are not suitable for storing data, but indeed they are how users can both **see** data and **send** data back to the system.

Understanding it in terms of call and response, we can see the interface itself as a response. This response allows a user to *see* part of the data of the system. For non-interactive interfaces, that's all there is. However, most interfaces also allow users to interact (that is, send data back) to the rest of the system. Therefore, these interfaces provide a way for users to *make calls* to the system.

```
@ "draw interface"
= "the interface goes here!"
```

A very concrete example is an interface that displays a table and has a couple of buttons. The entire interface can be considered as a response to a call, just data that allows the user to see a part of the dataspace. When the user clicks on one of the buttons, they are making further calls to the system.

```
@ click "left button" : @ show "next page"
```

In more abstract terms, an [interface](https://en.wikipedia.org/wiki/Interface_(computing)) is generally considered *a boundary between a DIS and a human*, over which they exchange information. In our framework, every call is a boundary between two parts of the system. If we consider a user to be part of the system it interacts with, we can then say that every interaction between the user and the rest of the system is a call.

What is then an interface? We could say that the interface is the combination of a call and its response; whereas the sequence of calls that make the call possible are considered the *implementation*.

```
implementation 1 "what transforms a call into a response"
interface 1 call
          2 response
```

In other words: an interface is the call and its message, plus what comes back. What is **not** the interface is the logic behind a call, which transforms the call itself into a response. Each call is an interface to its underlying implementation. And this is the entire point of building calls with calls: they allow us to organize ever larger and more meaningful units of communication and transformation of data.

What is an interface is in the eye of the beholder: a mere ordered list, retrieved from a specific location in the dataspace, can be considered an interface.

If you agree with the above, it's good to pause a minute to understand our departures from tradition:

1. We are doing away with any intrinsic boundary between user and system, considering them both as one. This means that calls vary in their behaviors and in what they respond with, but not in their intrinsic nature. There's no crucial difference between a call to increment a register in a CPU or a call to retrieve an HTML interface. **System calls and user calls are the same**.
2. There's no distinct general internal or external area. Every call exposes an interface and has its own internal implementation; but that internal representation is also made of calls. Rather than a few blockish components exchanging rays of data over the network, we have a [Koch Snowflake](https://en.wikipedia.org/wiki/Koch_snowflake) with calls expanding into further calls.

Considering any call and response to be an interface liberates us from the burden of having to sharply distinguish "internal" from "external" operations; instead, every call has an external surface (its interface) and its internal surface (its implementation). Through [self-similarity](https://en.wikipedia.org/wiki/Self-similarity), we overcome the separateness between user and system, and more generally between any two parts of our system.

This doesn't mean that users have to work with zeroes and ones, or that every call can be trusted without verification. A self-similar system can still show graphical data and enforce security policies. But that's a matter of the content of those calls, rather than enforced by separateness between user and system, between trusted and untrusted components.

Self-similarity is not a new idea, but it is often forgotten in most design efforts. It is worth remembering some very useful patterns that have come from this idea:
- Unix treating everything as a file: User and system interactions follow the same read/write interface, maintaining a consistent pattern.
- Shells as userland programs: A shell operates like any other program, using the same system interfaces it exposes to users.
- Unidirectional data flow in UIs: The same principles of state updates and data propagation apply at all levels, from individual components to the entire app.

Most of the time, users are the originators of many calls in a system. From the perspective of the computer, when a user initiates an action (like loading up an interface), the initiative (call) belongs to the user. However, this is usually reversed: imagine that the app delivered a notification to the user, which prompted them to then open the app: in that case, the initiative belongs to the computer, and the user's call is just a consequence (do we dare say *implementation*?) of the notification sent by the app.

Having broken the separation between user and system, we will now attempt to break the separation between time and dataspace.

The roots of DIS, and still its dominant paradigm, is [batch processing](https://en.wikipedia.org/wiki/Batch_processing). Systems are conceived to receive a call, process it and then provide a response. In this paradigm, once a call is made and its response is obtained, no further updates are necessary.

```
"copy of orientalism" @ http call method get
                             path /api/books/1234
                      = body author "Edward Said"
                             id 1234
                             isbn 978-0-394-42814-7
                             title Orientalism
                        code 200
```

In the batch paradigm, once we get the book, the response will not change. If, for example, the entry for the book is changed in the database after the copy is made, the copy will not be updated.

The contrasting paradigm to batching, and the one that we embrace here, is the [reactive paradigm](https://en.wikipedia.org/wiki/Reactive_programming). They were introduced by spreadsheets. Consider the following example:

```
    A      B
1|  5  |   5  |
2|     |=A1+B1|
```

Now, what would the value of B2 be? Since it references A1, which is `5`, and B1, which is also `5`, the result will be `10`. Now, if either A1 or B1 change, the value will be updated. This is reactivity! In a batch program, you would have to *re-run* the program to make use of the updated values of A1 and B1.

What a reactive system does is to update the dataspace when a change happens. For example, when A1 is updated, any cell dependent on it will be updated. And what *updated* means is that the call that sums A1 and B1 *will be made again*.

If a cell doesn't directly depend on A1, but on another cell that in turns depend on A1 (like, for example, A2), that cell will also make a call again to get its value when A1 is updated. A reactive system is a system that repeats a calls whenever the destination of the call, or its message, experiences a change.

```
@ destination message
= response
```

To say it one more time: whenever `destination` or `message` change, a call is made again and the response is updated. And if any other part of the dataspace depends on that response, either directly or indirectly, it will also make the call again.

Now, why does this overcome separateness between time and (data)space? Because, in a DIS, what marks the passage of time is changes to data. Systems that are not reactive are plagued with stale data; the dataspace is connected in space, but not time. A reactive system, by repeating calls when change happens, keeps the system connected in time as well as space.

If a given part of the dataspace is a call, then we can say that that part of the dataspace *depends* on both the destination of the call and its message.

```
location @ destination message
         = response
```

In the example above, `location` depends on both `destination` and `message`. If `message` had a reference to another part of the dataspace, `location` would also be dependent on that part of the dataspace too.

If instead of referencing a part of the dataspace, we copied its value, then the dependency would be broken. This is why reference is crucial: because not only it connects its current value with another part of the dataspace: it connects its value with another part of the dataspace for as long as the reference exists.

Some calls, however, have bounded reactivity:

```
"copy of orientalism" @ http call method get
                             path /api/books/1234
                      = body author "Edward Said"
                             id 1234
                             isbn 978-0-394-42814-7
                             title Orientalism
                        code 200
```

In the call above, `http` makes a HTTP call over the network. But that call has no way of "knowing" if the HTTP handler on the other end has experienced a change. Thus, it is still possible to have non-reactive calls, particularly when those calls go over certain system boundaries (like another computer). If, however, either the method or the path changed (or even the implementation of `http`), then the call would be repeated.

Reactivity is not just convenient: it allows the system to always stay in-sync with itself. This also happens in biological systems: when a living being perceives a change in their environment, everything that in the being's mind depends on the environment will also react to that change. And if a change takes place internally, that will trigger further changes in the organism. As I understand it, this is the basis of [autopoiesis](https://en.wikipedia.org/wiki/Autopoiesis): self-production.

In practice, reactivity gives us a system where the notion of "running a program" dissolves. A user can construct their system, and the system will respond (react) to changes brought by the user, as well as other parts of the system, as soon as the changes happen.

Reactive systems are much more *alive* than their batch counterparts. Every reference can be understood to be alive, in the sense that it is listening (and reacting) to changes in another part of the system. This means that every reference requires resources to keep it alive; but then again, that's a small price to pay in order to work with a system that shows life (as opposed to systems that are as dead as a [coffin nail](https://steve-yegge.blogspot.com/2007/01/pinocchio-problem.html)).

Reactive systems are always running: they are always ready to receive calls, and to generate further calls if a change happens in a part of the dataspace that is a dependency of another part of the dataspace.

Reactivity can be implemented by tracking what parts of the system depend on other parts of the system, and repeating calls for those parts that are affected by a change. The main concern of the implementation should be to avoid and report circular dependencies which might send the system into a crash.

We can already understand that a single change to the dataspace can trigger multiple calls in its dependencies. This 1:N relationship between a call and all possible calls that might be done in response to that original call, is a feature shared with [event systems](https://en.wikipedia.org/wiki/Event-driven_architecture). It may be even possible to replace event systems with reactive systems, since they share both the 1:n relationship described above, plus the fact that the dependency doesn't care which part of the system depends upon it (this is traditionally described as *loose coupling* but is best understood as an arrow that goes in one direction).

One last point concerning updates: when a new response replaces an old one, a system may still keep around the old value of the response. This is called [version control](https://en.wikipedia.org/wiki/Version_control) and allows users to be able to see a previous state of the system. In other words, version control is time travel in the context of the system. Version control is almost always a great idea; the most challenging part of it is to determine what should be forgotten (deleted), either because of lack of space or because of privacy concerns.

We've come a long way through the last five pillars. Hopefully we have, by now, established a systematic way to look at digital information systems. In the last part of the treatise we will discuss some applications of the theory to specific areas. The core of the treatise, however, is concluded here.

**DEAR READER: this treatise is in its [Hadean stage](https://en.wikipedia.org/wiki/Hadean); everything below this message has to undergo intense transformations to achieve a more stable shape. Below are very roughly sketched areas. They are quite unreadable. If they don't make sense to you, it's likely because they don't make sense at all, yet.**

## How to test the (hypo)thesis of this treatise

If you've made it this far into the treatise, the best thing you could do is to find out for yourself whether any of it stands the test of reality. If it does, and particularly if it doesn't, I would very much appreciate if you could let me know about your results, privately or publicly.

Some possible hypothesis and questions you may consider:
- When studying an existing sytem or designing a new one: is the design naturally expressible in terms of calls and responses? Does the model allow you to hide and show detail in a practical way?
- When stuyding design flaws: do these flaws stem from lack of understanding of data flows? Do they emerge as failures of self-similarity?
- When implementing a system: does the unified dataspace provide an adequate representation of the actual data flows?
- When running a system: is it practical to consider the logs of the system as an integral part of their data?

## Applications of the theory

### Team organization

For the creation of a general purpose DIS, any analytically capable person can read and write calls and their logic. The team can be staffed by analytically strong people with a good understand of the problem domain. They should focus on understanding the data flows and establishing [organizational principles](https://prog21.dadgum.com/177.html). Understanding the organization and flow of data defines 90-99% of the implementation and its tests.

Specialization works for certain areas: interface design, tool making, algorithm selection & implementation, data science, AI.

### Understanding existing systems

- Obtain a dump of all the databases. Convert it to fourdata and put it in a single dataspace.
- Write constraints, if any, that are present in the data (for example: types of different fields, relationships, possible values or valid ranges). In my experience, these checks cover 90-99% of the constraints: type, equality (or non-equality), range (for numbers), matching a pattern (for texts).
- Capture logs of the system and use it to see which logs are generated. Add more logging in critical calls to see what goes into them and what comes out of them. Put this data in the dataspace too.
- Use the system for real, eschew unit tests. Always go with the real thing.
- In sufficiently complicated systems, perform network analysis to see who's who, and add that information to the logs.
- Go 80/20 rather than all in: a few calls represent most of the value of the system, or perhaps most of the mystery. Understanding a few core calls well (or a few mysteries) will bring most of the payoff.
- Valuable code is only that that performs nontrivial operations, and can usually be isolated.
- Feed data to a LLM to find patterns. Having the data and the logs in an unified dataspace will make this easier.

### Designing and implementing new systems

- Design the data at rest in an unified dataspace.
- Design the interface of the main calls, using concrete examples of which response is generated by which call + message.
- Tackle the implementation of the most challenging calls to detect algorithmic issues early.
- Strictly define and validate the inputs to all of the calls to your system.

### Running systems

- Treat expansions as data. Keep them in a queryable dataspace.
- Obscure private data in the expansions by deleting it or replacing it with a placeholder.
- Have a clear policy for deletion of data when requested by users, or when enough time elapses. Enforce these policies as part of the logic of the system. Log the extent of deletions.

### Security

From the perspective of this treatise, a secure system shows three qualities:

1. [Identification & authentication](https://en.wikipedia.org/wiki/Authentication): is able to properly identify someone.
2. [Authorization](https://en.wikipedia.org/wiki/Authorization): is able to enforce access control so that only those that are allowed to make a call can in fact make it.
3. [Encryption](https://en.wikipedia.org/wiki/Encryption): sends data over the network in such a way that only the caller can read the response.

In other words, a secure system is one that properly perceives identity, makes sure that calls are done by those who are supposed to do them, and makes sure that eavesdropping is not possible.

At the time of writing, encryption is generally provided; all that system designers need to do is to make sure that encryption is being used.

Concerning the first two points, the crucial fact is to understand that data concerning users and permissions *can be part of the dataspace*. Generally, this is not the case, which is a source of great inefficiency and even outright security issues. Consider both users and permissions as data; the part of the dataspace on which they reside must, naturally, be very restricted.

In Pillar 5 we have attempted to break away from a model that separates the internal from the external and the user from the system. We can do the same with security, by abandoning security perimeters and moving to a [zero trust architecture](https://en.wikipedia.org/wiki/Zero_trust_architecture). Essentially, what this means is that every call checks for the identity and permissions of who makes the call. For any non-public call, authentication and authorization will be the first thing that the implementation does.

There are two objections to this type of design: performance and complexity. The performance impact is small and should not be a concern if lookups are done on a database that is fast enough. The complexity impact can be minimized by defining a single call that makes the authentication and authorization checks. Said call can "wrap" the other calls.

Interestingly enough, if we want to maintain zero trust, the internal calls originating from our system as a result from an external call can also send authentication and authorization information. This is not always necessary or desirable, but at least considering the possibility can significantly improve the security of the system, because then we leave behind the notion of being "inside". This treats security in a self-similar way, with every call potentially checking for identity and authorization.

As a North Star, it is worth upholding the [Kerckhoffs's principle](https://en.wikipedia.org/wiki/Kerckhoffs%27s_principle): don't rely on obscurity to protect your system. Instead, build security upon a clean, consistent design and solid cryptographic primitives.

### Scaling: consistency or performance

[Scaling](https://en.wikipedia.org/wiki/Scalability) a system is the act of adding more resources (memory and processors) to it, while keeping the system *correct*.

Adding hardware resources, in itself, is now very easy thanks to 1) the unbelievable size and speed of modern computers; 2) cloud providers which allow you to hire more resources on demand.

What is still hard about scaling is maintaining the correctness of the system when you scale it. This is the core problem of scaling.

Why do we need to scale a system, in the first place? We only need to scale a system if:

1. We need to store more data in it: if we don't have enough capacity to store the data, we can simply add more memory.
2. We want to improve the system's resilience: if we have our data in multiple computers, if one of those computer fails, we will still have multiple copies. This reduces the odds of losing data. It also reduces the odds of a call getting an error instead of a proper response.
3. We have to respond to more calls without the responses taking longer: we can add processors to handle calls **in parallel**.

Adding more memory, even when geographically distributed, is not challenging. As long as there is a design that puts every part of that new memory in the dataspace, the system will keep on working as it scales.

Point 3 above needs more explanation: imagine a system that can only do one thing at a time. This means that it can only respond to one call at a time; any other calls that come in have to be queued. Once the call currently being processed is responded, then the next call from the queue will be attended to. In systems with many concurrent users, this wait for the previous call can grow unacceptably. Any system that has to support multiple users, or a system that has one call that takes a very long time, will benefit from **parallel processing**.

A system that processes things in parallel is a system that *does multiple things at the same time*. In the context of scaling, this means that there are multiple processors responding to multiple calls at the same time.

The problem with a system that does multiple things at the same time is that, by doing so, it can yield incorrect responses. Consider the following system:

- We have a system with bank accounts.
- Money can be transferred from one account to another.
- No bank account may have a negative amount.

Now, the call for transferring money could look something like this:

```
transfer : m 1 @ if cond < . @ m from
                           . @ m amount
                    do res error "Insufficient funds"
             2 @ set dest m to
                     value @ + . @ m to
                               . @ m amount
             3 @ set dest m from
                     value @ - . @ m from
                               . @ m amount
```

In other words, we first check if the source account has enough funds. If it does, we add the amount to the target account and then withdraw it from the source account.

If this system does one thing at a time, the logic of `transfer` is correct. What would happen, however, if two calls for transferring money from the same account happened at the same time, and there was not enough money to cover them both?

If the calls happened at the same time, it could be perfectly possible that both transactions went through; more specifically, if the second transaction expanded call `1` (the conditional) before the first transaction expanded call `3` (the withdrawal), then we'd end up with a negative amount of money in the source account!

If we reshuffle the logic so that the withdrawal comes before the deposit, we might reduce the chance of an inconsistency, but not altogether eliminate it. Since calls don't happen instantly, no matter how fast they are, if our system does more than one thing at a time, we will encounter this issue.

What we are facing here is a *consistency* issue. We have logic that is correct if things happen one at a time, but that stops being correct if a specific set of parallel calls takes place. In the case of `transfer`, issues will arise if two transfers concerning related accounts happen in parallel. It's this shared nature of the data which makes parallel calls problematic.

Interestingly enough, adding more space (memory), even if distributed across multiple geographical locations, doesn't create consistency issues if you are doing things one at a time. But, since memory in disparate geographical locations can only be accessed by processors at the very same location, in practice increasing the amount of processors, and therefore we have the same problem.

Also interestingly enough, systems that are in a single computer but have multiple processors have the same problem, even if they don't have memory in different geographical locations. The problem of consistency or parallelism is not related with splitting a system in space.

Also also interestingly enough, we could encounter the same problem in a system that has a single processor. If the processor chooses to treat all calls equally and process them in parallel, it could perfectly be the case that it generates inconsistencies by expanding two calls to `transfer` at the same time (step 1 for transfer 1, then step 1 for transfer 2, then step 2 for transfer 1, etc.). So even with a single processor, expanding calls in parallel can generate the same type of problem.

To summarize our point so far: consistency issues arise when we attempt to respond to multiple calls in parallel, that is, instead of responding to one call and then to another call, and there is some shared data concerning both calls that is modified by one of the calls.

How could we tackle this problem? In my view, there are only two solutions.

1. We could restrict the system to process transactions involving a certain account one at a time. Whether this is achieved by [queues](https://en.wikipedia.org/wiki/Queue_(abstract_data_type)), [locks](https://en.wikipedia.org/wiki/Lock_(computer_science)), [database transactions](https://en.wikipedia.org/wiki/Database_transaction) or [consensus algorithms](https://en.wikipedia.org/wiki/Consensus_(computer_science)), the upshot is the same: one calls need to wait for the other. This is choosing **consistency over performance**.
2. We could just let transactions happen as quickly as possible, and report and fix consistency issues when we notice them. For example, in the example above, we could let `transfer` check if `@ m from` has now a negative balance, and if it does so, perform corrective actions or report the problem. This is choosing **performance over consistency**.

If consistency is chosen over performance, the challenge of scaling consists of figuring out how to let multiple calls happen at the same time while forcing them to wait as little as possible for other calls. Calls that are completely independent from each other can happen at the same time; calls that are not should be expanded one at a time.

If performance is chosen over consistency, the challenge of scaling consists of minimizing inconsistencies by adding checks and corrective actions in our system.

While parallelism is not the only cause of consistency failures, it is a very common one, as well as the hardest to eliminate. Other sources of data inconsistency can be:

1. Outright errors in logic. For example, forgetting to deduce money from the source account after crediting it to the target account.
2. Not checking for errors in multi-step sequences. For example, if the `+` operation fails when depositing funds but we still withdraw funds from the source account, the bank will lose money.

I prefer consistency over performance for the reason that a consistent system is easier to reason about. However, in many systems, loss of consistency might be bounded or negligible, and performance extremely important. The problem will often hint at the solution.

### Quality

By considering data, the substance that both makes and justifies information systems, we can now apply principles used for material manufacturing to data.
Considering informati

Implementing the Toyota Production System
- autoactivation
- flow backwards, with reactive

muri & mura as redraws that only hurt performance or also as inconsistencies (defects), respectively. muri is performance waste, mura is inconsistency.

testing
- convergence to mathematical proof
- to generate, you must understand the order of validations.
- see errors as valid outputs, validate all the way.

Simple systems are amenable to proof.

## Acknowledgments

OpenAI's ChatGPT models 4o and o1 have contributed very valuable feedback, and even encouragement.

## License

TODIS is written by [Federico Pereiro](mailto:fpereiro@gmail.com) and released into the public domain.
