# Content

There are two types of content in any organization **structured** and **unstructured**.

Atomic writing does not preference either type. Modern documentation stacks should handle both, and the interleaving of both, with equal ease.


## Unstructured Content

Unstructured content is any content that does not follow a specific pattern. In unstructured content, the _flow_ (ordering, "feel") of writing is more important than the _semantic structure_ of writing. 

For a technical writer, this can be a daunting concept, but there are all sorts of perfectly valid reasons that content
might not follow an established pattern or not be strictly a Concept, Reference or Task. To illustrate this concept, let's look at React's documentation: https://reactjs.org/docs/introducing-jsx.html

On this page, the heading levels aren't semantic (in the sense that they define discrete concepts, tasks, and references) – but they serve the writing's _flow_. There are some sections which seem to follow a similar pattern ("Embedding Expressions in JSX", "Specifying Attributes in JSX") but the point of this document _isn't_ to provide consistent structure and patterns, it's to introduce a set of interrelated background topics to the user so they're prepared for the next sections.

Unstructured content can contain structured content blocks, if needed, but these are always secondary to the flow of any given content section. 

Some other examples of unstructured content can include the following:

* Tutorials, which ideally weave through ordered steps, pedagogic explanations, introductory concepts, explaining and presenting alternatives, etc. 
* Recipes, which provide both a reference code sample and a break-down of the code sample
* Philosophy essays, like this one, which introduce a way of thinking that might be relevant to your users, but are decidedly _not_ concepts.
* Compatability matrices, and other documents designed to guide users through a descision-making process. 
* FAQs and other question-and-answer type documentation (knowledge base articles, i.e.)
* Walk-through blog posts which talk about what _one person did_ in _one specific instance_, and provide wisdom/learnings.

Unstructured content is inherently subjective: for example, in some organizations, tutorials and FAQs are highly standard in structure, and might be considered structured. 

With zero substantiation behind this statement: I think that all content starts in some way unstructured, and evolves into structured content as required. Structured content is fundamentally emergent. Bottom-up structuring, rather than top-down.



## Structured Content

Structured content is any content that must conform to a strictly defined pattern. Patterns are defined and described by the teams doing the writing. In structured content, the _semantic structure_ of the writing is more important than the _flow_ of the writing.

Examples of structured content are as follows:

* UI tasks with numbered steps
* API References
* Release notes

Structured content is _not_ a content taxonomy or classification in the traditional Information Mapping/DITA sense. API Referneces can have conceptual information in them if the team decides it's nessecary, for example. Structured content follows a predictable pattern which can be validated against and (in some cases), automated. 

The key of atomic writing is in flexibility, so structured content can contain unstructured content blocks if the pattern allows. However, this should be avoided. 

The key advantage of using structured content is for **validation**: because structured content follows a predictable structure, rendering components can be designed around them, and their visual output can be validated using modern testing methodologies.

## Content blocks

A content block is a chunk of content and a header. 

Content blocks are single-concern sections of content.  Once again, the content writers determine what "single concern" is to them. However, the DITA definition of a "topic" comes in handy:

> A topic is a unit of information with a title and content, short enough to be specific to a single subject or answer a single question, but long enough to make sense on its own and be authored as a unit.

Beyond that, content blocks are semantically undefined. Because we author using Markdown or similar lightweight text markup languages, we do don't include any metadata, tags, assosciations, keywords, etc. in a content block. These concerns should be factored out to _rendering components_. 

Atomic writing should prioritize **human-readable content** at the content block level. 


## Technical Implications

### File structure

A system supporting Atomic Writing must allow for the following:

* Content blocks which can be referenced easily, using a UUID or similar. Normal markdown linking (relative paths) also works.
* Embeddable content blocks
* 
