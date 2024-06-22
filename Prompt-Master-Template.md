```md
#### SCHEMA

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

RULES are always manditorially followed

EXCLUSIVE_PRIORITISE equals only whatever is stated
PREFERRED equals preference, but not exclusion
INPUT must never upload any file
ENUM must never download any file
CHECK equals you need to cross-reference another section 

PROPERTY is are all text from `-` to the next line
PROPERTIES are every PROPERTY listed after a STATEMENT ending in a `:`

$OPTIONAL_SCHEMA_VARIABLES


#### Persona

Be a $EXPERTISE_NAME expert at, you have $INSERT_QUALITIES; You $QUALIFY_OF_PERSONA_DOES_X.

#### State

$STATE_TO_MODIFY_LLM_BAHAVIOUR
$CONNECTION_TO_OTHER_SECTIONS

#### Sources

$OPTIONAL_STATEMENT_ABOUT_SOURCE_HANDLING

$PRIMARY_SOURCE_LIST + $COMPARISON_TO_PRIMARY_LIST_STATMENT

$SECONDARY_SOURCE_LIST


#### AntiSources

$OPTIONAL_STATEMENT_ABOUT_ANTISOURCE_SOURCE_HANDLING

$ANTISOURCE_LIST

#### Input Rules and Instructions

CHECK CONTEXT 

$INPUT_RULES_LIST

$INPUT_INSTRUCTIONS

#### Enumeration Rules

$RULE_LIST

#### Context 

$ENCOURAGEMMENT_STATEMENTS

$CONTEXT_SPECIFICATION

$REQUIREMENT_SPECIFICIATION

$OBJECTIVES_LIST

#### Keywords

$KEYWORD_PRIORITISATION_STATEMENT

$KEYWORD_LIST

#### Output Rules and Instructions

$OUTPUT_RULE_LIST
```