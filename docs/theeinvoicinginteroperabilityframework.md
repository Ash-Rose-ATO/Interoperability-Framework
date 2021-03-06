# 3. The eInvoicing Interoperability Framework

The Framework aims is to provide certainty on how a prescribed set of established open standards can be used to extend eInvoicing to all Australian businesses, minimise the cost of implementation for software providers and enhance business interactions (especially for micro to small businesses) by making invoicing an automatic digital interaction.

## 3.1  What is it

The Council’s Interoperability Framework is based on the concept of standardising interconnections around what is called a ‘four corner model’. Similar models have emerged from the financial sector (for inter-bank interoperability), telecommunications sector (for global roaming) and are already being used in many countries for eInvoicing. In Australia, the
superannuation sector (via Superstream) also uses a standardised form of the ‘four corner model’.


Under this logical model, businesses can send messages :
 - directly to each other by implementing their own
 - Access Points (without intermediaries);
 - via a mutual 3rd party Access Point (3-corners); or 
 - via two independent external service providers (4-corners). 


As the digital economy grows, the trend is toward the increased use of 4-corner models. However, as with rail networks, telephony systems and other communication technologies, unless standards are introduced, complex and expensive interconnections are required to connect all existing participants. The DBC Framework has proposed standards for the creation of an ‘open’ 4-corner
model.

A key requirement for the eInvoicing Interoperability Framework is that a Buyer’s or Supplier’s digital address and digital capabilities may change over time. The associated challenge with using an ‘open’ 4-corner model is finding out what businesses are reachable and what their digital capabilities are.  The Framework resolves this by establishing a business discovery service. The idea of using the 4-corner model with business discovery is a well-established and an internationally accepted solution, and an extension to the existing SuperStream
model.

The actors involved in eInvoicing are:

 - Buyers: The Buyer is the legal person or organisation who purchases goods or services; 
 - Suppliers: The Supplier is the legal person or organisation who provides a good or service; 
 - Access Point: A service (in-houseor outsourced) that sends and receives eInvoices and passes them on to the respective participants;
 - Digital Capability Locator: A service for looking up the location of the Digital Capability Publisher for a Buyer or Supplier; and
 - Digital Capability Publishers: Providers of a service for Buyers and Suppliers to store details of their capabilities, and includes what scenarios they can
process, the data formats they support and the delivery address for their eInvoices.

eInvoicing using the Framework means that the business
applications of the Suppliers and Buyers (corners one and four) do not exchange
invoices directly with each other but via Access Points (corners two and
three). Any organisation (such as a Buyer or Supplier) has the choice of using
a third party service provider to provide an Access Point or to implement their
own.

Finally, the meaning of the information in eInvoices needs
to be understood by all Buyers and Suppliers regardless of the natural business
systems they use, so an agreed set of information elements in a standardised
data format is required for exchanges between Access Points.

## 3.2 How does it work

Interoperability means working together – a collaboration of systems, services and people with common understanding. An interoperability framework can be defined as the overarching set of policies, standards and guidelines that describes how organisations have agreed, or should agree, to do
business with each other[1].

There are four components to the Framework:
 - Legislation and policy: Reducing legal or policy reasons why paper is preferred to digital. This includes recommending refinements to legislation and policy, if any, to remove impediments or barriers to adoption;
 - Organisational interoperability: Describing business process scenarios and standardising how businesses discover each other’s digital capabilities for these scenarios;
 - Semantic interoperability: Standardising the data exchanged so the information is commonly understood by the parties involved; and 
 - Technical interoperability: Technical standards and protocols to ensure information is exchanged securely and reliably between parties (directly or via service providers).

## 3.3 Legislation and Policy 

### 3.3.1 Legislation

The federal, state and local governments are reviewing legislation to identify and recommend opportunities to remove impediments or barriers to adoption. Any relevant changes are expected to be published by the respective Government.

### 3.3.2 Policy

The Framework provides an opt-in solution and does not impact current eInvoicing solutions unless businesses choose to adopt it. This means new participants are not excluded from using or providing eInvoice services and existing eInvoice users or service providers are not excluded form future growth and development.

Within the public sector there is ongoing work within the three levels of government to introduce policies to encourage the use of digital technologies for eInvoicing. Any relevant policy changes for the public sector are expected to be published by the Government. 

### 3.3.3 Agreements and charges

As part of the work to provide implementation guidance and ongoing governance of the framework the Council is expected to provide interoperability agreements for service providers so that:
 - There is an appropriate approach to accreditation and service levels for service providers with periodic reviews;
 - There will be no charges for exchanging documents between Access Points; and
 - There will be an open market for providing Access Points.
 
## 3.4 Organisational Interoperability
### 3.4.1 Business Processes
 
