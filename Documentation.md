# Documentation

#### Schema

Schema section defines variables and logic per section, cross-sections. Below mandatory:
```markdown
#### = Section Headers
-- = Comments ignore these if indent 0,1

All Schema Variables are uppercase words:
PERSONA = All information in #Persona section
STATE = All information in #State section
SOURCES = All information in #Sources section
ANTISOURCES = All information in #AntiSources section
RULES = All information in #Persona section
INPUT = All information in #Input-Rules-And-Instructions section
ENUM = All information in #Enumeration-Rules-And-Instructions section
KEYWORD = All information in #Keywords section
OUTPUT = All information in #Output-Rules-And-Instruction section
```

Custom variable allow LLM to cross referencing properties or section originating properties that try to create informational clustering by design to attempt to constrain the weirdness of LLMs. Best practice is similar to Nix-esque - it does one thing and it does it very well. Custom variables follow a simple syntax:
```markdown
-- SVO/OVS
-- Subject Verb Object or Object Verb Subject
VARNAME1 = LLM readable (so human readable) sentence SVO or OVS structure
VARNAME2 = variable can also alter other variables if encoded as a condition
```
#### Persona

Persona section defines properties for the LLM to impersonate or appropriate that have a human equivalent regard anything that is verb about a profile; so a Medical Doctor with a speciality in particular area of medicine. Try to use real world emulatable equivalents that are extreme specifics of how, quality level and description of what tasks the Persona does. 
#### State

State section defines properties for the LLM to impersonate or appropriate; Jason Haddix refers in [Practical AI for Bounty Hunters @jhaddix - https://www.youtube.com/watch?v=DqgterfPHzg](https://www.youtube.com/watch?v=DqgterfPHzg) to research of hand about description extreme emulatable human states affecting the LLM capability. 

#### Sources

Sources section defines sources to use as lists and prioritisation statements. Think of it a whitelist with prioritisation. The primary should have been vetted and could be used to compare to other sources. 
#### AntiSources

AntiSources section defines sources to avoid use as lists and prioritisation statements potential. This is limit crawling into data sources that could containment or hijack the host or LLM in anyway. Threat models and purposes are different so think of this a blacklist to sources

#### Input Rules and Instructions

Input Rules and Instructions section defines any rules or logic or instructions about how data handled from hosted input data. **Input is not the same as Enumeration**.This is separate about control flow to minimise weird instruction race/prioritisation conditions or odd behaviour of LLMs. A picture hosted local used to compare other images would be an example of input. 

#### Enumeration Rules and Instructions

Rules and Instructions section defines any rules or logic or instructions about to find and interact with sources. **Input is not the same as Enumeration**. This is separate about control flow to minimise weird instruction race/prioritisation conditions or odd behaviour of LLMs. Tools that are hosted that used during crawling sources would be example of thing hosted locally that is use, but should not be in the input section.

#### Context

Context section defines any schemata about context. This could be in similar schema section syntax or human readable like writing a short story setting. If the later it is worth optimising with other LLMs that have been trained on reading books to provide critique and improvement as author has noticed that humans get inherently narcissistic surrounding anything that they create that is artist including Creative Writing; consider how your cooking always tastes better, there are probably evolutionary reasons for this. 
1. Provide objectives
2. Specification about the context; so there is metadata for the LLM to understand the statements about a context you have provided
3. Use a markdown block with three tildes to start and end the block 
	- This is try a make the context data not contaminate into other properties of the prompt.
#### Keywords

Context section defines any Keyword, rules and logic about how to process Keyword. A Simple list with variables to link or mutate other section would probably be optimal.

#### Output Rules and Instructions

Output Rules and Instructions section defines any Rules and Instructions about output. This should be a list of separate Rules and Instructions; A rule would be `for any url link ALWAYS defang`  and instruction would be `Format all output into a Report in Markdown`, but `Report needs to have Berkley Reference style` could be either rule or instruction so with Prompt engineering it will depend on LLM, so trying to think in both and test both could change results.