# CHAPTER 4 - NET OPERATIONS

<!-- TOC START -->
- [4.1 INTRODUCTION](#41-introduction)
- [4.2 TYPES OF NETS](#42-types-of-nets)
- [4.3 NET ORGANIZATION](#43-net-organization)
- [4.4 NET CONTROL PROCEDURES](#44-net-control-procedures)
- [4.5 TRAFFIC ASSIGNMENT](#45-traffic-assignment)
- [4.6 TRAFFIC DISPATCHING](#46-traffic-dispatching)
- [4.7 NET SYNTAX AND CONVENTIONS](#47-net-syntax-and-conventions)
- [4.8 TRAFFIC CATEGORIES](#48-traffic-categories)
- [4.9 STATION OPERATIONS ON NETS](#49-station-operations-on-nets)
- [4.10 NET CONTROL RESPONSIBILITIES](#410-net-control-responsibilities)
- [4.11 SPECIAL SITUATIONS](#411-special-situations)
- [4.12 NET COORDINATION](#412-net-coordination)
<!-- TOC END -->

<!-- TOC ANCHOR --><a name="41-introduction"></a>
## 4.1 INTRODUCTION

Net operations manage the routing of messages beyond two-station exchanges. Scheduled directed traffic nets are the primary means for establishing liaison connections, listing message traffic, assigning outlets, dispatching traffic, and providing administrative communications.

<!-- TOC ANCHOR --><a name="42-types-of-nets"></a>
## 4.2 TYPES OF NETS

### 4.2.1 NTS Daily Traffic Nets
Structured hierarchy for systematic message routing:
- **Local Nets**: City/county level traffic collection
- **Section Nets**: State/section level traffic routing  
- **Region Nets**: Multi-state regional traffic routing
- **Area Nets**: Transcontinental traffic routing
- **Transcontinental Corps (TCC)**: Final relay between areas

### 4.2.2 Welfare Nets
- Handle incoming/outgoing public traffic
- Often activated during disasters
- Focus on health and welfare messages

### 4.2.3 Emergency Nets (ARES/RACES)
- Activated for emergency communications
- May handle both formal and tactical traffic
- Coordinate with served agencies

### 4.2.4 Special Nets
- Holiday greetings nets
- Special events
- Training exercises

<!-- TOC ANCHOR --><a name="43-net-organization"></a>
## 4.3 NET ORGANIZATION

### 4.3.1 Net Manager (NM)
ARRL-appointed position responsible for:
- Net scheduling and frequency coordination
- Recruiting net control stations and liaisons
- Training and mentoring operators
- Submitting monthly net reports

### 4.3.2 Net Control Station (NCS)
Daily operational control:
- Opening and closing the net
- Calling stations and taking check-ins
- Managing traffic assignments and dispatching
- Maintaining net discipline and efficiency

### 4.3.3 Liaison Stations
- Connect different nets in the NTS hierarchy
- Carry traffic between levels (section to region, etc.)
- Have specific time schedules and frequencies
- Essential for NTS traffic flow

### 4.3.4 Traffic Handlers
Regular stations that:
- Check into nets with traffic
- Provide delivery outlets for messages
- Originate traffic from the public
- Maintain NTS operation through participation

<!-- TOC ANCHOR --><a name="44-net-control-procedures"></a>
## 4.4 NET CONTROL PROCEDURES

### 4.4.1 Opening the Net
Standard net preamble includes:
- Net identification and frequency
- Time, date, and NCS call sign  
- Net purpose and scope
- Operating procedures and courtesies
- Initial traffic poll

### 4.4.2 Station Check-ins

#### Liaison Station Calls
```
Voice: "Eastern Area Net liaison, please check in"
CW: "QNI EAN LNK"
```

#### General Station Calls  
```
Voice: "Any station with traffic, please check in"  
CW: "QNI QTC"
```

#### Specific Calls
```
Voice: "W1ABC, please check in"
CW: "W1ABC QNI"
```

### 4.4.3 Traffic Listing
Stations report traffic in standardized format:
```
Voice: "W1ABC, 2 routine for Maryland, 1 priority for Virginia"
CW: "W1ABC QTC 2R MD 1P VA"
```

<!-- TOC ANCHOR --><a name="45-traffic-assignment"></a>
## 4.5 TRAFFIC ASSIGNMENT

### 4.5.1 Assignment Priorities
1. **Liaisons first**: Traffic for other nets via liaison stations
2. **Direct outlets**: Stations in destination areas
3. **Regional outlets**: Stations in nearby areas  
4. **Store and forward**: Digital systems when appropriate

### 4.5.2 Assignment Syntax
```
Voice: "W1ABC, take 2 routine for Maryland from W2DEF"
CW: "W1ABC TK 2R MD DE W2DEF"
```

### 4.5.3 Booking Assignments
```
Voice: "W1ABC, take book of 3 for Maryland from W2DEF"  
CW: "W1ABC TK BK 3 MD DE W2DEF"
```

<!-- TOC ANCHOR --><a name="46-traffic-dispatching"></a>
## 4.6 TRAFFIC DISPATCHING

### 4.6.1 On Net Frequency
For brief exchanges:
```
Voice: "W1ABC and W2DEF, go ahead on net frequency with your traffic"
CW: "W1ABC W2DEF QNV NET"
```

### 4.6.2 Off Net Frequency (Stack)
For longer exchanges:
```  
Voice: "W1ABC and W2DEF, please move off frequency for your traffic"
CW: "W1ABC W2DEF QNV"
```

### 4.6.3 Three-Station Relays
When direct contact not possible:
```
Voice: "W1ABC, W2DEF, W3GHI - W3GHI relay between W1ABC and W2DEF"
CW: "W1ABC W2DEF W3GHI - W3GHI QNB W1ABC W2DEF"
```

<!-- TOC ANCHOR --><a name="47-net-syntax-and-conventions"></a>
## 4.7 NET SYNTAX AND CONVENTIONS

### 4.7.1 Flow Control
- Stations respond only when called
- No tail-ending without permission
- Maintain proper turn-taking protocol

### 4.7.2 Station Identification
- Full call signs on first exchange
- Suffixes acceptable after establishment
- Regular identification per FCC requirements

### 4.7.3 Precedence Handling
- Emergency traffic takes absolute priority
- Priority traffic handled before routine
- Welfare traffic handled after priority

### 4.7.4 Q-Signal Usage (CW Nets)
```
QNU - Net has traffic for you, stand by
QNC - All stations copy  
QND - Net is directed (NCS permission required)
QNF - Net is free (any station may call)
QNI - Check into net
QNV - Establish contact, move off frequency
QNX - You are excused from the net
QRT - Closing station/net
```

<!-- TOC ANCHOR --><a name="48-traffic-categories"></a>
## 4.8 TRAFFIC CATEGORIES

### 4.8.1 Formal Radiograms
- Standard ARRL message format
- Complete preamble, address, text, signature
- Counted in net statistics

### 4.8.2 Service Messages  
- Report delivery status
- Handle undeliverable messages
- Maintain message accountability

### 4.8.3 Administrative Traffic
- Net business and announcements
- Scheduling and coordination messages
- Training and procedural updates

### 4.8.4 Informal Traffic (Announcements)
- General information for net stations
- Not counted as formal messages
- Handled after formal traffic

<!-- TOC ANCHOR --><a name="49-station-operations-on-nets"></a>
## 4.9 STATION OPERATIONS ON NETS

### 4.9.1 Checking In
```
Voice: "Net Control, W1ABC in Baltimore with 2 routine for Virginia"
CW: "NCS DE W1ABC QNI BALTIMORE QTC 2R VA"
```

### 4.9.2 Taking Assignments
```
Voice: "W1ABC takes the traffic for Virginia"
CW: "W1ABC TK VA"
```

### 4.9.3 Handling Multiple Assignments
- Accept only what you can handle
- Consider time constraints
- Request help if needed

### 4.9.4 Returning to Net
Report status when returning:
```
Voice: "Net Control, W1ABC returning - all traffic handled"
CW: "NCS DE W1ABC RTN QRU"
```

<!-- TOC ANCHOR --><a name="410-net-control-responsibilities"></a>
## 4.10 NET CONTROL RESPONSIBILITIES

### 4.10.1 Traffic Management
- Assign traffic efficiently
- Monitor progress of assignments  
- Reassign unhandled traffic
- Maintain accurate traffic count

### 4.10.2 Time Management
- Keep net moving efficiently
- Balance thoroughness with time constraints
- Recognize liaison departure times
- Close net on schedule

### 4.10.3 Station Coordination
- Welcome new stations
- Provide guidance when needed
- Maintain net discipline
- Excuse stations appropriately

### 4.10.4 Record Keeping
- Maintain net control sheet
- Record traffic counts and handling
- Track station participation
- Prepare net reports

<!-- TOC ANCHOR --><a name="411-special-situations"></a>
## 4.11 SPECIAL SITUATIONS

### 4.11.1 Emergency Traffic
- Suspend normal operations
- Handle emergency traffic immediately
- Resume normal operations only when cleared

### 4.11.2 Heavy Traffic Loads
- Extend net time if necessary
- Use auxiliary frequencies
- Prioritize by precedence and destination
- Request additional net control help

### 4.11.3 Missing Liaisons
- Call for volunteers
- Arrange temporary coverage
- Store traffic for later handling
- Notify net management

### 4.11.4 Equipment Problems
- Have backup plans ready
- Use alternate frequencies
- Arrange for relay assistance
- Maintain communications

<!-- TOC ANCHOR --><a name="412-net-coordination"></a>
## 4.12 NET COORDINATION

### 4.12.1 Inter-Net Communication
- Maintain liaison schedules
- Coordinate frequency usage
- Share traffic load information
- Support emergency activations

### 4.12.2 Training and Development
- Mentor new operators
- Practice emergency procedures
- Conduct training exercises
- Improve operating efficiency

### 4.12.3 Quality Control
- Monitor message accuracy
- Ensure proper procedures
- Provide constructive feedback
- Maintain professional standards

This chapter establishes the framework for efficient net operations that form the backbone of the National Traffic System, ensuring reliable message handling through coordinated amateur radio networks.