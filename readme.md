# The Organization of Digital Information Systems

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

Simple systems are easier to understand than complex systems. Rich Hickey [brilliantly defines simplicity](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/SimpleMadeEasy.md) as something that is not intertwined or entangled with other things; whereas complex things are things that are "folded together", therefore requiring you to understand them not just in isolation, but in all their possible interrelations.

According to [Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks), complexity can be divided into two: essential complexity, which is the minimum possible complexity of a system that implements a set of features; and accidental complexity, which is complexity that can be avoided by a better design. In other words, essential complexity is the minimum possible complexity of a given system.

Whether you pick Hickey's or Brooks' definition, the art of system design is the making of systems that are as simple as possible. For Fred Brooks, the main quality of simple systems is conceptual integrity. Conceptual integrity is an emergent property of a system that is designed by either one person or a small group of persons who have an unified vision of how the system should be. The notion of the concepts of the system being "integral" resonates deeply with Christopher Alexander's notion of strong centers as the main quality of good architectural designs. These two authors may well be talking about the same thing: a good system is composed of consistent parts that are organized harmoniously.

**The limiting factor of those who create information systems is complexity**. Data transformations, by themselves, are extremely cheap (in terms of the time and the energy used by the computer resources required to do them) and have extremely low error rates. It is the making and maintaining of a coherent information system that can make or break an organization, an institution, and even perhaps the global economy.

This is quite interesting, because in pre-information economies, it was energy, not organization, that is the limiting factor of the creation of wealth. Therefore the search for simplicity is not merely an interesting or reasonable pursuit: it is the central way in which complexity, the limiting factor of an information economy, and therefore of wealth creation, can be tackled.

Perhaps we can draw a line between simple systems and complex systems: simple systems are those whose complexity grows linearly (or less than linearly) with the value they produce; whereas complex systems are those which grow quadratically (or more) in complexity with the value they produce.

## The main thesis: to organize the system, always focus on the data

The main contention of this treatise is that *the* way to design simple DIS is to focus on the data that they communicate, transform and store. It is as simple as that.

Designing DIS is already a complex task. However, it becomes exponentially harder when those responsible for building or understanding a system are distracted by everything except the data it handles.

What is this everything else that holds the attention of makers or DIS? Here are a few examples:

- Programming languages.
- Programming paradigms.
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

If you take away one thing from this treatise, it should be this one: **if you are working with a DIS, look at the painting (the data) as much as possible. And ignore as much as possible the brush and the palette (The List).**

Why not look at data and focus on The List? Normally, nobody even asks this question. When I raised it, I obtained two arguments against looking at the data:

1. There's too much data, so we cannot look directly at it. That's why we have programming languages, programming paradigms, libraries, etc.
2. Data is just a detail. We should be focused on bigger, deeper things, not on low-level things.

This entire treatise is built on toppling these two myths with the following (hypo)theses:

1. Once we decide to look at the data directly, there are ways in which we can abridge it without losing descriptive power. And these ways are much simpler than The List. "These ways" is what fills up the rest of this treatise.
2. Makers of DIS are in dire need of humility. Simple data is powerful, even exciting. The details matter. They can be joined into harmonious wholes. But to eschew details because they are beneath oneself is *exactly* what's keeping us mired in a mess of our own making.

When the data is not seen, the trivial becomes difficult and the nontrivial impossible.

Data itself is simple and can be directly seen. By using data to understand and make a DIS, we can find the simplest possible expression of the system that will get the job done.

This is the central thesis of this treatise. We'll explore now how to make this a reality through five practical concepts, called pillars.

## The five pillars

1. **Vocabulary**: Have a simple and consistent data vocabulary. We use cell's fourdata, in alf (abridged line format).
2. **Unification**: Put all the data in a single dataspace. Unification. (and addressability is there if the data is split). Representation can be existence, whether it is there or not is not that important, as long as it can be understood to be there.
3. **Explicitness**: see the data at every level: coming in, at each transformation, going out. That's why we use logs! That's why layers are helpful!
4. **Code is data**: code as data that produces data. The call is data, the responder is data, the transformation is data. The result is only part of the transformation. Understand code in terms of sequences: linear, cond, iteration, jump. Program + call = result. Data1 + data2 = data3.
5. **Interfaces are data**: interfaces as windows to data, and themselves data.

