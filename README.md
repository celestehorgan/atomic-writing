# The Atomic Writing Manifesto

Topic based writing for the "learn to code" generation.

Structured authoring did not make the jump into modern web applications smoothly. Documenting Software as a Service systems, continuous delivery and cloud-based models simply is cumbersome and tired in DITA XML based systems. While the 

## The proposal

* Use [MDX](https://mdxjs.com/) and a system of React Components to model the a lightweight structured authoring environment
* Encourage atomic writing – decompose documents into modular blocks and compose them into pages and guides/books using React
* Build components for serving up conditionals, props, and managing translation.
* Build components for multiple output streams
  * But, prioritize **topic based authoring** concepts over single sourcing concepts.
  
**Goals**: 
  * make documentation easy (and familiar?) to manage for technical writers, but modular and extensible for developers.
  * handle complex documentation topics (props, conditionals, etc.) with ease
  * make markdown more semantic and rendering more contextual
  * allow for **easy** extension of the base set of components by adding your own components.
  * Allow for **easy** interactivity and advanced visual design of documentation **with as little interference as possible in the text content**  -----> MODULAR DOCUMENTATION DESIGN
   * Allow for **easy fallback to a reasonable non-interactive version** of the content allowing for single sourcing with further implementation
  * Make **visual design** of documentation testable using **modern web development practices and frameworks**, while making **actual text readable by humans and parse-able by linting tools** to improve and automate the writing process


Is this a standard which is implemented or an implementation?


## Princples

### Atoms: Content blocks

* The _key module component_ is a block of content.
* A content block has at a minimum:
  * A header
  * some content
* Content blocks can be as small as the minimum or as large as is needed. The spec does not seek to define what a semantically relevant content block is for any given project. 
  * The project defines the size and conventions of content blocks depeding on their needs. Allow for emergent standards (i.e. angular-style commit messages
* Content blocks should be _readable by humans_, beginning to end, without needing a rendering or compiling engine.


### Molecules: Composers 


### Organisms: Sites or site sections