The procurement, accounts payable, accounts reveivable and sales processes of any buyers and suppliers are inextricably linked. Figure 2 shows that invoicing is one sub-process of this broader process.
 
While there are significant benefits in digitising the whole end to end process, overseas evidence suggests it will be more effective and achieve borader market adoption by focusing on the invoice processes as the first step.
 
Eventually, as the ecosystem matures, the entire procure-to-pay process will be digitised (Penttinen, 2008).
 
Figure 2- Abbreviated procure to pay process
 
It is also recognised that procure to pay forms one part of an overall set of supply chain processes, such as financial supply chain (dealing with banking/payment) and the logistical supply chain (dealing with receipt/delivery of the purchased items). Information flows into and out of these processes and so suitable interfaces will also be required. 
 
Business scenarios
 
The business processes introduced in this document are industry neutral and depict a generic cross-industry set of scenarios.
 
Scenario One: Invoicing (and Adjustment Invoices)
 
 1. Supplier's business application to Supplier's Access Point (CORNERS ONE to TWO)
 
The Supplier's business application (for example, an accounts receivable system) creates an invoice detailing purchase(s) made by the Buyer. The Supplier sends this invoice data to their Access Point.

 2. Supplier's Access Point to Buyer's Access Point (CORNERS TWO to THREE)
 
The Supplier's Access Point transforms the Supplier's invoice data to the standardised eInvoice data format (if it is not already in that format). The Supplier's Access Point then uses the Business Discovery service (defined later in this document) to determine the address of the Buyer's Access Point before forarding the eInvoice to that Access Point.
 
 3. Buyer's Access Point to Buyer's business application (CORNERS THREE to FOUR)
 
The Buyer's Access Point transforms the eInvoice data format to the Buyer's required format (if they differ) and delivers this to the Buyer's business application (for example, their accounts payable system).
 
 4. [Optional] Buyer's business applicaiton to Supplier's business application (CORNERS FOUR to ONE)
 The Buyer may acknowledge when the invoice has been received. In which case:
 
 - The Buyer's business application verifies the invoice and sends some form of acknowledgement to their Access Point (CORNER THREE);
 - Buyer's Access Point to Supplier's Access Point (CORNERS THREE to TWO)
 
The Buyer's Access Point transforms the Buyer's acknowledgement into a standardised response message (if they differ), uses the Business Discovery service to discover the locaiton of the Supplier's Access Point and forwards the response message; and

 - Suppler's Access Point to Supplier's business application (CORNERS TWO to ONE)
 
The Supplier's Access Point transforms the response message into an acknowledgement format suitable for the supplier (if required) and forwards the acknowledgement to the Supplier. 
 
Scenario Two: Recipient Created Tax Invoice (RCTI)

With RCTIs a Tax Invoice is issued by the Party receiving the goods or services rather than the Supplier. For example, a sugar cane farmer and a mill, have entered into an agreement and the Buyer will invoice and provide payment for a delivery of cane based quality of the cane. On a delivery of cane to the mill, the Buyer creates a Recipient Created Tax Invoice.

1. Buyer's business application to Access Point (CORNERS ONE to TWO)

The Buyer's business application creates a Recipient Created Tax Invoice detailing the purchase(s) made by the Buyer. The Buyer sends the invoice to their Access Point.

2. Buyer's Access Point to Supplier's Access Point (CORNERS TWO to THREE)
 
The Buyer's Access Point transforms the Buyer's Invoice data to the standardised eInvoice data format (if they differ). The Buyer's Access Point then uses the Business Discovery service to discover the adddress of the Supplier's Access Point before forwarding the eInvoice to that Access Point.

3. Access Point to Supplier's business application (CORNERS THREE to FOUR)
 
The Supplier's Access Point transforms the eInvoice data format to the Supplier's required format (if they differ) and delivers this to the Supplier's business application (for example, their accounts receivable system).
 
### 3.4.2 Business Identifier
 
 A key consideration in the Framework is that all parties who may receive eInvoices (or Responses) need to be uniquely identified.
 
 Business identifiers are information elements that are used to establish the unique identity of businesses (organisations, agencies, branches within organisations, etc.) within the Framework. They are used to identify the parties (sender or receiver) for both business discovery and messaging exchanges. Business identifers also appear within eInvoices themselves to identify parties such as the Supplier and Buyer, it is not a requirement that htey may be so and different Business Identifiers may be used for these roles. 
 
### Framework Business Identifiers;
 - Identify any AUstralian or international private and public sector recipient of digital documents (for example a Buyer) in a standardised and platform independent way;
 - Allows multiple established identification schemes and scheme registries; and
 - Are encoded in a standardised and machine process-able data format. 
 
### 3.4.3 Business Discovery

