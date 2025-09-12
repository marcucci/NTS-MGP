# CHAPTER 3 - SENDING MESSAGES ON CW

<!-- TOC START -->
- [3.1 INTRODUCTION](#31-introduction)
- [3.2 CW TRANSMISSION TOOLS](#32-cw-transmission-tools)
- [3.3 CW MESSAGE EXCHANGE](#33-cw-message-exchange)
- [3.4 QSK OPERATIONS](#34-qsk-operations)
- [3.5 BOOKING MESSAGES ON CW](#35-booking-messages-on-cw)
- [3.6 MULTIPLE MESSAGES](#36-multiple-messages)
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
[After first message]: MORE 3    (3 more messages