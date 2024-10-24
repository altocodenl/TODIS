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

My hope is that, by making DIS simpler, more humans will be empowered to bring their best to the world.

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

Here I will propose a data representation based on *text*. While data representations can also be graphical (though always using text), I've chosen to go with the portability and compactness of text.

Whether you use this data representation or some other representation, it is my contention that without a clear and sufficient data representation, you cannot directly look at the data in a DIS. **Therefore, the first step towards seeing the data is to have a single representation of data** and use it for *everything*.

A data representation requires us to define two things:

- Ways to set boundaries between one *value* and another value. Values are discrete units of data.
- Specify basic *types* of data.

[Elsewhere](https://github.com/altocodenl/cell?tab=readme-ov-file#the-data-vocabulary-fourdata), I have presented a data representation, called *fourdata*. This representation is purely based in text and has four types of data:

1. Number
2. Text
3. List
4. Hash

Number and text are self explanatory. Those are *single* data types. For example, `1234`, or `Hello!`.

Single data types, however, need to be organized into structured wholes. Fourdata also provides two *multiple* data types, where one value can hold multiple values *inside* itself. The first multiple data type is the *list*, which is a sequence of ordered values.

```
1 Eggs
2 Butter
3 Lettuce
```

In the list above, each item has a number next to it. This is its *key*, which is always a number.

The second multiple data type is the *hash*. In a hash, the keys are texts:

```
born 1959
firstName Gustavo
lastName Cerati
```

Hashes don't have a particular order to their keys; however, fourdata orders them alphabetically, so that two equivalent hashes are represented with the exact same text.

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

**DEAR READER: this treatise is in its [Hadean stage](https://en.wikipedia.org/wiki/Hadean); everything below this message has to undergo intense transformations to achieve a more stable shape. Below are very roughly sketched areas. They are quite unreadable. If they don't make sense to you, it's likely because they don't make sense at all, yet.**

### Pillar 2: single dataspace

 Put all the data in a single dataspace. Unification. (and addressability is there if the data is split). Representation can be existence, whether it is there or not is not that important, as long as it can be understood to be there.
Data cannot be floating. It has to be somewhere. Path is how you reference a value. There's no notion of a value without a path. Everything exists in a space and everything has a handle. There's no "floating" or "dangling" data.

A particular point in the dataspace is a *place*. Places are data.

two servers
one database

Everything has a path. Address is path.

A space and a name are the same thing.

Let's call them keys. a path is one or more keys, followed by a value.

Component is where we draw the lines.
State of a component is the data inside the component at a point in time.
The data stored by the system at any point in time can be called "state". But we'll just call it the data of the component.


- Dataspace: access vs control. Open access, use control to determine when to block.

What makes an unified information space powerful is that you can address everything from it. This is why the web is powerful, because it is a single dataspace.

Not everything actually "is" in dataspace, but if you can map it, then it is there. For example, a relational database is not using cell, but you can associate its data and operations to the dataspace. That's how you can put it in the dataspace. Representation can stand for existence. But you need a part of your system to actually provide those mappings so that you can do "as if" it was there.

By focusing on the data, we also can just retain the essential details of the hardware and the network. The core concept we will examine is that of a *digital component* (or just *component*), which is both a source and a repository of data.
Let's first define what is a digital component. A digital component is something that can transmit, transform and store data. Draw the boundaries wherever you want: entire system, program, function.

Can you model a chip, with registers and memory locations as addresses?

main obstacle: fragmentation

### Pillar 3: call and response

: see the data at every level: coming in, at each transformation, going out. That's why we use logs! That's why layers are helpful!

pillar 3 is the central pillar. From communication to changes in data.
calls represent communication, transformation and storage. storage is considered calls to data repositories, like disks or memory? but no, even a register is a data repository. anywhere where you can put data is a repository, even if then you replace it immediately. it doesn't matter. then, why is storage important? Because you need to get it back. The place where you cannot store data is the network. But you can store it in registers, memory and disk and tape.

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

bytes: "01234567"

storage is a matter of timescale. while processing a call, data is stored in API. but that doesn't outlive the call.
side effect as a call that changes what you consider durable data that is somewhere else in the space where the response is written on the caller.

can see the final result of the call or can see all the intermediate calls.

call goes beyond csp and actor. more simple. three examples: computer instruction (without even assembler), function call inside a hll and an API call.

When you make a call, you allocate. Or rather, with the response, you call the storage.

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

- Obstacles: implicitness, being blind at the process

Communication as basis.
Read is write. get is a call. consider the data at rest as a queryable surface. there's no data in itself, only data that you can query. a read is a write on the readers end. a transformation that is symmetric in the read and write perhaps.

request model of data transformations:
- a component has a set of endpoints. component + endpoint give you an URL (universal resource locator).
- - there's then the request data itself.
   - http: request headers, body.
   - sql: query.
   - fs: operation + data.

responder or surface?

### Pillar 4: code is data

code as data that produces data. The call is data, the responder is data, the transformation is data. The result is only part of the transformation. Understand code in terms of sequences: linear, cond, iteration, jump. Program + call = result. Data1 + data2 = data3.

Write code in the same vocabulary that you use for data. It's already parsed. And it forces you to think all in terms of explicit data at every step. Also, it is unified.

- Higher level languages let you focus on data at a human level.
- The data from the call changes the sequence into something else.

Levels where you draw lines have sublevels down to a single chip operation.

a flow as a sequence.

the problem with expressions: they are not automatically referenceable from outside of their immediate context. solved by pillar 3.
the problem with statements: they are not data. solved by pillar 4.

- then there's what happens inside the component. only see what happens with regards to the other components. inner data mappings are irrelevant or fold. The essential computing model:
   - call
   - Variable subsitution as call.
   - Sequence.
   - Conditional.
   - Loop as conditional.
   - Errors: the essence is that they jump up many levels, through a different channel than the return. It can be seen as a conditional return based on value.

### Pillar 5: interface is code

 interface is code, therefore data.
this is all great for backend, but what about interfaces?
An interface is a way for a human to interact with software - always through hardware.
interface mapped to state! see the data being displayed and the possible transformations.

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
