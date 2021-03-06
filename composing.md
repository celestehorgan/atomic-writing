# Composing atoms

If, as discussed in [Content](content.md), we store our content in "atoms", or topic-scoped content blocks, then how do we render these onto a page?

On the whole, particularly in relation to developer documentation, the preference is for longer pages with well-structured subsections

## A prelude: the pitfalls of structured writing and semantic metadata

Before we talk about composing layers, let's talk about the one greatest irritations normal people have when engaging with structured authoring markup languages: the pitfalls of semantic metadata.

Semantic metadata is often touted as one of the biggest advantages of structured writing markups: by tagging things semantically, we can render blocks of content based on their meaning, and validate formatting based on the semantic type of content present. 

What structured authoring through use of semantic metadata misses, however, is this makes documents _irritating to read._ Documents which are irritating to read are irritating to collaborate on, without specialized knowledge. Documents which are irritating to collaborate on aren't updated and aren't useful to the user.

Traditionally, this means that no one but trained technical writers update documentation. However, a "hands off" policy simply doesn't work in software, let alone in highly autonomous, self-organizing Agile development environments. 

Documentation is a cross-cutting concern. It reaches its fullest potential to help the user when stakeholders from various groups – development, support, client services – can contribute anything from a quick grammar fix to long chunks of documentation. Trapping documentation away behind arcane markup formats does not achieve this.

## Back to the composition layer thing

In atomic writing, rather than worry about normal structured authoring concepts, like semantic tagging and namespaced markup languages, we emphasize the creation of human readable content. 

We add back in semantic concepts, like typed content, when we compose our atoms into larger content. This keeps the content itself readable by regular human beings, and keeps structured authoring abstractions – templates and layouts, topic-by-topic flow, 

_seperation of semantic metadata and human-readable content_. 


## Seperation of concerns

In Atomic Writing, atoms (Content blocks) are always human-readable content. What this means is that we need a seperation of concerns..

* Between _authoring_ and _rendering_
* Between _a single page_ and _the files which make up the page_ 
* Between _the files that make up a page_ and _how the page is rendered_

To the extent possible, we seperate writing from structure and presentation.

The goal is always _human readable and human editable content_. Anything else is too annoying to deal with. 

## Technical Implications

However, in most modern web application architectures, presentation and content aren't seperated. Moreover, it's a misleading idea to think that content and presentation are _ever_ entirely seperate: Bulleted lists, headings, and tables are examples of presentation-in-content. The display of these elements is inherently related to the nature of the content they house. In other words, presentation influences meaning.

An implementation should do the following:

* As a user, I want to author in _plain markdown_ whenever possible.
* When needed, I want to pass _a plain markdown file_ to a _rendering component_ to display it in a particular way.
* The _rendering component_ should..
  * provide formatting or interactive functionality 
  * provide validation(?) of the content in it. 
  


