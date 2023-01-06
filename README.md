# VDI5100 Ontology-Design-Pattern

## Introduction

The development of software functionalities, or applications in general, that monitor and analyze manufacturing related data in order to improve, support or automate processes, is becoming increasingly important in industry. These applications require several information from different data sources in their context. An application that is planning a maintenance workers daily schedule for instance, requires several information about machine statuses, production plans and inventory, which resides in different systems likes Programmable Logical Controllers (PLC) or Structured Query Language (SQL) databases. Furthermore, manufacturing companies usually run machines and software systems from different vendors or of different ages. The schemata used in such systems do therefore not follow a certain standard, i.e. they are very heterogeneous in their semantics. When building such applications, accessing, searching and understanding the data sources is becoming a very time intensive, manual and error prone procedure that is repeated for every newly build application and for every newly introduced data source. To allow for an eased access, searching and understanding of these heterogeneous data sources, an ontology can be used to integrate all heterogeneous data sources in one schemata. 

This repository contains an ontology of VDI5100 which is a standard to describe the system architecture of an intralogistics plant. We maintain a whole list of standard-based ontologies, check out these links:
 - [VDI 2206](https://github.com/hsu-aut/IndustrialStandard-ODP-VDI2206)
 - [VDI 2860](https://github.com/hsu-aut/IndustrialStandard-ODP-VDI2860)
 - [VDI 3682](https://github.com/hsu-aut/IndustrialStandard-ODP-VDI3682)
 - [DIN 8580](https://github.com/hsu-aut/IndustrialStandard-ODP-DIN8580)
 - [DIN EN 61360](https://github.com/hsu-aut/IndustrialStandard-ODP-DINEN61360)
 - [WADL](https://github.com/hsu-aut/IndustrialStandard-ODP-WADL)
 - [DIN EN 62264-2](https://github.com/hsu-aut/IndustrialStandard-ODP-DINEN62264-2)
 - [OPC UA](https://github.com/hsu-aut/IndustrialStandard-ODP-OPC-UA)
 - [ISO 22400-2](https://github.com/hsu-aut/IndustrialStandard-ODP-ISO22400-2)
 - [ISA 88](https://github.com/hsu-aut/IndustrialStandard-ODP-ISA88)


## VDI5100

The VDI 5100 describes a system architecture for intralogistics. 
It is an architectural model used to describe components for intralogistic systems as well as their basic functions and
principle interfaces.

A detailed description of all Interfaces can be found in the standard [VDI/VDMA 5100 Part 1].

![](./pictures/VDI5100ComponentsFunctions.png?raw=true "VDI5100 Components and their Functions")<br></br>
Figure 1: VDI5100 Components and their Functions

Fig. 1 shows the Components defined in the Standard as well as their functions.

![](./pictures/VDI5100InformationExchange.png?raw=true "VDI5100 VDI5100 Information Exchange")<br></br>
Figure 2: VDI5100 Information Exchange at Interfaces between Components

Fig. 2 shows the Information that can be exchanged between the different components. 


## Usage

If you want to this ontology design pattern, the easiest way is to directly import it into your ontology via `owl:imports` statements. Make sure to reference a fixed release version so that you can't get surprised by future changes. To do so, click on the branch selection right below the number of commits and select a tag from the dropdown, e.g. v1.0.0. Then navigate to the .owl-file and open the raw file. For this example it would be https://raw.githubusercontent.com/hsu-aut/IndustrialStandard-ODP-VDI5100/v1.0.0/VDI5100.owl. You can use this URL in an `owl:imports` statement of your ontology. If you're having trouble using this URL in a tool like Protégé, try opening your ontology with a text editor and simply inserting your imports manually.
An example of an imports section looks like this:

```xml
<owl:Ontology rdf:about="http://www.hsu-ifa.de/ontologies/capability-model#">
    <owl:versionIRI rdf:resource="http://www.hsu-ifa.de/ontologies/capability-model/1.0.0#"/>
    <owl:imports rdf:resource="https://raw.githubusercontent.com/hsu-aut/IndustrialStandard-ODP-VDI5100/v1.0.0/VDI5100.owl"/>
</owl:Ontology>
```
Of course you can also clone or download this repository and import an ODP from a local copy. The advantage of the first approach is that tools like Protégé or TopBraid Composer will directly use the ontologies from the internet and you can simply increase the version number in case you want to use a newer version of our ODPs.

## Further reading:
- C. Hildebrandt, A. Köcher, C. Kustner, C.-M. Lopez-Enriquez, A.W. Muller, B. Caesar, C.S. Gundlach, A. Fay: Ontology Building for Cyber-Physical Systems: Application in the Manufacturing Domain. IEEE Transactions on Automation Science and Engineering, 2020, S. 1–17.
-  C. Hildebrandt, S. Törsleff, T. Bandyszak, B. Caesar, A. Ludewig, A. Fay: Ontology Engineering for Collaborative Embedded Systems – Requirements and Initial Approach. In: Schäfer, Karagiannis (Hrsg.): Fachtagung Modellierung, 2018.
- C. Hildebrandt, S. Törsleff, B. Caesar, A. Fay: Ontology Building for Cyber-Physical Systems: A domain expert centric approach. In: 2018 14th IEEE Conference on Automation Science and Engineering (CASE 2018), 2018.
- C. Hildebrandt, A. Scholz, A. Fay, T. Schröder, T. Hadlich, C. Diedrich, M. Dubovy, C. Eck, R. Wiegand: Semantic Modeling for Collaboration and Cooperation of Systems in the production domain. In: 22nd IEEE Emerging Technology and Factory Automation (ETFA), 2017.
