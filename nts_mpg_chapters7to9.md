# CHAPTERS 7-9 - REPORTING, DELIVERY, AND TACTICAL OPERATIONS

<!-- TOC START -->
- [CHAPTER 7 - STATION ACTIVITY REPORTING (SAR/PSHR)](#chapter-7---station-activity-reporting-sarpshr)
   * [7.1 MEMBERSHIP IN THE NTS](#71-membership-in-the-nts)
   * [7.2 STATION ACTIVITY REPORT (SAR) - TRAFFIC](#72-station-activity-report-sar---traffic)
   * [7.3 PUBLIC SERVICE HONOR ROLL (PSHR)](#73-public-service-honor-roll-pshr)
- [CHAPTER 8 - DELIVERING, SERVICING, ORIGINATING](#chapter-8---delivering-servicing-originating)
   * [8.1 DELIVERING MESSAGES](#81-delivering-messages)
   * [8.2 SERVICE MESSAGES](#82-service-messages)
   * [8.3 ORIGINATING MESSAGES](#83-originating-messages)
   * [8.4 DISASTER COMMUNICATIONS TRAFFIC](#84-disaster-communications-traffic)
- [CHAPTER 9 - TACTICAL NETS, PUBLIC SERVICE EVENTS](#chapter-9---tactical-nets-public-service-events)
   * [9.1 TACTICAL NET OPERATIONS](#91-tactical-net-operations)
   * [9.2 PUBLIC SERVICE EVENT PROCEDURES](#92-public-service-event-procedures)
   * [9.3 TACTICAL COMMUNICATION PROCEDURES](#93-tactical-communication-procedures)
   * [9.4 SPECIAL CONSIDERATIONS](#94-special-considerations)
   * [9.5 WRITTEN vs VERBAL TRAFFIC](#95-written-vs-verbal-traffic)
   * [9.6 PLANNING AND PREPARATION](#96-planning-and-preparation)
   * [9.7 INTEGRATION WITH FORMAL TRAFFIC SYSTEMS](#97-integration-with-formal-traffic-systems)
<!-- TOC END -->

<!-- TOC ANCHOR --><a name="chapter-7---station-activity-reporting-sarpshr"></a>
## CHAPTER 7 - STATION ACTIVITY REPORTING (SAR/PSHR)

<!-- TOC ANCHOR --><a name="71-membership-in-the-nts"></a>
### 7.1 MEMBERSHIP IN THE NTS

Participation in the National Traffic System is voluntary and open to all licensed amateur radio operators. Regular participation and reporting helps maintain system statistics and demonstrates amateur radio's public service value.

<!-- TOC ANCHOR --><a name="72-station-activity-report-sar---traffic"></a>
### 7.2 STATION ACTIVITY REPORT (SAR) - TRAFFIC

#### 7.2.1 Categories of Activity
Monthly reporting uses four categories:

- **ORIG** (Originated): Messages created for others and introduced into the amateur system
- **RCVD** (Received): Messages accepted from other amateur stations  
- **SENT** (Sent): Messages transmitted to other amateur stations
- **DLVD** (Delivered): Messages delivered to addressees outside the amateur system

#### 7.2.2 Counting Guidelines
- Count each message only once in each category
- Messages transferred between modes count as RCVD/SENT
- Service messages count in all applicable categories
- Digital messages count equally with voice/CW messages

#### 7.2.3 SAR Message Format
```
[Number] R [Your Call] [Count] [Your City ST] [Month] [Day]
[STM Call and Name]
[STM Address]
[STM City, State, ZIP]
[STM Phone]
BT
SAR [Month] [Your Call] ORIG [#] RCVD [#] SENT [#] DLVD [#]
BT
[Your Name]
```

Example:
```
15 R W1ABC 12 BALTIMORE MD JUN 30
W3XYZ JOHN SMITH STM
456 RADIO ST
BALTIMORE MD 21201
410 555 7890
BT
SAR JUN W1ABC ORIG 5 RCVD 23 SENT 25 DLVD 8
BT
MARY JONES
```

<!-- TOC ANCHOR --><a name="73-public-service-honor-roll-pshr"></a>
### 7.3 PUBLIC SERVICE HONOR ROLL (PSHR)

#### 7.3.1 PSHR Categories
Recognition for significant public service contributions:

- **A** (ARRL): 70+ hours per month in ARRL activities
- **E** (Emergency): 70+ hours in emergency communications  
- **T** (Training): 70+ hours in training activities
- **B** (Both): Qualifies for both A and E categories

#### 7.3.2 PSHR Reporting
Combined with SAR in single message:
```
SAR JUN W1ABC ORIG 5 RCVD 23 SENT 25 DLVD 8 PSHR 85A
```

#### 7.3.3 PSHR Requirements (ARRL Reference)
- **Accurate records**: Detailed time logs required
- **Verification**: Section Traffic Manager verification
- **Monthly reporting**: Consistent reporting to maintain status
- **Activity categories**: Must meet specific criteria for each category

---

<!-- TOC ANCHOR --><a name="chapter-8---delivering-servicing-originating"></a>
## CHAPTER 8 - DELIVERING, SERVICING, ORIGINATING

<!-- TOC ANCHOR --><a name="81-delivering-messages"></a>
### 8.1 DELIVERING MESSAGES

#### 8.1.1 Finding Addressees
- **Telephone directories**: Primary resource for current information
- **Internet searches**: Verify current addresses and phone numbers
- **Directory assistance**: When other methods fail
- **Previous delivery records**: Use updated information from past deliveries

#### 8.1.2 Delivery Methods

**Telephone Delivery (Preferred)**
```
"Hello, this is [Your name], amateur radio operator [Your call]. 
I have a message for [Addressee name] sent by amateur radio. 
May I deliver it to you?"

[If confirmed as correct person:]
"The message is from [Signature] in [Place of origin], 
dated [Date]. The message reads: [Text content]. 
That completes the message. This is a free public service 
provided by amateur radio operators."
```

**Mail Delivery**  
When telephone delivery not possible:
- Use official ARRL message forms
- Include station identification in Block 9
- Mail to complete address from message
- Keep delivery records

#### 8.1.3 Delivery Confirmation
For HXC handling instruction:
```
SVC [Number] R [Your call] [Check] [Your city] [Date]
[Originating station call and address]
BT  
ARL SIXTY SEVEN [Original msg #] [Addressee name] 
DELIVERED [Date] [Time] BY TELEPHONE
BT
[Your name]
```

<!-- TOC ANCHOR --><a name="82-service-messages"></a>
### 8.2 SERVICE MESSAGES

#### 8.2.1 When to Send Service Messages
Send service messages when:
- Message cannot be delivered
- Handling instructions cannot be followed
- Significant delays occur
- Delivery confirmation requested (HXC)
- Reply requested and obtained (HXE)

#### 8.2.2 ARL SIXTY SEVEN Format
"Your message number [____] undeliverable because of [____]. Please advise."

Example undeliverable reasons:
- NO SUCH ADDRESS
- PHONE DISCONNECTED  
- MOVED NO FORWARDING ADDRESS
- REFUSED DELIVERY
- DECEASED

#### 8.2.3 Service Message Procedure
```
[Your msg #] R [Your call] [Check] [Your city] [Date]
[Original station of origin address]
BT
ARL SIXTY SEVEN [Original msg #] [Addressee last name] 
[Reason undeliverable] X [Additional details if helpful] X 73
BT  
[Your name]
```

<!-- TOC ANCHOR --><a name="83-originating-messages"></a>
### 8.3 ORIGINATING MESSAGES

#### 8.3.1 Taking Messages from the Public
- **Permission required**: Never originate without explicit permission
- **Complete information**: Get full originator and addressee details
- **Legal content**: Ensure compliance with FCC regulations
- **25-word limit**: Explain text length restrictions
- **No guarantee**: Explain that delivery cannot be guaranteed

#### 8.3.2 Message Legality Requirements
- **No business traffic**: Commercial communications prohibited
- **No encryption**: All content must be in plain language
- **Third party**: Check international third-party agreements
- **Public service**: Must serve a public communications need

#### 8.3.3 Helping with Text Composition
- Suggest ARRL Numbered Radiograms when appropriate
- Help condense message to essential information
- Explain punctuation limitations and substitutions
- Assist with proper addressing format

<!-- TOC ANCHOR --><a name="84-disaster-communications-traffic"></a>
### 8.4 DISASTER COMMUNICATIONS TRAFFIC

#### 8.4.1 ARES Operations
- Coordinate with served agencies
- Handle both formal radiograms and tactical traffic
- Maintain integration with NTS for long-haul routing
- Document all activities for after-action reports

#### 8.4.2 RACES Operations  
- Activate under government authority
- Handle official government communications
- Coordinate with ARES when appropriate
- Follow specific activation procedures

#### 8.4.3 Welfare Traffic Priority
Health and welfare messages during disasters:
- **Welfare precedence**: Handle after emergency and priority
- **DWI coordination**: Work with Red Cross Disaster Welfare Inquiries
- **Family reunification**: Facilitate family communications
- **Volume handling**: Prepare for large message loads

---

<!-- TOC ANCHOR --><a name="chapter-9---tactical-nets-public-service-events"></a>
## CHAPTER 9 - TACTICAL NETS, PUBLIC SERVICE EVENTS

<!-- TOC ANCHOR --><a name="91-tactical-net-operations"></a>
### 9.1 TACTICAL NET OPERATIONS

Tactical nets handle operational communications during public service events, differing from formal traffic nets in format and procedures while maintaining professional standards.

<!-- TOC ANCHOR --><a name="92-public-service-event-procedures"></a>
### 9.2 PUBLIC SERVICE EVENT PROCEDURES

#### 9.2.1 Event Station Assignments
Typical assignments:
- **Net Control**: Overall coordination and communication management
- **Start/Finish**: Critical timing and safety communications  
- **Aid Stations**: Medical and support communications
- **Course Marshals**: Safety and participant monitoring
- **Mobile Units**: Roving coverage and emergency response
- **EOC/Command**: Coordination with event management

#### 9.2.2 Directed Net Procedures
- **Net Control directs all communications**: Stations transmit only when called
- **Emergency priority**: Safety traffic takes absolute precedence
- **Efficiency**: Keep transmissions brief and clear
- **Coordination**: Maintain contact with event management

<!-- TOC ANCHOR --><a name="93-tactical-communication-procedures"></a>
### 9.3 TACTICAL COMMUNICATION PROCEDURES

#### 9.3.1 Check-in Procedures
```
Voice: "Net Control, this is [Tactical ID] at [Location], checking in"
Example: "Net Control, this is Aid Station 3, checking in"
```

#### 9.3.2 Traffic Handling
**Operational Communications** (Not formal messages):
```
"Net Control, Aid Station 3"
"Aid Station 3, Net Control, go ahead"
"Net Control, Aid Station 3, request ambulance at mile marker 15 for dehydrated runner, non-emergency"
"Aid Station 3, Net Control, copy ambulance request mile 15, dehydrated runner, dispatching EMS"
```

**Formal Message Traffic**:
Follow standard NTS procedures when handling written messages requiring delivery outside the amateur system.

#### 9.3.3 Emergency Procedures
```
"Break Break Break, Emergency Traffic, Emergency Traffic"
[Emergency station]: "[Tactical ID] Emergency"
Net Control: "[Tactical ID], Net Control, go ahead with your emergency"
```

<!-- TOC ANCHOR --><a name="94-special-considerations"></a>
### 9.4 SPECIAL CONSIDERATIONS

#### 9.4.1 Identification Procedures
- **Tactical IDs**: Use functional identifiers (Aid Station 1, Start Line, etc.)
- **FCC ID requirements**: Include amateur call sign per FCC regulations
- **Coordination**: Ensure event management understands amateur procedures

#### 9.4.2 Repeater Operations
- **Repeater delays**: Allow time for repeater switching
- **Coverage planning**: Ensure adequate signal coverage
- **Backup frequencies**: Have alternate channels available
- **Interference**: Coordinate with other users

#### 9.4.3 Transmission Speed and Clarity
- **Speak slowly**: Many listeners may not be amateur operators  
- **Clear pronunciation**: Use proper voice procedures
- **Standard phonetics**: When spelling is required
- **Brevity**: Keep transmissions concise but complete

<!-- TOC ANCHOR --><a name="95-written-vs-verbal-traffic"></a>
### 9.5 WRITTEN vs VERBAL TRAFFIC

#### 9.5.1 Verbal Communications
- **Tactical coordination**: Real-time operational communications
- **Status reports**: Routine position and status updates  
- **Resource coordination**: Equipment and personnel management
- **Safety communications**: Immediate safety-related information

#### 9.5.2 Written Traffic
Formal messages requiring:
- **Delivery outside amateur system**: Messages for non-amateurs
- **Official documentation**: Formal reports and requests
- **Legal requirements**: Messages requiring written record
- **Accurate transmission**: Critical information requiring exact wording

<!-- TOC ANCHOR --><a name="96-planning-and-preparation"></a>
### 9.6 PLANNING AND PREPARATION

#### 9.6.1 Pre-Event Coordination
- **Frequency coordination**: Avoid conflicts with other operations
- **Equipment testing**: Verify all communications equipment  
- **Personnel briefing**: Train operators on event-specific procedures
- **Emergency procedures**: Review safety and emergency protocols

#### 9.6.2 Event Execution Checklist
- **Net control setup**: Establish communications hub
- **Station deployment**: Position operators at assigned locations
- **Communication check**: Verify all stations operational
- **Coordination**: Establish contact with event management
- **Documentation**: Maintain logs and records

#### 9.6.3 Post-Event Activities
- **Equipment recovery**: Collect and inventory equipment
- **After-action review**: Evaluate performance and lessons learned
- **Documentation**: Complete reports and submit statistics
- **Recognition**: Thank participants and served agencies

<!-- TOC ANCHOR --><a name="97-integration-with-formal-traffic-systems"></a>
### 9.7 INTEGRATION WITH FORMAL TRAFFIC SYSTEMS

#### 9.7.1 NTS Coordination
- Formal messages from tactical nets may enter NTS for delivery
- Tactical nets may provide local outlets for NTS traffic
- Emergency traffic may require both tactical and formal handling
- Maintain contact with local NTS nets when appropriate

#### 9.7.2 Dual Operations
Some operators may:
- Handle tactical communications during events
- Participate in formal traffic nets
- Bridge between systems as needed
- Maintain proficiency in both procedures

This comprehensive coverage of Chapters 7-9 completes the essential operational procedures for traffic handling, from statistical reporting through message delivery to tactical public service operations, ensuring amateur radio continues to serve the public professionally and effectively.