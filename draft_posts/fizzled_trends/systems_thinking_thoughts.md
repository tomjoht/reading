---
title: Systems thinking thoughts
---


In this series, I've more or less arrived at the following conclusion:

* Technology's trajectory is to become ever more specialized.
* In a hyper-specialized world, the system view becomes lost.
* Technical writers, not being technical specialists, will lose relevance in authoring documentation themselves, becoming more editors and publishers for specialized engineers only.
* One area technical writers can exploit, however, is the systems view, which individual engineering teams often fail to understand.
* Writing more horizontal than vertical, technical writers can develop overviews of systems that describe all constituent parts, how they interrelate, and other big picture thinking and lifecycles/journeys in this system.

Systems view writing is horizontal. It encompasses all the components that make up a system and traces the lifecycle of common journeys through the system. For example, a typical system overview might be a "Life of a ________" narrative, with a typical example being the life of a web query. These narratives trace the journey of an action through an entire system.

Horizontal writing is hard and not frequently done. Why? Several reasons:

* Technical writers depend on engineering teams for information. If engineering teams themselves are specialized and lack the big picture, where then do technical writers learn all of this information? Tech writers will have to piece together the story through interviews across multiple teams, gathering pieces of a puzzle that they then assemble together themselves.
* Not many people ask for this systems overview. Since most engineers are specialized, they focus on a specific information need, such as parameters for an API. They don't necessarily need the systems view to achieve their tasks.
* Often times, the systems view becomes most relevant during onboarding, when engineers try to get a sense of the whole before moving into their specialized role. After a number of years, the engineer learns that he or she doesn't need to know anything beyond X, Y, and Z related to their role.
* Organizational boundaries reinforce the specialized knowledge within a technology company. Division Acme is responsible for component 1, Division Beta is responsible for component 2, and so on. The product consists of components 1-10, but the organizational divisions reinforce the idea that each division need only concern itself with what it owns. As long as it delivers its component, the product's overcall outcome doesn't matter.
* In a world where people are drowning in information, it's natural to carve out boundaries around what you need to know. Engineers quickly decide what they're responsible for and the information necessary for their roles. Many other parts of the system become irrelevant because they exceed what the engineer can feasibly understand and master.
* Few tickets that come into a system ask for the larger picture. For example, a user rarely files a ticket explaining that he or she doesn't understand the purpose of the product or what it does. The tickets usually focus on some small technical detail, such as missing parameter formats or a bug related to the data returned by an API. As such, no one drives technical writers to create this larger view.

What happens when the horizontal system overview isn't available? The developer portal becomes full of specialized documentation that resembles technical notes, explaining how to implement this or that service but with little context about why, or what dependencies it has, or how the system works as a whole.

The larger developer journey becomes lost. Documentation is something that requires handholding and supplementary slide decks or other information.

What does a systems view describe?

idea: horizontal writing might be what tech writers are really good at.
* how does this product relate to other company products in the same category?
* how does this product relate to products at competitor companies?
* what are all the components involved in the system, and how do they relate?
* what's the general workflow for some action through the entire system? what path does a "life of a ______" take?
* what are the points of interface across teams, where one team's services are rendered by another team, such as API they make available?
* who is the audience that needs this birds-eye view? engineers, product managers?

"what dependencies does component X have?". If



the hypothesis I've arrived at: as tech becomes more specialized, the systems view becomes lost. Almost every knowledge worker understands only their specialized sliver of the whole. the ability to document the big picture becomes its own specialized skill, since no one has such horizontal understanding to fully comprehend all the pieces of the whole. no understanding the whole puts knowledge workers at a disadvantage in solving problems because many problems are system-wide in scope.

example: understanding all the parts of a computer.

idea: horizontal writing might be what tech writers are really good at.
* how does this product relate to other company products in the same category?
* how does this product relate to products at competitor companies?
* what are all the components involved in the system, and how do they relate?
* what's the general workflow for some action through the entire system? what path does a "life of a ______" take?
* what are the points of interface across teams, where one team's services are rendered by another team, such as API they make available?
* who is the audience that needs this birds-eye view? engineers, product managers?

"what dependencies does component X have?". If
tech writers are poised for this because they don't need to go technically deep with each layer. instead, you provide more of a brief overview of the service, what it does in the role of this larger system, etc.

seeing this larger view is a much more challenging aspect of writing documentation.

problems:
- no one requests this documentation, but many feel the pain of its absence
- few tickets filed against lack of understanding of this larger view
- what if it's just the tech writers and knowledge workers who lack the understanding; for the audience, they already get this context.
- how do you actually document this? people sort of fall asleep at irrelevance. a diagram at the top that allows people to jump to specific parts in the workflow? 
- 


How do you diagram large and complex software systems?
Even with a relatively small software system, it's tempting to try and include the entire story on a single diagram. For example, if you have a web application, it seems logical to create a single component diagram that shows all of the components that make up that web application. Unless your software system really is that small, you're likely to run out of room on the diagram canvas or find it difficult to discover a layout that isn't cluttered by a myriad of overlapping lines. Using a larger diagram canvas can sometimes help, but large diagrams are usually hard to interpret and comprehend because the cognitive load is too high. And if nobody understands the diagram, nobody is going to look at it.

Instead, don't be afraid to split that single complex diagram into a larger number of simpler diagrams, each with a specific focus around a business area, functional area, functional grouping, bounded context, use case, user interaction, feature set, etc. The key is to ensure that each of the separate diagrams tells a different part of the same overall story, at the same level of abstraction.

See also Diagramming vs modelling for an alternative approach.https://c4model.com/

The C4 model vs UML, ArchiMate and SysML?
Although existing notations such as UML, ArchiMate and SysML already exist, many software development teams don't seem to use them. Often this is because teams don't know these notations well enough, perceive them to be too complicated, think they are not compatible with agile approaches or don't have the required tooling.


The C4 model is just a way to describe a software system, from different levels of abstraction,

One of the frequently asked questions (above) is about diagramming large and complex software systems. Once you start to have more than ~20 elements (plus the relationships between them) on a diagram, the resulting diagram starts to become cluttered very quickly. 
One approach to dealing with this is to not show all of the components on a single diagram, and instead create multiple diagrams, one per "slice" through the container (image 2, below). This approach can certainly help, but it's worth asking whether the resulting diagrams are useful. Are you going to use them and, if so, what are you going to use them for? Although the System Context and Container diagrams are very useful, Component diagrams for large software systems often have less value because they are harder to keep up to date, and you might find that very few people look at them anyway, especially if they are not included in documentation or presentations.

sounds good in theory but in practice you realize how complex this. understanding a technical system and all the parts, how they fit and work together, etc., is an enormous undertaking. unclear who the audience is for this. is it something writes can even do? 

another question is what scale would you describe? for example, the Gizmo API handles X versus 50 + pages of details about this API.

maybe writers have to go even higher up to connect the parts at a much higher level? 

c4model.com zooming in and out.

what approach to describing something so massive? 

who will maintain such a thing?

what use case are you solving for? onboarding? when users have to work across teams? i'm not sure this is the right approach.


seeing the whole
writing horizontal
how horizontal do you go? 
who is this view important to?

the GDG project
hard to write b/c unfamiliar territory

central thesis: as world becomes more specialized, there's an opportunity to focus on systems thinking/views. no one sees the whole anymore.

