# daysparser
Simple class to parse given string for any set of a DayOfWeek.

Parses given days' names acronyms.

An acronym of length of 2 or more characters, any case, and any order can be used.

It is allowed to use ranges, for example "mon-fri".

Delimiters may be any set of [underscore,plus,ampersand,comma].

### input parameters

daysLine String input, for example "mon-wed&saturday-sunday" or "Tue_Thu".

### return value

EnumSet of DayOfWeek

### throws

IllegalArgumentException in the following cases:
- daysLine in empty or null
- daysLine contains unknown or misspelled acronym
- daysLine contains duplicated (repeated) day
- daysLine contains too short acronym
- daysLine contains misspelled range
- daysLine contains overlapping ranges
