# CHAPTER 1 - THE ARRL MESSAGE FORMAT

## 1.0 INTRODUCTION

The standard ARRL message format is used to send written amateur radio messages throughout the National Traffic System (ARRL NTS) and independent nets. The format is standardized to provide a uniform means of originating, handling, and tracking messages.

A message is considered a "formal" radiogram when completed with a correctly formatted preamble, address, text and signature. Stations in the system are not obligated to handle incomplete or improperly formatted messages.

### Message Structure
The ARRL standard message consists of four main parts:
1. **PREAMBLE**: Information to track the message
2. **ADDRESS**: Name and address of the intended recipient (with optional delivery "Op Note")
3. **TEXT**: The message information
4. **SIGNATURE**: The party for whom the message was originated (with optional service/reply "Op Note")

### Character Rules
The ARRL radiogram consists of GROUPS using ONLY three character types:
- **LETTERS** (all upper case)
- **FIGURES** (numbers)
- **SLASHES** (/) - used to separate characters within a group

### Special Substitutions
- **"X"** - substitute for a period (never used as last group of text)
- **"R"** - substitute for decimal point within figure groups (7013R5 = 7013.5)
- **"DOT"** - substitute for period in email addresses/URLs
- **"DASH"** - separates 9-digit US zip codes (12345 DASH 6789)

Other punctuation must be spelled out as word groups.

## 1.1 EXAMPLE MESSAGE

```
1 R HXE W1AW 12 NEWINGTON CT 1830Z JUL 1    (PREAMBLE)
DONALD R SMITH                              (ADDRESSEE)
164 EAST SIXTH AVE                          (ADDRESS)
RIVER CITY MD 00789                         (CITY/ST/ZIP)
301 555 3470                               (TELEPHONE)
THANKS FOR MESSAGE X HOPE                   (TEXT)
TO SEE YOU AT HAMFEST                      (TEXT)
X 73                                       (TEXT)
DIANA                                      (SIGNATURE)
```

## 1.2 PREAMBLE PART

All messages must have a preamble containing tracking information that remains with the message to delivery point.

### Preamble Components
```
NR   PREC  [HX]   STN-ORIG  CK   PLACE-ORIG  [TIME]  MON  DAY
1     2     3        4       5        6         7     8    9
```

**Bracketed items [HX] and [TIME] are OPTIONAL**

#### 1.2.1 Message Number (NR)
- Selected by originating station
- Digits only, no letters or leading zeros
- Usually begun with 1 at start of year/month
- For SERVICE messages: precede with "SVC " (space after)

#### 1.2.2 Precedence (PREC)
Message priority handling order:
- **EMERGENCY** (spelled out): Life/death urgency, absence of commercial facilities
- **PRIORITY (P)**: Time-critical, official messages, press, death/injury notices
- **WELFARE (W)**: Health/welfare inquiries or advisories from disaster areas
- **ROUTINE (R)**: Normal traffic, handled after higher precedences

**Exercise Messages**: Precede with "TEST" (TEST R, TEST P, TEST EMERGENCY)

#### 1.2.3 Handling Instructions [HX] - OPTIONAL
Used by originator to specify special handling:
- **HXA[number]**: Collect landline delivery authorized within [number] miles
- **HXB[number]**: Cancel if not delivered within [number] hours
- **HXC**: Report delivery date/time to originating station
- **HXD**: Report routing and delivery details to originating station
- **HXE**: Get reply from addressee, originate message back
- **HXF[date]**: Hold delivery until [date]
- **HXG**: No toll calls required; cancel and service if expense involved

#### 1.2.4 Station of Origin (STN-ORIG)
- Call sign of amateur station creating the message
- Only punctuation allowed: slash after call + number (W1AW/3)
- Service messages return to this station

#### 1.2.5 Check (CK)
Number of word groups in TEXT:
- **Standard**: Just the number (12)
- **With ARL**: "ARL" precedes number (ARL 12) when ARRL Numbered Radiograms used
- **Corrections**: Original preserved with amendment (13/12)

#### 1.2.6 Place of Origin
- Location of person for whom message created (not station location)
- City and standard 2-letter state abbreviation
- No punctuation symbols allowed

#### 1.2.7 Time Filed [TIME] - OPTIONAL
- Only when filing time is important
- 24-hour format + "Z" (UTC) or time zone (2215EDT)
- "L" acceptable for local time (2215L)

