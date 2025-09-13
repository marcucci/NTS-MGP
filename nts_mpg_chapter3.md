# CHAPTER 3 - SENDING MESSAGES ON CW

<!-- TOC START -->
- [3.1 INTRODUCTION](#31-introduction)
- [3.2 CW TRANSMISSION TOOLS](#32-cw-transmission-tools)
- [3.3 CW MESSAGE EXCHANGE](#33-cw-message-exchange)
- [3.4 QSK OPERATIONS](#34-qsk-operations)
- [3.5 BOOKING MESSAGES ON CW](#35-booking-messages-on-cw)
- [3.6 MULTIPLE MESSAGES](#36-multiple-messages)
- [3.7 STATION OPERATIONS](#37-station-operations)
- [3.8 ERROR CORRECTION](#38-error-correction)
- [3.9 PROSIGN AND ABBREVIATION REFERENCE](#39-prosign-and-abbreviation-reference)
- [3.10 SPECIAL CW PROCEDURES](#310-special-cw-procedures)
- [3.11 EMERGENCY PROCEDURES](#311-emergency-procedures)
- [3.12 QUALITY CONTROL](#312-quality-control)
<!-- TOC END -->

<!-- TOC ANCHOR --><a name="31-introduction"></a>
## 3.1 INTRODUCTION

Transmission of formal written traffic by CW presents unique advantages and techniques different from voice operations. This chapter presents CW message exchanging protocols and two-station CW exchange procedures.

<!-- TOC ANCHOR --><a name="32-cw-transmission-tools"></a>
## 3.2 CW TRANSMISSION TOOLS

### 3.2.1 Sending Requirements
- **Clean keying**: Proper timing and spacing
- **Consistent speed**: Match receiving station capability
- **Break-in capability**: QSK preferred for efficiency

### 3.2.2 Break-in Operations (QSK)
- Enables instant interruption capability
- Allows real-time error correction
- Improves efficiency and accuracy
- Essential for professional traffic handling

### 3.2.3 Prosigns and Abbreviations

#### Essential CW Prosigns
```
<BT>    - Break (separates message parts)
<AR>    - End of message  
<SK>    - End of work/contact
<KN>    - Go ahead (specific station only)
<K>     - Go ahead (any station may respond)
<AS>    - Wait/Stand by
<BK>    - Break (interruption)
```

#### Punctuation Prosigns
```
<AAA>   - Period (.) - Not used in radiograms
<DN>    - Slash (/) - When sent as separate character
<SN>    - Understood/Roger
<IMI>   - Repeat/Say again  
<NIL>   - Nothing/No traffic
<C>     - Correct/Yes
<N>     - Wrong/No
```

### 3.2.4 Q-Signals for Traffic Work
```
QRV     - Ready to copy
QRU     - No traffic/nothing for you
QTC     - Have traffic for you
QSL     - Acknowledge/confirm
QSM     - Repeat last message sent  
QSZ     - Send each word/group twice
QTB     - First initials of text
QSK     - Break in on my transmission
QNI     - Check into net
QNV     - Establish contact and move off frequency
QNB     - Act as relay between ___ and ___
QNC     - All stations copy
```

<!-- TOC ANCHOR --><a name="33-cw-message-exchange"></a>
## 3.3 CW MESSAGE EXCHANGE

### 3.3.1 Establishing Contact

#### Ready to Copy Signals
```
QRV     - Ready to copy (general)
QRV UR  - Ready to copy your traffic
QSZ 5   - Send each group 5 words at a time (optional)
```

#### Traffic Announcement
```
QTC 3   - Have 3 messages for you
QTC 1P 2R - Have 1 Priority, 2 Routine messages
SVC QTC 1 - Have 1 service message
```

### 3.3.2 Message Transmission Format

#### Basic CW Message Structure
```
QTC [count] DE [your call]
[Message number] [Prec] [HX] [Stn Orig] [Check] [Place] [Time] [Mon] [Day]
[Addressee line 1]
[Address line 2] 
[City/State/ZIP]
[Telephone]
[OP NOTE if any]
<BT>
[Text groups]
<BT>
[Signature]
[OP NOTE if any]
<AR>
```

#### Example CW Message Transmission
```
QTC 1 DE W2ABC
1 R HXE W1AW 12 NEWINGTON CT 1830Z JUL 1
DONALD R SMITH
164 EAST SIXTH AVE
RIVER CITY MD 00789
301 555 3470
<BT>
THANKS FOR MESSAGE X HOPE TO SEE YOU AT HAMFEST X 73
<BT>
DIANA
<AR>
```

### 3.3.3 Receiving Procedures

#### Copy Confirmation
```
<SN>    - Roger/understood (after each part)
QSL     - Message received OK
CFM     - Confirm/verify
```

#### Fill Requests
```
WA [group]  - Word after [group]  
WB [group]  - Word before [group]
AB [group]  - All before [group]
AA [group]  - All after [group]
RPT         - Repeat
AGN         - Again
```

### 3.3.4 Check Verification

#### Standard Check Process
```
RX: CK?          (What is check?)
TX: CK 12        (Check is 12)
RX: QTB?         (First initials?)
TX: QTB T F M    (Thanks For Message)
RX: QSL          (Confirmed)
```

#### Check Discrepancies
```
RX: IMI CK       (Repeat check)
TX: CK 12        (Check is 12)
RX: I HV 13      (I have 13)
TX: ?            (Question - check again)
RX: QTB?         (Send first initials)
TX: QTB T F M    (Thanks For Message)  
RX: QSL CK 12    (Confirmed check 12)
```

<!-- TOC ANCHOR --><a name="34-qsk-operations"></a>
## 3.4 QSK OPERATIONS

### 3.4.1 QSK Advantages
- Immediate interruption capability
- Real-time error correction
- Higher efficiency
- Better accuracy

### 3.4.2 QSK Techniques
```
TX: THANKS FOR MESSAGE X HO   ?
RX: <BK>                     (Break in)
TX: ?                        (Ready for correction)
RX: WA MESSAGE               (Word after MESSAGE)
TX: HOPE                     (Word after MESSAGE is HOPE)
RX: <SN>                     (Roger, continue)
TX: TO SEE YOU AT HAMFEST X 73
```

### 3.4.3 Non-QSK Operations
When QSK not available:
- Send in shorter segments
- Pause frequently for breaks
- Use "?" to invite corrections
- Wait for acknowledgment before continuing

<!-- TOC ANCHOR --><a name="35-booking-messages-on-cw"></a>
## 3.5 BOOKING MESSAGES ON CW

### 3.5.1 Book Announcement
```
QTC BOOK 3 DE W2ABC          (Book of 3 messages)
FIXED PBL AND TXT TO 1 STN   (Fixed preamble and text)
```

### 3.5.2 Book Message Format
```
QTC BOOK 3 DE W2ABC
FIXED PBL AND TXT TO 1 STN
5 R W2ABC 8 BALTIMORE MD JUL 15    (Preamble)
JOHN SMITH                          (First address)  
123 MAIN ST
BALTIMORE MD 21201
410 555 1234
<BT>
HAPPY BIRTHDAY X BEST WISHES X 73   (Fixed text)
<BT>
MARY                               (Fixed signature)
<AR>

BK 2                               (Book message 2)
ROBERT JONES                       (Address only)
456 ELM ST  
BALTIMORE MD 21202
410 555 5678
<AR>

BK 3                               (Book message 3)
SUSAN BROWN
789 OAK AVE
BALTIMORE MD 21203  
410 555 9012
<AR>

END BOOK                           (End of book)
```

<!-- TOC ANCHOR --><a name="36-multiple-messages"></a>
## 3.6 MULTIPLE MESSAGES

### 3.6.1 Message Sequence
```
QTC 4 DE W2ABC               (4 messages total)
QTC 1P 3R                    (1 Priority, 3 Routine)
```

Send in precedence order:
1. Priority messages first
2. Routine messages after
3. Announce count remaining

### 3.6.2 Progress Tracking
```
[After first message]: MORE 3    (3 more messages)
[After second message]: MORE 2    (2 more messages)
[After third message]: MORE 1     (1 more message)
[After last message]: NO MORE     (All complete)
```

<!-- TOC ANCHOR --><a name="37-station-operations"></a>
## 3.7 STATION OPERATIONS

### 3.7.1 On Net Frequency
- Brief exchanges as directed by NCS
- Acknowledge assignments with call signs
- Return to net when complete

### 3.7.2 Off Net Operations

#### Establishing Contact
```
W2XYZ DE N1ABC QTC 2 K        (Calling with 2 messages)
N1ABC DE W2XYZ QRV K          (Ready to copy)
W2XYZ DE N1ABC QTC 1P 1R K    (1 Priority, 1 Routine)
```

#### Frequency Changes
```
N1ABC DE W2XYZ QSY 14085 K    (Move to 14085)
W2XYZ DE N1ABC QSY 14085 K    (Confirm frequency change)
```

### 3.7.3 Returning to Net
```
[Net frequency]
NCS DE N1ABC QRU              (Returning, no traffic)
or
NCS DE N1ABC QTC 1            (Returning, 1 message for reassignment)
```

<!-- TOC ANCHOR --><a name="38-error-correction"></a>
## 3.8 ERROR CORRECTION

### 3.8.1 Immediate Correction
```
TX: THANKS FOR MESSAG <BK>     (Error in transmission)
TX: E <AR>                     (Correction)
RX: <SN>                       (Roger)
TX: X HOPE TO SEE YOU...       (Continue)
```

### 3.8.2 Fill Procedures
```
RX: WA HAMFEST                 (Word after HAMFEST)
TX: X                          (X)
RX: <SN>                       (Roger)

RX: AA HOPE                    (All after HOPE)  
TX: TO SEE YOU AT HAMFEST X 73 (All after HOPE)
RX: QSL                        (Confirmed)
```

### 3.8.3 Check Verification
```
RX: QTB                        (First initials)
TX: T F M                      (Thanks For Message)
RX: QSL CK 12                  (Confirmed check 12)
```

<!-- TOC ANCHOR --><a name="39-prosign-and-abbreviation-reference"></a>
## 3.9 PROSIGN AND ABBREVIATION REFERENCE

### 3.9.1 Traffic Handling Prosigns
```
<BT>    Break (message part separator)
<AR>    End of message
<SK>    End of contact
<KN>    Go ahead (specific station)
<K>     Go ahead (any station)
<BK>    Break in
<AS>    Wait/stand by
```

### 3.9.2 Common Abbreviations
```
AGN     Again
CFM     Confirm
CK      Check  
DE      From/This is
HV      Have
IMI     Repeat
NIL     Nothing
PBL     Preamble
RPT     Repeat
SIG     Signature
TXT     Text
UR      Your/You're
WA      Word after
WB      Word before
```

### 3.9.3 Net Q-Signals
```
QNI     Check into net
QNV     Establish contact, move off frequency
QNB     Act as relay
QNC     All stations copy
QND     Net is directed
QNF     Net is free
QNG     Take over as net control
QNH     Your net frequency is
QNO     Change to another frequency
QNP     Unable to copy you
QNQ     Move frequency and wait
QNS     Following stations are excused
QNT     I request permission to leave net
QNU     Net has traffic for you
QNX     You are excused from net
QNY     Shift to another frequency
QNZ     Zero beat your signal with mine
```

<!-- TOC ANCHOR --><a name="310-special-cw-procedures"></a>
## 3.10 SPECIAL CW PROCEDURES

### 3.10.1 Mixed Groups
Groups containing letters and numbers:
```
146R52   - Send as: 146R52 (no special indication needed)
N2ABC    - Send as: N2ABC (call signs are obvious)
34TH     - Send as: 34TH (mixed group)
```

### 3.10.2 Email Addresses  
```
W3ABC ATSIGN DOMAIN DOT COM
(Sent exactly as written - no @ symbol used)
```

### 3.10.3 Numbered Radiograms
```
ARL FORTY SIX    (Always spell out numbers)
ARL SIXTY TWO CHRISTMAS  (With filled blank)
```

<!-- TOC ANCHOR --><a name="311-emergency-procedures"></a>
## 3.11 EMERGENCY PROCEDURES

### 3.11.1 Emergency Break-in
```
<BK> <BK> <BK> EMERGENCY <BK> <BK> <BK>
```

### 3.11.2 Emergency Priority
- Emergency traffic takes absolute priority
- All other traffic suspended
- Resume only when emergency traffic cleared

### 3.11.3 Emergency Acknowledgment
```
STA EMERGENCY DE [call] QRV    (Emergency station ready)
```

<!-- TOC ANCHOR --><a name="312-quality-control"></a>
## 3.12 QUALITY CONTROL

### 3.12.1 Accuracy Standards
- Perfect copy required
- All fills must be resolved
- Check verification mandatory
- Clean, readable handwriting essential

### 3.12.2 Speed Considerations
- Match receiving station capability
- Accuracy more important than speed
- Allow time for proper copying
- Use QSZ if receiving station requests slower speed

### 3.12.3 Professional Standards
- Maintain consistent keying
- Use proper prosigns and procedures
- Acknowledge all transmissions appropriately
- Keep transmissions concise and accurate

This chapter establishes CW as a precise, efficient mode for traffic handling, with procedures that ensure accurate message transmission while maintaining professional operating standards.