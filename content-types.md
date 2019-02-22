# Content

There are two types of content in any organization **structured** and **unstructured**.

Atomic writing does not preference either type. Modern documentation stacks should handle both, and the interleaving of both, with equal ease.


## Unstructured Content

Unstructured content is any content that does not follow a specific pattern. In unstructured content, the _flow_ (ordering, "feel") of writing is more important than the _semantic structure_ of writing. 

For a technical writer, this can be a daunting concept, but there are all sorts of perfectly valid reasons that content
might not follow an established pattern or not be strictly a Concept, Reference or Task. To illustrate this concept, let's look at React's documentation: https://reactjs.org/docs/introducing-jsx.html

On this page, the heading levels aren't semantic (in the sense that they define discrete concepts, tasks, and references) – but they serve the writing's _flow_. 


Unstructured content can contain structured content blocks, if needed, but these are always secondary to the flow of any given content section. 


## Structured Content

Structured content is any content that must conform to a strictly defined pattern. Patterns are defined and described by the teams doing the writing. In structured content, the _semantic structure_ of the writing is more important than the _flow_ of the writing.

Examples of structured content are as follows:

* UI tasks with numbered steps
* API References
* Release notes

Structured content is _not_ a content taxonomy or classification in the traditional Information Mapping/DITA sense. API Referneces can have conceptual information in them if the team decides it's nessecary, for example. Structured content follows a predictable pattern which can be validated against and (in some cases), automated. 

The key of atomic writing is in flexibility, so structured content can contain unstructured content blocks if the pattern allows

## Content blocks

A content block is a chunk of content and a header. 

Content blocks are single-concern sections of content. 










For example: 
* Tutorials, which ideally weave through ordered steps, pedagogic explanations, introductory concepts, explaining and presenting alternatives, etc. 
* Recipes, which provide both a reference code sample and a break-down of the code sample
* Philosophy essays, like this one, which introduce a way of thinking that might be relevant to your users, but are decidedly _not_ concepts.
* Compatability matrices, and other documents designed to guide users through a descision-making process. 
* FAQs and other question-and-answer type documentation (knowledge base articles, i.e.)
* Walk-through blog posts which talk about what _one person did_ in _one specific instance_, and provide wisdom/learnings.

You'll notice some of these examples are things which do _have_ structure, however – for example, FAQs typically have blocks of 
question-and-answer formats
Unstructured content can include modules of structured content, but structured content does not include unstructured content.
