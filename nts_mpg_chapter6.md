# CHAPTER 6 - NTSD RADIO-EMAIL OPERATIONS

<!-- TOC START -->
- [6.1 NTSD OVERVIEW](#61-ntsd-overview)
- [6.2 WINLINK 2000 SYSTEM](#62-winlink-2000-system)
- [6.3 TARGET STATIONS](#63-target-stations)
- [6.4 ADDRESSING METHODS](#64-addressing-methods)
- [6.5 MESSAGE FORMATTING](#65-message-formatting)
- [6.6 OPERATIONAL PROCEDURES](#66-operational-procedures)
- [6.7 TRAFFIC COUNTING AND REPORTING](#67-traffic-counting-and-reporting)
- [6.8 TECHNICAL CONSIDERATIONS](#68-technical-considerations)
- [6.9 NTSD STANDARD OPERATING PROCEDURES](#69-ntsd-standard-operating-procedures)
- [6.10 SPECIALIZED APPLICATIONS](#610-specialized-applications)
- [6.11 TROUBLESHOOTING PROCEDURES](#611-troubleshooting-procedures)
- [6.12 QUALITY CONTROL](#612-quality-control)
- [6.13 FUTURE DEVELOPMENTS](#613-future-developments)
- [6.14 REFERENCE MATERIALS](#614-reference-materials)
<!-- TOC END -->

<!-- TOC ANCHOR --><a name="61-ntsd-overview"></a>
## 6.1 NTSD OVERVIEW

### 6.1.1 NTS Digital (NTSD) Purpose
The NTSD system provides digital message handling capabilities that complement and integrate with traditional voice and CW nets. It uses modern digital modes and email-style addressing while maintaining compatibility with standard ARRL radiogram format.

### 6.1.2 System Integration
- **Parallel Structure**: Mirrors traditional NTS hierarchy
- **Mode Compatibility**: Messages transferable between digital and manual nets
- **Common Format**: Uses standard ARRL radiogram structure
- **Routing Coordination**: Works with established NTS routing procedures

<!-- TOC ANCHOR --><a name="62-winlink-2000-system"></a>
## 6.2 WINLINK 2000 SYSTEM

### 6.2.1 System Components

#### Clients
- **Airmail**: Popular HF client software
- **Paclink**: VHF/UHF packet client
- **RMS Express**: Winlink Express client
- **Telnet**: Internet gateway access (emergency backup)

#### Gateways (RMS)
- **HF RMS**: HF radio message servers
- **VHF/UHF RMS**: VHF/UHF radio message servers  
- **Pactor, PSK31, WINMOR**: Various digital modes supported

#### Servers
- **Common Message Servers (CMS)**: Central routing and storage
- **Internet Integration**: Seamless email connectivity when available

### 6.2.2 Message Flow
1. **Origination**: Message created at client station
2. **Radio Link**: Transmitted via RF to RMS gateway
3. **Internet Backbone**: Routed through CMS servers
4. **Delivery**: Delivered via radio or internet to destination

<!-- TOC ANCHOR --><a name="63-target-stations"></a>
## 6.3 TARGET STATIONS

### 6.3.1 Section Target Stations
Designated stations for ARES®/NTS/NTSD coordination:
- Handle traffic between digital and manual systems
- Provide gateway services for emergency communications
- Maintain current routing information

### 6.3.2 NTS Target Stations  
Bridge between NTSD and manual net system:
- Monitor both digital and voice/CW nets
- Transfer messages between systems as needed
- Provide backup communications paths

### 6.3.3 NTSD MBO Operations
Mailbox Office (MBO) stations provide:
- **Store and Forward**: Hold messages for later delivery
- **Routing Services**: Automatically route to proper destinations
- **System Integration**: Connect NTSD with manual NTS operations

<!-- TOC ANCHOR --><a name="64-addressing-methods"></a>
## 6.4 ADDRESSING METHODS

### 6.4.1 Standard Email Addressing
For stations with internet email access:
```
To: w1abc@winlink.org
Subject: NTS Traffic
```

### 6.4.2 Radio-Only Addressing
For stations without internet access:
```
To: W1ABC
Subject: //WL2K [Call Sign] 
```

### 6.4.3 Tactical Addressing
For emergency operations:
```  
To: ICS213@COUNTY-EOC
Subject: Resource Request
```

### 6.4.4 NTS Integration Addressing
For messages entering manual NTS:
```
To: [STM call]@[section].NTS.WL2K.ORG
Subject: NTS [destination state/section]
```

<!-- TOC ANCHOR --><a name="65-message-formatting"></a>
## 6.5 MESSAGE FORMATTING

### 6.5.1 Radio-Email with Radiogram
Complete ARRL radiogram in message body:
```
To: w2def@winlink.org
Subject: Radiogram for John Smith

1 R W1ABC 12 NEWINGTON CT JUL 15
JOHN SMITH
123 MAIN ST  
ANYTOWN MD 20123
301 555 1234
BT
HAPPY BIRTHDAY X BEST WISHES X 73
BT  
MARY
```

### 6.5.2 Direct Email Format
For non-NTS traffic:
```
To: john.smith@example.com
Subject: Birthday Wishes

Happy Birthday John! Hope you have a wonderful day.
Best wishes from all of us here.

73,
Mary W1ABC
```

### 6.5.3 Batch File Processing
Multiple radiograms in single transmission:
```
!BATCH!
[Message 1 radiogram]
!BATCH!
[Message 2 radiogram]  
!BATCH!
[Message 3 radiogram]
!EOF!
```

<!-- TOC ANCHOR --><a name="66-operational-procedures"></a>
## 6.6 OPERATIONAL PROCEDURES

### 6.6.1 Normal Operations
- **Full Internet**: All services available
- **Radio-Email**: Gateway services via RF
- **Store and Forward**: MBO operations
- **Manual Integration**: Bridge to voice/CW nets

### 6.6.2 Emergency Operations

#### No Internet at Deployment Site
- Use radio-only addressing
- Rely on RF gateways
- Coordinate with served agencies via radio
- Maintain contact with EOC/ICP

#### Infrastructure Failure
- **"Last Mile" Solutions**: RF links to internet connection points
- **Manual Relay**: Transfer to voice/CW nets
- **Direct RF**: Point-to-point digital communications
- **Backup Systems**: Satellite, cellular, other modes

### 6.6.3 Served Agency Integration

#### ICS-213 Messages
Standard incident command forms via radio-email:
- **Point-to-Point**: Direct transmission between units
- **Manual Relay**: Through voice/CW nets when needed  
- **Radio-Email**: Via Winlink system

#### ARESMAT Integration
ARES Management and Tracking system:
- Standardized forms and procedures
- Integration with ICS structure
- Automated routing and tracking

<!-- TOC ANCHOR --><a name="67-traffic-counting-and-reporting"></a>
## 6.7 TRAFFIC COUNTING AND REPORTING

### 6.7.1 SAR/PSHR Reporting
Digital traffic counts toward Station Activity Reports:
- **Originated**: Messages created for others
- **Received**: Messages accepted from other stations
- **Sent**: Messages transmitted to other stations
- **Delivered**: Messages delivered to addressees

### 6.7.2 Net Traffic Integration
Radio-email traffic may be:
- Listed on manual nets for assignment
- Handled via store-and-forward systems
- Transferred between digital and manual systems
- Counted in combined net statistics

<!-- TOC ANCHOR --><a name="68-technical-considerations"></a>
## 6.8 TECHNICAL CONSIDERATIONS

### 6.8.1 Mode Selection
Choose appropriate digital mode based on:
- **Propagation conditions**: HF vs VHF/UHF
- **Data rate requirements**: Speed vs reliability
- **Equipment availability**: Station capabilities
- **Emergency vs routine**: Urgency considerations

### 6.8.2 Gateway Selection
Select RMS gateways considering:
- **Signal strength**: Reliable RF path
- **Gateway load**: Avoid overloaded systems
- **Geographic location**: Routing efficiency  
- **Service reliability**: Established operations

### 6.8.3 Message Size Considerations
- **Text messages**: Efficient transmission
- **Binary attachments**: Use sparingly, consider RF bandwidth
- **Image files**: Compress when possible for faster transmission
- **Document attachments**: PDF/Word docs increase transmission time

### 6.8.4 Security Considerations
- **No encryption**: Amateur radio prohibition applies
- **Plain text**: All content must be readable
- **Third party**: Follow international third-party traffic rules
- **Privacy**: Respect addressee privacy in forwarding

<!-- TOC ANCHOR --><a name="69-ntsd-standard-operating-procedures"></a>
## 6.9 NTSD STANDARD OPERATING PROCEDURES

### 6.9.1 Digital Station Principles
- **Interoperability**: Maintain compatibility with manual systems
- **Reliability**: Provide redundant communication paths
- **Efficiency**: Use appropriate technology for conditions
- **Training**: Maintain operator proficiency

### 6.9.2 Area Digital Coordination
- **Frequency coordination**: Avoid interference with manual nets
- **Gateway management**: Ensure adequate RMS coverage
- **Training programs**: Develop operator skills
- **Emergency planning**: Prepare for infrastructure failure

### 6.9.3 Integration Procedures
- **Manual net coordination**: Bridge digital and voice/CW operations
- **Traffic transfer**: Move messages between systems as needed
- **Backup communications**: Provide alternate paths when systems fail
- **Quality control**: Maintain accuracy and reliability standards

<!-- TOC ANCHOR --><a name="610-specialized-applications"></a>
## 6.10 SPECIALIZED APPLICATIONS

### 6.10.1 Welfare Traffic
Health and welfare inquiries during disasters:
- **Welfare Email**: Direct email format for non-amateur addressees
- **Welfare Radiograms**: Standard format for amateur handling
- **DWI Integration**: Coordinate with Red Cross Disaster Welfare Inquiries
- **Mass Casualty**: Handle large volumes efficiently

### 6.10.2 Agency Traffic
Official communications for served agencies:
- **ICS Forms**: Standard incident command system documents
- **Resource Requests**: Equipment, personnel, supplies
- **Situation Reports**: Status updates and intelligence
- **Coordination Messages**: Inter-agency communications

### 6.10.3 Training and Exercises
- **SET Integration**: Simulated Emergency Test participation
- **Training Messages**: Practice scenarios and procedures
- **System Testing**: Verify gateway and routing operations
- **Interoperability**: Test integration with manual systems

<!-- TOC ANCHOR --><a name="611-troubleshooting-procedures"></a>
## 6.11 TROUBLESHOOTING PROCEDURES

### 6.11.1 Connection Problems
- **Gateway Selection**: Try alternate RMS stations
- **Frequency Issues**: Check propagation and interference
- **Mode Problems**: Verify software configuration
- **RF Issues**: Check antenna and power settings

### 6.11.2 Routing Problems
- **Address Verification**: Confirm correct addressing format
- **System Status**: Check gateway and server operation
- **Alternative Routes**: Use backup addressing methods
- **Manual Intervention**: Transfer to voice/CW nets if needed

### 6.11.3 Message Delivery Issues
- **Undeliverable Messages**: Generate service messages
- **Delayed Delivery**: Check system queues and routing
- **Format Problems**: Verify proper radiogram structure
- **Integration Issues**: Coordinate with manual net operations

<!-- TOC ANCHOR --><a name="612-quality-control"></a>
## 6.12 QUALITY CONTROL

### 6.12.1 Message Accuracy
- **Format Verification**: Ensure proper ARRL radiogram structure
- **Address Validation**: Confirm deliverable addressing
- **Content Review**: Check for prohibited content
- **Routing Verification**: Ensure proper destination addressing

### 6.12.2 System Performance
- **Delivery Statistics**: Monitor success rates and timing
- **Gateway Performance**: Track RMS reliability and speed
- **Integration Efficiency**: Measure manual/digital coordination
- **Error Rates**: Monitor and correct systemic problems

### 6.12.3 Operator Standards
- **Training Requirements**: Maintain current knowledge
- **Procedure Compliance**: Follow established protocols
- **Professional Standards**: Represent amateur radio appropriately
- **Continuous Improvement**: Update skills and knowledge

<!-- TOC ANCHOR --><a name="613-future-developments"></a>
## 6.13 FUTURE DEVELOPMENTS

### 6.13.1 Technology Evolution
- **New Digital Modes**: Adaptation to improved protocols
- **Internet Integration**: Enhanced gateway services
- **Mobile Applications**: Smartphone and tablet clients
- **Mesh Networks**: Distributed emergency communications

### 6.13.2 Integration Enhancements
- **Automated Routing**: Improved message handling
- **Cross-Mode Compatibility**: Seamless system integration
- **Emergency Activation**: Rapid deployment capabilities
- **Training Systems**: Enhanced operator development

<!-- TOC ANCHOR --><a name="614-reference-materials"></a>
## 6.14 REFERENCE MATERIALS

### 6.14.1 Software Documentation
- **Winlink Express**: Client software manual
- **RMS Gateway**: Setup and operation guide
- **Paclink**: VHF/UHF packet client guide
- **ARESMAT**: Management system documentation

### 6.14.2 Addressing References
- **Target Station Database**: Current routing information
- **Tactical Addressing**: Emergency operations guide
- **International Routing**: Third-party traffic agreements
- **System Status**: Gateway and server status pages

### 6.14.3 Integration Guides
- **Manual Net Coordination**: Voice/CW integration procedures  
- **ICS Integration**: Incident Command System compatibility
- **Agency Coordination**: Served agency communication protocols
- **Emergency Procedures**: Disaster response operations

This chapter establishes NTSD as a vital component of modern amateur radio emergency communications, providing digital capabilities while maintaining seamless integration with traditional NTS operations and ensuring continued service to the public and served agencies.