# CHAPTER 2 - SENDING MESSAGES ON VOICE

## 2.1 INTRODUCTION

Transmission of formal written traffic by voice confronts the amateur with difficulties of voice perception when attempting to convey form and content with precision. This chapter presents voice message exchanging protocols and two-station voice exchange procedures.

## 2.2 VOICE TRANSMISSION TOOLS

### 2.2.1 Phonetic Alphabet
Standard ITU phonetic alphabet must be used for clarity:
```
A - Alfa        J - Juliett     S - Sierra
B - Bravo       K - Kilo        T - Tango  
C - Charlie     L - Lima        U - Uniform
D - Delta       M - Mike        V - Victor
E - Echo        N - November    W - Whiskey
F - Foxtrot     O - Oscar       X - X-ray
G - Golf        P - Papa        Y - Yankee
H - Hotel       Q - Quebec      Z - Zulu
I - India       R - Romeo
```

### 2.2.2 Pauses and Interruptions
- **Natural pauses**: Between logical groups
- **Interruption readiness**: Pause frequently to allow corrections
- **Listening periods**: Monitor for "break" or questions

### 2.2.3 Prowords (Operational Words)

#### Essential Prowords
- **NUMBER**: Before message number or SVC
- **END**: End of message  
- **BOOK OF (#)**: Multiple messages follow
- **END BOOK**: End of multiple messages
- **BREAK**: Separates message parts
- **I SPELL**: Phonetic spelling follows
- **I SAY AGAIN**: Repeat for clarity or correction
- **NO MORE/ONE MORE/MORE**: Quantity remaining
- **OVER**: Your turn to transmit
- **ROGER**: Message received and understood

#### Introductory Words for Groups
- **FIGURE(S)**: Number group(s) follow
- **TELEPHONE FIGURES**: Phone number follows  
- **INITIAL**: Single letter follows
- **INITIALS**: Letter group follows
- **MIXED GROUP**: Letters and numbers combined
- **AMATEUR CALL**: Call sign follows
- **ARL**: ARRL numbered radiogram follows

## 2.3 VOICING RULES

### 2.3.1 Mandatory Phonetics
**Must use phonetics for:**
- All letters in preamble except numbers and "X"/"R"
- Addressee names and critical address information
- Mixed groups containing letters
- Amateur call signs
- Any letter that might be misunderstood

### 2.3.2 Voicing Message Parts

#### Preamble Voicing
```
Example: "1 R HXE W1AW 12 NEWINGTON CT 1830Z JUL 1"

Voiced as:
"NUMBER ONE, ROUTINE, HANDLING INSTRUCTIONS ECHO, 
WHISKEY ONE ALFA WHISKEY, CHECK ONE TWO,
NEWINGTON CONNECTICUT, ONE EIGHT THREE ZERO ZULU,
JULY ONE"
```

#### Address Voicing
```
"DONALD R SMITH
164 EAST SIXTH AVE  
RIVER CITY MD 00789
301 555 3470"

Voiced as:
"DONALD ROMEO SMITH
ONE SIX FOUR EAST SIXTH AVENUE
RIVER CITY MARYLAND ZERO ZERO SEVEN EIGHT NINE  
TELEPHONE FIGURES THREE ZERO ONE FIVE FIVE FIVE THREE FOUR SEVEN ZERO"
```

#### Text Voicing
```
"THANKS FOR MESSAGE X HOPE TO SEE YOU AT HAMFEST X 73"

Voiced as:
"BREAK
THANKS FOR MESSAGE X HOPE TO SEE YOU AT HAMFEST X SEVEN THREE
END"
```

### 2.3.3 Special Group Types

#### Mixed Groups
Groups containing both letters and numbers:
- **146R52**: "MIXED GROUP ONE FOUR SIX ROMEO FIVE TWO"
- **N2ABC**: "AMATEUR CALL NOVEMBER TWO ALFA BRAVO CHARLIE"

#### Email Addresses
- **W3ABC ATSIGN DOMAIN DOT COM**: "WHISKEY THREE ALFA BRAVO CHARLIE AT SIGN DOMAIN DOT COM"

#### Spelling Requirements
- Spell phonetically when requested with "I SPELL"
- Use "letter spelling" for simple letter sequences when appropriate
- Always confirm difficult or unusual spellings

## 2.4 THE MESSAGE EXCHANGE

### 2.4.1 Transmitting Guidelines

#### Sending Speed
- Match receiving station's capability
- Slow enough for accurate copying
- Natural speaking pace with clear enunciation

#### Pausing Strategy
- Pause after each logical group
- Allow time for "break" interruptions
- Monitor for fill requests

### 2.4.2 Receiving Guidelines

#### Copy Requirements
- **Transcribe exactly**: Word for word, group for group
- **No modifications**: Don't "fix" apparent errors
- **Verify every group**: Ask for fills when uncertain
- **Accept responsibility**: Only take messages you can handle

#### Fill Requests
Standard format for requesting repeats:
- **"WORD AFTER [group]"**: Next word after specified group
- **"WORD BEFORE [group]"**: Previous word before specified group  
- **"ALL AFTER [group]"**: Everything after specified group
- **"ALL BEFORE [group]"**: Everything before specified group

### 2.4.3 Exchange Examples

#### Example 1: Basic Message
```
TX: "STATION WITH TRAFFIC FOR N1ABC, THIS IS W2XYZ"
RX: "W2XYZ, THIS IS N1ABC, READY TO COPY"
TX: "N1ABC, W2XYZ, ONE MESSAGE, NUMBER..."
[Complete message transmission]
RX: "I COPY ONE MESSAGE, CHECK ONE TWO, ROGER"
TX: "ROGER, W2XYZ CLEAR"
```

#### Example 2: With Fills
```
RX: "WORD AFTER HAMFEST"
TX: "WORD AFTER HAMFEST IS X"
RX: "ROGER, CONTINUE"
```

#### Example 3: Check Verification
```
RX: "I SHOW CHECK ONE THREE"
TX: "NEGATIVE, CHECK IS ONE TWO"
RX: "I SAY AGAIN, FIRST INITIALS"
TX: "FIRST INITIALS ARE TANGO FOXTROT MIKE"
RX: "ROGER, CHECK ONE TWO, THANKS"
```

## 2.5 BOOKING MESSAGES

### 2.5.1 When to Book
Booking is optional but useful for:
- Multiple similar messages
- Special events with many greetings
- Time-saving when patterns exist

### 2.5.2 Book Structure
```
"BOOK OF THREE TO ONE STATION"
[First complete message]
"BOOK MESSAGE TWO"
[Only different parts]
"BOOK MESSAGE THREE" 
[Only different parts]
"END BOOK"
```

### 2.5.3 Booking Examples

#### Fixed Preamble and Text
```
"BOOK OF TWO, FIXED PREAMBLE AND TEXT TO ONE STATION"
"5 R W2ABC 8 BALTIMORE MD JUL 15"
"JOHN SMITH, 123 MAIN ST, BALTIMORE MD 21201, 410 555 1234"
"BREAK, HAPPY BIRTHDAY X BEST WISHES X 73, MARY"

"BOOK MESSAGE TWO, ADDRESS ONLY"
"ROBERT JONES, 456 ELM ST, BALTIMORE MD 21202, 410 555 5678"
"END BOOK"
```

## 2.6 STATION OPERATIONS

### 2.6.1 On Net Frequency
- Exchange brief messages on net frequency when directed
- Acknowledge assignments promptly
- Return to net control when complete

### 2.6.2 Off Net Frequency (Stacks)

#### Establishing Contact
```
"W2XYZ FROM N1ABC WITH PRIORITY TRAFFIC"
[Repeat call 2-3 times if no answer]
[Move to alternate frequency if needed]
```

#### Two-Station Exchange
- Complete all assigned traffic
- Handle in precedence order  
- Verify all checks and copies
- Exchange courtesies appropriately

#### Returning to Net
Report completion status:
- **"N1ABC RETURNING, QRU"**: All traffic handled
- **"N1ABC RETURNING, QTC 2"**: Unable to complete, have 2 for reassignment

## 2.7 MULTIPLE MESSAGES

### 2.7.1 Sequence Planning
- Handle by precedence order
- Group similar destinations
- Announce total count: "QTC 4 - TWO PRIORITY, TWO ROUTINE"

### 2.7.2 Progress Tracking
- Keep running count
- Announce remaining: "TWO MORE" or "ONE MORE" or "NO MORE"
- Verify totals at completion

## 2.8 COMMON VOICE PROCEDURES

### 2.8.1 Standard Acknowledgments
- **"ROGER"**: Understood/received
- **"STAND BY"**: Wait/pause transmission
- **"NEGATIVE"**: No/incorrect
- **"AFFIRMATIVE"**: Yes/correct

### 2.8.2 Emergency Procedures
- Emergency traffic takes absolute priority
- Use "BREAK BREAK BREAK EMERGENCY" to interrupt
- Clear frequency immediately for emergency traffic
- Resume normal operations only when emergency cleared

### 2.8.3 Quality Control
- Verify check counts on all messages
- Request fills for any uncertain groups  
- Confirm unusual names, addresses, or technical terms
- Maintain professional demeanor throughout

This chapter establishes the foundation for professional voice traffic handling, ensuring accurate message transmission while maintaining efficient net operations.