### Pillar 1: data vocabulary

https://github.com/altocodenl/cell?tab=readme-ov-file#the-data-vocabulary-fourdata

main obstacle: lack of consistent data vocabulary

### Pillar 2: unification in the dataspace

Everything has a path. Address is path.

Let's call them keys. a path is one or more keys, followed by a value.

- Dataspace: access vs control. Open access, use control to determine when to block.

- Web is a single dataspace.

main obstacle: fragmentation

### Pillar 3: explicitness at every step

The traditional approach: input, program and result. For now, let's ignore the program and focus on the input and result, which are data. The focus is generally on those two, at best. The intermediate steps are not shown, except in logs or debugger.

- Logs are necessary as long as we're doing "blind manipulation of symbols" (get that quote).

- REST is great because it is about sending data for changes. Changes represented as data.
- Microservices give you more rest. Corba also. Vs rpc; rpc can be represented as data, but less contractual.

This is why REST is better than non-REST, why microservices are more tractable than monoliths.

- Obstacles: implicitness, being blind at the process

### Pillar 4: code is data

Write code in the same vocabulary that you use for data. It's already parsed. And it forces you to think all in terms of explicit data at every step. Also, it is unified.

- Higher level languages let you focus on data at a human level.

### Pillar 5: interfaces are code, therefore data

## On scaling, consistency and parallelism

- Distributed and parallel: consistency. Scalability with that assured is trivial (throw more nodes in), except for the "inside api" problem that Hickey points out.

## How to test the (hypo)thesis of this treatise

- inverse relationship between data hiding and system quality and ROI
- importance of observability
- security

## Applications of the theory

- Design
- Implementation & testing
- Security
- Running the system
- Sciences