#### 1.2.8-1.2.9 Month/Day Filed (MON/DAY)
- **Month**: 3-letter abbreviation (JAN, FEB, MAR, etc.)
- **Day**: Figures only, no leading zeros
- Must agree with time zone if TIME used

## 1.3 ADDRESS PART

Complete addressee information for delivery:

```
DONALD R SMITH              (Full name as in telephone directory)
164 EAST SIXTH AVE         (Street address - spell out directions)
RIVER CITY MD 00789        (City, 2-letter state, ZIP)
301 555 3470              (Area code, exchange, number - no punctuation)
OP NOTE WORKDAY ONLY      (Optional delivery instructions)
```

### Special Addressing Cases
- **Children**: Include parent's name
- **International**: Check third-party traffic agreements
- **Institutions**: Include facility name and room/unit
- **Extended ZIP**: Use DASH (21117 DASH 2345)

## 1.4 TEXT PART

The actual message content framed by "BREAK" (voice) or <BT> (CW):

### Punctuation Rules
- **X**: Period substitute (not last group)
- **R**: Decimal point in numbers (146R670)
- **DOT**: Email address periods
- **DASH**: Special separators
- **Other**: Spelled out (QUERY, COMMA, EXCLAMATION)

### Word Group Counting
ANY GROUP of consecutive characters with spaces before/after = ONE GROUP
- Examples: "X 73" = 2 groups, "145R67" = 1 group, "555 5678" = 2 groups

### ARRL Numbered Radiograms
- Always preceded by "ARL" (ARL SIXTY TWO)
- Spell out numbers completely
- Fill in blanks as needed
- Requires "ARL" in check count

## 1.5 SIGNATURE PART

Name of person for whom message created:

```
DIANA                                    (Name)
N1ABC ATSIGN DOMAIN DOT NET             (Optional contact info)
OP NOTE REPLY VIA EMAIL ADDRESS ABOVE   (Optional handling note)
```

### Signature Rules
- Same punctuation rules as TEXT
- May include multiple lines (address, phone, etc.)
- Amateur call signs follow name on same line
- Salutations ("love", "regards") go in TEXT, not signature

## 1.6 MESSAGE RECORDS

Handling stations must maintain records in blocks 5-9:
- **Block 5**: Station received from, net, date/time
- **Block 6**: Station sent to, net, date/time  
- **Block 7**: Origination information (name, address, phone)
- **Block 8**: Delivery information and corrections
- **Block 9**: Station identification for mailing

## 1.7 ORIGINATING MESSAGES

### Requirements
- Only with permission from the originating party
- Complete addressee information
- 25-word limit explanation
- Proper precedence assignment
- Legal content compliance

### Legal Considerations
- No business traffic
- No encrypted/coded content
- Check international third-party agreements
- FCC compliance responsibility on licensee

## 1.8 SERVICE MESSAGES

When messages cannot be delivered:
1. **Relay** it, or
2. **Deliver** it, or  
3. **Service** it back to originating station

### ARL SIXTY SEVEN Format
"Your message number [number] undeliverable because of [reason]. Please advise."

### Service Message Rules
- Preceded by "SVC" and space (optional current practice)
- Same precedence as original message
- Addressed to station of origin
- Include specific reason for non-delivery

## 1.9 ARRL NUMBERED RADIOGRAMS

Pre-coded messages for common situations:

### Group One - Emergency Use
- **ARL ONE**: Everyone safe here. Please don't worry
- **ARL SEVEN**: Please reply by Amateur Radio through amateur delivering this message
- **ARL EIGHT**: Need additional mobile/portable equipment for immediate emergency use

### Group Two - Routine Messages  
- **ARL FORTY SIX**: Greetings on your birthday and best wishes for many more to come
- **ARL FIFTY**: Greetings by Amateur Radio
- **ARL SIXTY ONE**: Wishing you a very Merry Christmas and a Happy New Year

*[Complete list available in full document appendix]*

## 1.10 HANDLING INSTRUCTIONS REFERENCE

**Complete HX codes and definitions:**
- Multiple codes may be combined (HXAC or HXA50 HXC)
- Compliance is mandatory
- Reports considered service messages

*Document Reference: ARRL FSD-218 2/91*