Digital capability is the ability of an organisation to send and receive digital documents. The target for this digital capability is known as the digital address. For example, a Buyer will have a digital address if they are capable of receiving eInvoices. Delivering an eInvoice to their digital address will result in the Buyer to be able to receive and procee the eInvoice. 

The Business Discovery service is a means of determining a business's digital address for a given type of document within a given process. For example, by supplying a Buyer's business identifier, the type of document (eInvoice) and the process involved (eInvoicing), the Business Discovery service will determine the Buyer's digital address for eInvoices.

However, the digital capabilities registered for a business will change as their services develop and migrate over time. For example, a recipient's Access Point provider may allocate their digital addresses. A benefit of the open Framework is the freedom for businesses to connect with any Access Point provider, or even establish their own Access Points. And so these addresses may change if the Access Point changes and this impacts the registered digital capability of the recipient.

Because of these continually changing details it is necessary to dynamically discover the current digital addresses of recipients. THe finer details of the Business Discovery service are discussed later in the Technical Interoperability section.

## 3.5 Semantic Interoperability
### 3.5.1 How does semantic interoperability help eInvoicing

Semantic interoperability is the ability for different business applications (in this case those of Buyers and Suppliers) to recognise and process the information they exchange.

However businesses operate in different industry, geopolitical, and regulatory contexts that may necessitate different rules and requirements for the information exchanged in an invoice. Consequently, most trading communities and businesses use differing forms of invoices. Transforming the data to suit different contexts is usually required when two parties using different invoice models or formats (for example, between two different communities) need to trade. Such transformations may be a complex and expensive process prone to misinterpretations. As many Suppliers (and Buyers) trade with many different communities this complexity is common and yet another barrier to eInvoicing. 

One proven approach to enabling greater interoperability is to agree upon a colleciton of terms with well-defined meanings that are consistent across alll contexts of use. This is called the semantic model of the core elements.

A semantic model is based on the idea that common pieces of information used in an invoice may have many names, use different terminology and be expressed in different ways, but the meanings are constant and commonly understood. Semantic models help us identify what the common pieces of information mean without the distraction of how we express this. This is similar to how drawing pictures helps people who don't speak a common language to communicate.

THe semantic model is an attempt to remove the language/syntax/grammar/format from information to enable us to compare one thing with another and see if htey are describing the same thing. In the software world this is useful because:
 - Technology is constantly evolving and standardising and the semnatics ensures the invoice information that is standardised does not need redesigning to satisfy new tehcnologies- formats may change by semantics does not need to; and
 - When transforming an invoice between various formats the mapping of information is easier for software developers if there is a common semantic model to reference. 
 
### 3.5.2 The Core eInvoice Semantic Model

The Core eInvoice Semantic Model consists of a dictionary of terms, concepts used, the minimal content of a document, the rules validating the content, the use of identifiers, and code lists. Adopting a single common semantic model promotes reliable information exchange and ensures technology neutrality. It is also easier and cheapter for enterprises to subscribe to a single model as comapred to several.

### The Semantic Model:
 - Inforporates invoice requirements for regulatory e.g. tax, commercial, technical, financial, and industry extentions;
 - Will be aligned with the Austrlaian Reproting Dictionary (through incorporation);
 - Exploits the ability to share the model and gain efficiencies of a standardised data model;
 - Identifies the common case model;
 - Consistent reuse of standardised definitions and meanings provides greater opportunities to optimise business processes and the ability to integrate information with further cost reduction;
 - Makes use of a proven methodology; and
 - The semantic model has been defined and elaborated in a consultative manner- reusing an existing international standard.
 
### 3.5.3 Digital Data Format

The Core eInvoice Semantic Model in itself does not enable software developers to create the necessary eInvoice data files to exchange. The semantic model needs to be expressed in a standardised digital format. The term data format is used to mean the software expression of the information described by the semantic model (also called the message syntax or markup language). In the data format all the data elements, concepts and validation rules defined in the semantic model are expressed in ways computer applications can process.

It may help to remember that the semantic model is for business people to understand while the digital data format is for software developers to understand and computer programs to process.

### The eInvoicing data format:
 - Is based on an international standard;
 - Is aligned with relevant and established international standards. Australian standards and practices will only be adopted where international standards are not applicable;
 - Encompasses procure to pay documents;
 - Will not inhibit the future extension to other elements of the procure to pay process;
 - Has a published semantic model;
 - Will not impose a particular design on internal solutions for stakeholders;
 - Has an established user base;
 - Has open participation and governance;
 - Is open, royalty free and vendor agnostic;
 - Allows development of tools that are easily available;
 - Has interfaces with common business applications; and
 - Enables business to business (B2B) connectivity irrespective of platform or solution to exchange electronic business transactions. 

## 3.6 Technical Interoperability














