# Introduction
Project 07 focuses on Borrows -Wheeeler Transform, an algorithm which compresses data in order to maximize space. The algorothm BWT, reencodingarranges a character string into runs of similar characters, making it more susceptible to compression techniques like to move-to-front and run-length encoding. The BWT works by sorting all possible rotations of a string lexigraphically and then extracting the last column of the sorted matrix. 

# Pseudocode
Put pseudocode in this box,

```
FUNCTION BWT(string)
    special_character ← "$"
    string ← string + special_character

    INITIALIZE rotations AS empty list

    FOR i FROM 0 TO LENGTH(string) - 1 DO
        APPEND string TO rotations
        string ← shift_right(string)
    END FOR

    SORT rotations lexicographically

    last_chars ← empty string
    FOR EACH rotation IN rotations DO
        last_chars ← last_chars + LAST_CHARACTER(rotation)
    END FOR

    RETURN last_chars
END FUNCTION

```

# Successes
I was bale to build majority of the functions until I gpt til the last two. Felt great about this and my coding ability.

# Struggles
I had issues understanding some parts implementing these functions. Also understanding the earlier graphs an

# Personal Reflections
## Group Leader Earl
I had to re-read this project multiple times and dig deep in some old notes for the coding aspect. I did comfuse myself with obtaining the output to match the examples, especially the last two functions. I
started to think this algorithm was pointless and useless, but had to think about its' application in the biotech field.

## Other member
NA

# Generative AI Appendix
I used AI to decode some of the instructions in the html file to help understand more what I need to do to build the functions. I also used AI to help write my pseudo code due to trying to get this in right before work and trying to understand why the last two functions were not working.