DEAR READER: this treatise is in its [Hadean stage](https://en.wikipedia.org/wiki/Hadean); most of the stuff is there, but it has to undergo intense transformations to achieve a more stable shape. Below go many ideas that will probably make their way to the final version. They are quite unreadable, but if you're curious, there they are. If they don't make sense to you, it's likely because they don't make sense at all.

```

- New developments such as generative AI or big data don't change these facts; the paradigm is neutral towards them.
- The data from the call changes the sequence into something else.
- Digital information systems provide a central way to organize human society. Therein lies their importance.
- For security: make it about data, not about perimeter; it's zero trust but naturally. And kerchoffs principle: no unnecessary layers.

Reference to cell

Means of computation are widespread. The main problem is to organize them. Trivial operations compound.

Not difficulty of algorithms, just making coherent wholes.

Communication as basis.
Patterns: fire forget, fire and return (with optional value)
Read is write
This can explain everything

Levels where you draw lines have sublevels down to a single chip operation.

the hypotheses (plural):
- The best way to understand any information system is the data it transmits, transforms and stores.
- Data can be used to express concrete data sequences dynamically, not just statically.
- Any analytically capable person can read and write these data sequences.
- These data sequences define 90-99% of the implementation and its tests.
- Working on the data sequences directly is the most effective way to create a simple and reliable system.

a flow as a sequence.

Here I intend to explore software from the perspective of data, as a fresh angle that can yield useful insights. Our contemporary attitude towards software is focused, perhaps naturally, on software itself, and not on the data which flows through it and which justifies the existence of software itself. But it is perfectly possible to see code as the negative impression (just like a picture taken with film has a [negative](https://en.wikipedia.org/wiki/Negative_(photography))) of the data flows it enables.

By switching the emphasis from code to data, my goal is to find conceptual tools that can help us reason about and design better information systems. Fred Brooks' recommendation to tackle conceptual integrity was to try to fit the design in the head of a single architect, or of a small and highly coordinated group of architects. I am intrigued by the possibility of going beyond this, and finding conceptual tools that allow information workers to co-create information systems that evolve towards simplicity and create a harmonious whole, not unlike what workmen did five hundred years ago when building a cathedral.

By focusing on the data, we also can just retain the essential details of the hardware and the network. The core concept we will examine is that of a *digital component* (or just *component*), which is both a source and a repository of data.

It is my contention that the challenge of designing information systems in a simple way can be drastically reduced by understanding it in terms of data flows going through digital components. The architecture of the system can emerge from the desired data flows that the system will enable. More importantly, a concrete understanding of the system can emerge, with which we can understand, replace and modify existing information systems.

My hope is that through the very concrete abstractions of digital components and data flows, we'll be able to make more sense of our digital world, both as individuals and collectively.

### Data flows through digital components

"The fundamental problem of communication is that of reproducing at one point either exactly or approximately a message selected at another point."

Communication in the Shannon sense is done one way.
call and response model, it can all be understood like that
communication is about the call getting to the other side
here we study transformations.
what about reading? We can see it as a sort of call and response.

what about communication? that was covered by Shannon. We can assume that it can happen.

call is always a function call. the function call can be local, or make calls to toher processes - other processes can be seen as the network, whether local or outside.

things that fold onto themselves: function call, call to the OS, call to the network.

function allows you to have abstraction. function as a layer.
component is a function! indistinguishable.

return vs respond. control vs data. but isn't it the same, with the data taking over the channel for a while?

transform as communication, through call?

response = call + arguments + state

Read is a call. Transform is a call. Everything has an address. Call is to an address, the result is written to an address. Why? Because every piece of computation (one of the three) responds to a call.
It is all calls, even cron.
When you make a call, you allocate. Or rather, with the response, you call the storage.

Address 7890 of what you call. But what called it also has an address! Where's the execution is written? In another set of addresses. Internal would be one way, but what about when it involves an external server? Ir also has an execution space that needs ro be addressed. This has to be named.

Reactivity event system is just doing it through those calls through the event system.
This is the third layer?

Context is a way of resolving urls in a way where you're looking at the last part of the path starting from your area and then going one out. This is the second layer.

This is it. Together with the data types and the 10? Verbs.

Can you model a chip, with registers and memory locations as addresses?
A way to comfortably and directly represent all computation.
Yep, it's a new model for computation. Practical enough to implement, intuitive enough to directly understand.

Minimum verbs: reference and conditional. Assumes it is always going further. Without that assumption, you can see that a reference to the function is an execution. And therefore you need a quote foe the function itself. Is this the right way? Yes, because you execute functions far more than you reference/quote them.

Is there standalone data? At least in the arg calls?
Function is call
The response is the transformation of the call
Side effects as change in state that is indirect. If it was calls elsewhere without wrote no problem. An intended write to the DB coming from a POST would not considered side effect except for absolute purists.

data flow: data is text, but can be structured. discrete vs continuous flows.
digital component: conncomp/human
t
where do we draw the boundaries on both data flows and digital components? nested.
- for a data flow: call/response, only between two. to understand more complex things you can see them as chains of requests/responses.

data can be represented as text for humans to consume. there are other ways in which humans can see data, but we'll use text as the main one (later we'll see that interfaces, to a considerable extent, can be transformed to textual representations).
data can be communicated, stored and transformed through digital computers connected to the network.

Let's take a couple steps back.

Digital data can be represented as text. This text can be 1) read by humans (through interfaces); 2) processed digitally.

The digital is about text. A character is not a half character, but a whole one.

Let's first define what is a digital component. A digital component is:
1. A computer.
2. Connected to the internet.
3. That can run some software.

Digital components have the ability to communicate, store and transform data.

A small piece of the same program can be considered a component, if you want. Draw the boundaries wherever you want?

data must be serializable. if there's internal data shared, then represent that flow explicitly.

Lang is machine sat atop the machine. Also for humans. Transformation and communication happen, as well as retrieval. Humans as elements of an information system.
No need for an extra description layer, that's the software itself. The software itself rather than a concrete map. Leave funs undefined yet if needed.
It's not that we have to send multiple commands of the same kind, like enough soldiers for the battle, for it to go through. That's not the issue. There's a low error rate.
First define the data representation. Then extend. Data rep has no vars! The var is the first step.
Funs are lists that have each outermost step starting with a fun.
Deserialization as the beginning of structured data, from text to that. text is unstructured data.
message vs continuous flow. this is a boundary on time, and it could also be of chunks if you're multiplexing. see channel as only one at a time. this is what shannon gave us.

digital component: something running on top of hardware+software+network
the digital is physical, still physical. but so subtle, so compact, that that is what gives it its value.
Where you draw the boundaries?
within a computer you could have many services at the same time. and a service can be astride multiple computers.
single thread, computer and human with lang

paths: all can be expressed as path, the value is the last part!

Data vocabulary
Code vocabulary

Feat of null. Just empty string. Bool is n
empty string is '
we need to create a textual representation for all info

Shared mem
Single statement as machine?
Turing machine also catches of sorts

- the digital is physical
- where do you draw the boundaries?
- see data with a vocabulary
- all addressable in one space
- transformations: code
- you can draw the boundary at the atomic function level
- a practical example: a service with DB

how to see flows concretely, through layers? because the layers or elements we can draw boundaries around. what's the boundary for a dynamic process? does it happen with initiation and finish?

Is an abstraction layer just a transformation? Or perhaps just a component.

what I call a path is called a resource, even by Tim Berners-Lee

.and
.or
.if
.loop
like assembler instructions!

dot to specify access
.id

scope of memory
you have internal memory and external memory? no. you only have other components, and your own memory.
does this hold under a shared memory paradigm?

.define .hello
   1
   2
   3

.define .hello
   a 1
   b 2
   c 3

.hello.1
.hello.a

return as just having the address to which to jump to afterwards.
return is going to the next.

registers in arm:
- general purpose
- stack pointer: point to top of the current stack

R13 (SP, Stack Pointer): Used to point to the top of the current stack. It's essential in function call conventions and for managing the stack frame.
R14 (LR, Link Register): Used to store the return address in function calls. When a function is called, the address of the next instruction (return address) is saved in LR.
R15 (PC, Program Counter): Holds the address of the next instruction to be executed. It's effectively the pointer to the current point of execution in the program.

But what do we mean by data flows? A flow of data is data that goes through the boundary of the component of an information system. Information systems are made of components that are connected through a network, or through shared memory. When data comes to a component, we consider that to be a *request* done to the component.

Software is a set of instructions given to a computer to execute.
software is a set of data (calls) to modify data.

What makes an unified information space powerful is that you can address everything from it. You might not be allowed, but you can. There are no overlapping names. Think of telephone numbers, or URLs.

Use data to represent it

turing five argument function:
- current position of the tape
- value on the current position of the tape
- current configuration

this generates:
- optional write on the tape
- optional move on the tape
- jump to another configuration

request model of data:
- a component has a set of endpoints. component + endpoint give you an URL (universal resource locator).
- - there's then the request data itself.
   - http: request headers, body.
   - sql: query.
   - fs: operation + data.
- then there's what happens inside the component. only see what happens with regards to the other components. inner data mappings are irrelevant or fold. The essential computing model:
   - Sequence.
   - Variable subsitution as sequence.
   - Conditional.
   - Loop as conditional.
   - Function: which was implicit all along in your unit of what's going on. see the outermost handler of a request as a function. you can actually even see functions as components, because they really are.
   - Errors: the essence is that they jump up many levels, through a different channel than the return. They are irreducible.

I need a way to express try catches that can bubble up. the return never jumps levels.

scope of a function IS the autopoietic boundary of the center! scope, or rather closure. What's stunning about this is that the boundary, in an informational system, is about context, context being reducible to reference. Reference is a computation, a dereferencing that happens within a context as a data flow unfolds.

So:
- Address
- Incoming request
- List of requests done to other components, seeing how the data moves between subparts.
- Response.

but I need addressability of the sequence itself!

The two concepts of presentation and transformation of data hint at a conceptual elephant in the room: the system has an "inside" and an "outside". The data going from the inside to the outside of the system is the data being presented, while the data that comes into the system is the data being transformed. Some of the data being transformed will also be stored, while other parts of it will not. It is up to the information system to decide which data to store.

The data stored by the system at any point in time can be called "state". Henceforth, when we refer to the "state" of the system, we will refer to the entirety of the data that it stores.

A system does not emit data randomly. Systems are built to handle requests. A request is an incoming unit of data. In any system that functions correctly, the request will be processed and a response will be provided to the caller.

Requests and responses are done through the network; the network belongs to the "outside" of the system.

algorithmic challenge vs mapping challenge

this is all great for backend, but what about interfaces?
An interface is a way for a human to interact with software - always through hardware.
interface mapped to state! see the data being displayed and the possible transformations.

state machine 2 args?

interfaces + data flows - but isn't flow a lower level thing?

batch and queue is not storing, just presenting and transforming.
info system is executable by machines, hence a lot of calculations can be done cheaply and precisely.

surfaces, entrypoints + flows.
a system is a surface and can have multiple surfaces. better analogy than layer, because surfaces are not necessarily concentric.
request & response
families of data.
implicit contracts.

turing machine is an information system. but a single request and it keeps on going forever.

all the way down: chip + memory is info system, request is executed instruction with arguments, response is change to memory and next set of instructions. turing machine is an info system!

state as data inside the surface

auth as extra info. zero trust as checking the auth credentials with someone you trust. yet, how do you know that someone you trust is there? if https, it's not zero trust. it'd have to be through a key exchange, but what about getting the keys in the first place? you need to trust. if you're in the same place and then you separate, then you had a trust network that then got partitioned.

the code is a negative impression of the data flows

consider the data at rest as a queryable surface. there's no data in itself, only data that you can query. a read is a write on the readers end. a transformation that is symmetric in the read and write perhaps.

what do you mean by "details"? things you can change and still have the same system from the pov of outside the surface. it's relative to your frame of reference.

amenable to proof.

lowest level: machine code. highest level: specify the data transformations and the code is generated by an algorithm.
data grammar: the constructs to express data transformations. not constraints, transformations. the family of transformations also defines the constraints.

understanding CAP: when distributed surface (distributed as amenable to experiencing partitioning) receives data, it either rejects (rejection as the lack of upating and also reading, indicating that that's not data) and presents/maintains consistency, vs remains available and has either temporary or permanent inconsistency. consistent system, in a partition does not present or update state, only stores it.

by oop nesting, you cannot just bring things from the side

request response vs call response. the core is request response. event system does the calls, in practice. listener as a polling

rest vs sql
sql could be databases, could be tables.
funny how graphql is like sql.

data on the wire vs data ready for processing.

metcalfe on info space. reverse: utility of the network (network size squared) as multiplier of the value that a system can bring.
but that makes no sense. we already have one network.

## implications for existing systems

data discovery!
- look at the data first, the logs second, finally the code.
- use data tools to look at the data.
- you can replace only parts of the system by doing 80/20.
- valuable code is only that that performs nontrivial operations, and can usually be isolated.
- the core is to find the data constraints of the system.
- contrast with data as done today: don't just look at the data at rest, look at the data going through boundaries to understand the mappings/transformations.

- setup flows:
   - rest requests
   - websockets requests
   - db queries
- analysis:
   - network analysis (who whom)
   - 80/20 analysis of endpoints & body forms
   - use llm to analyse bodies
- implications for rebuild:
   - know what's really going on
   - go look for essential code that produces certain transformations

implications for new systems
- design the data flows.

implications for testing
- convergence to mathematical proof
- to generate, whitelist
- and yet, how to do it from existing thing?

implications for disciplines
- economics: economic system as information system to determine resource use constraints without recourse to legal intervention or force. info system as the "business as usual" allocation of resources, except for force or law changes.
- biology: autopoiesis: see surfaces internally that communicate with each other. it's like input output but with many families per surface + entrypoint. and notion of no data in itself, only read or written, makes everything autopoietic. what's the equivalent of data in biology? an info system has always constant voltage/energy, it is very very controlled/unchanging. life flows with bursts of energy and matter; perhaps there could be a data representation of matter and energy as information. but this would miss the truth, because data
```

## License

TODIS is written by [Federico Pereiro](mailto:fpereiro@gmail.com) and released into the public domain.
