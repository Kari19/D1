## 1. Background, Problem Statement & Proposed Solution.
### a. Introduction
Emergency response systems play a critical role in safeguarding public health and safety. However, in majority of regions in South Africa, significant inefficiencies and lack of innovation within healthcare responders, crime units, and wild and accidental fire response units have led to severe consequences for communities. The challenges faced by these industries not only exacerbate the vulnerability of community members but also result in tragic loss of life and widespread trauma. The inefficiencies of these systems are primarily rooted in outdated technological infrastructure and fragmented management systems. These critical industries continue to rely on legacy systems that are ill-equipped to handle the growing demands of a rapidly evolving environment and a fast-growing population.

### b. Industry Background:  Emergency Responses in South Africa
South Africa is a diverse country with congested urban areas and vast informal settlements, each facing unique challenges in accessing emergency assistance. The inefficiencies within the current emergency response system have led to delays, particularly in critical situations such as crime, accidents and medical emergencies.

In major cities such as Johannesburg, Cape Town, and Durban, emergency services are often overwhelmed due to high crime rates, accident rates, fire breakouts and large populations. The centralized emergency system, where calls are directed through a national call centre and dispatched to local responders, struggles to manage the volume of incoming calls. In 2020, approximately 40% of calls were abandoned due to long wait times, leaving communities vulnerable.

In informal settlements like Khayelitsha and Alexandra, the lack of proper roads and clear addresses makes it difficult for emergency services to locate those in need. Ambulances and fire trucks often face delays as they navigate poorly mapped areas and rely on directions through phone calls. Additionally due to the underdevelopment in these areas, limited access to private vehicles further exacerbates the situation, as community members are unable to transport patients to hospitals in critical situations. Without clear communication or awareness of the urgency, people might not realize that an ambulance or car is needed quickly, and local volunteers can't step in to help in time. Without this knowledge, they can't offer their own vehicles or assistance to help someone get to the hospital fast, which makes medical emergencies even more dangerous.

Firefighters often respond without adequate information on the size and severity of the fire. This results in the wrong equipment being dispatched initially, causing further delays when additional resources are requested. This inefficiency hampers efforts to contain fires swiftly and protect lives and property.

Community members who witness crime or break-ins in their communities often find it difficult to report these incidents to the police. Reporting crimes to the police means that they must survive lengthy and frustrating call processes which discourage them from reporting incidents. This leads to unreported crimes and a sense of insecurity within communities.

In response to these inefficiencies, communities have established neighbourhood watches, volunteer patrols, and community groups to provide immediate assistance. These local groups leverage their knowledge of the area to respond quicker to emergencies before official services arrive. Communities have turned to WhatsApp groups to share real-time information on crimes, accidents, and medical emergencies. However, this approach has challenges. An overload of messages can cause important updates to be missed, leading to slower response times. While these community-driven efforts are commendable, they often lack financial resources, trained personnel, and legal support. Volunteers rely on personal resources and face legal risks in the absence of official backing.

The struggles faced by South African communities in accessing timely and effective emergency assistance highlight the inefficiencies within the current system.

### c.  Current System Procedures Followed:
 1.	Emergency Health Response Units:
    * Emergency Calls and Reporting:
        * Emergency calls are received through a national call centre.
        * Call operators obtain the address and scene description directly  from the caller.
    * Inter-Departmental Communication:
        * Communication between departments (police, hospitals, fire departments) relies heavily on WhatsApp groups and telephone calls for coordination and updates.

    * Scene Assessment:
        * A scene size-up is conducted during call registration to gauge the emergency’s severity.

    * Dispatch and Deployment:
        * Crews are dispatched based on the initial report.
        * Upon arrival, responders provide a situational report to update the central command.
        * Resources are not strictly area-bound; dispatch from neighbouring towns is possible if local units are occupied.

    * Pre-Arrival Verification:
        * There is no formal pre-arrival verification process; follow-up calls are made to confirm the need for EMS resources.

    * Challenges in Locating Incidents:
        * Locating incidents often relies on landmarks (e.g., churches, schools, taverns) due to the lack of formal addresses.
        * There is a high possibility of incomplete patient information, incorrect contact details, incomplete communication regarding road infrastructure, weather changes, and incorrect usage of EMS resources.
        * High possibility of Incomplete patient information, incorrect contact details, incomplete communication of road infrastructure, weather changes, and incorrect EMS resource usage.

2. Crime Response Units:
    * Emergency Calls and Reporting:
        * Crime-related calls are received through a national call centre (e.g., 10111) or directly via local police stations.
        * Call operators obtain the incident details, including the crime type, location, and a brief scene description from the caller.

    * Initial Assessment and Verification:
        * Call operators conduct a quick assessment to determine the urgency and nature of the crime, sometimes requiring follow-up calls for clarification.
        * Location identification often relies on landmarks or local descriptions due to the absence of formal addresses in many areas.

    * Communication Between Departments:
        * Coordination among various units (local police, specialized crime units, and sometimes community watch groups) is carried out primarily via telephone calls and messaging apps (e.g., WhatsApp).
        * Real-time communication is essential for updating the status of the incident and coordinating response efforts.


    * Dispatch and Deployment:
        * Based on the incident assessment, police patrols or specialized units are dispatched immediately to the scene.
        * In areas with limited local resources, backup units may be dispatched from neighbouring jurisdictions to cover the incident.

    * Scene Size-Up and Initial Reporting:
        * Upon arrival, responding officers perform a scene size-up to assess the situation, gather additional details, and determine immediate risks.
        * Initial situational reports are relayed back to the central command to update the incident status and coordinate further actions if needed.

    * Pre-Arrival Verification:
        * There is often minimal pre-arrival verification; follow-up calls may be made to the caller to confirm details, though this is not consistently enforced.
    * Challenges in Incident Location and Information Gathering:
        * Locating the exact scene relies heavily on landmarks (e.g., shops, schools, community centres) due to the lack of formal addresses.
        * There is a high possibility of incomplete or inaccurate information being provided, such as incorrect contact details or vague descriptions of the crime scene.
        * Communication challenges (e.g., language barriers, noisy environments) can further complicate the verification process and delay response times.

    * Resource Allocation and Coordination:
        * Crime response units are not strictly area-bound, which allows for the possibility of dispatching resources from nearby areas if local units are fully engaged.
        * This flexible resource allocation can sometimes lead to delays if coordinating across jurisdictions is required.

3.	Fire Response Units:

4.	Community Members:

### d. Problem Statement:

### e. Proposed Solution:

## 2.  Requirements Extraction

### Functional Requirements
These requirements apply to all emergency services (Fire, Police, Healthcare):
* Users must register and log in securely using multi-factor authentication (MFA).

* Authorities should be registered by other authorities and have separate roles.

* Authorities should receive immediate alerts for incidents to deploy the appropriate emergency responders based the type of emergency.

* Users should be able to report incidents specifying the type (Fire, Crime, Medical, or multiple types if needed).

* Reports may include:
    * Incident type (Fire, Crime, Medical Emergency)
    * Description (What happened)
    * Location (Auto-detected via GPS or manually entered)
    * Attachments (Photos/videos/audio for better assessment)

* Users should have the ability to create an SOS emergency alert, visible to both authorities (Police) and nearby users.

* Users and emergency responders should have access to a real-time incident map categorized by emergency type:
    * Fire (Red icon)
    * Medical Emergency (Green icon)
    * Crimes (Hidden from public view for security reasons)

* Multi-agency response should be supported for incidents requiring multiple responders (e.g., fire with injuries → Firefighters + Paramedics + Police).

* A priority scoring system should categorize incidents: 
    * High Priority → Multiple reports, life-threatening situations
    * Medium Priority → Needs response but not urgent
    * Low Priority → Minor issue or already handled

* Users should receive notifications about nearby emergencies and emergency broadcasts (e.g., wildfire warnings, curfews, hospital capacity updates).

* Authorities should have a web-based admin dashboard to monitor and manage reports.

* Users should have the option to deactivate their accounts.

* The system should allow for real-time tracking of both medical and firefighting responders viewed by professionals and the community.

* The system should allow for estimated arrival time of emergency responders.

* The system should allow for communication between emergency responders and the reporter during emergencies.

* Police locations must be hidden from the public for security reasons. Crime reports should be routed to police officers without public visibility.

* A pre-arrival aid guide should be available to help users provide aid before responders arrive.

### Non-Functional Requirements
* Response times must be minimal for life-threatening situations.
* The system must comply with security regulations (e.g., POPIA, GDPR).
* Authorities should be able to track response times and generate emergency reports.
* Access control should prevent unauthorized users from accessing sensitive authority data.
* The system should provide accurate real-time tracking.
* The app must support thousands of simultaneous users, especially during disasters.
* The system should have 99.9% uptime with failover mechanisms.

## 3.  Identification and Prioritization of Use Cases

![Login use case](./Login.drawio.svg){width=500px}

![Registration use case](./Registration.drawio.svg){width=500px}

![Emergency reporting use case](./emergencyReporting.drawio.svg){width=500px}

![Dispatch use case](./dispatch.drawio.svg){width=500px}

![Reporting use case](./Reporting.drawio.svg){width=500px}

![Receive report use case](./receiveReport.drawio.svg){width=500px}

![SOS use case](./SOS.drawio.svg){width=500px}


## 4.  Feasibility and Risk Study
#### 4.1 System Feasibility
* Existing Systems Comparison:

    The app shares some common features with safety apps like Namola, including real-time tracking, SOS alerts, and incident reporting. However, our solution focuses on multi-agency coordination for Fire, Police, and Healthcare (with minimal health data to avoid legal issues). This system is designed for rapid incident reporting rather than full-scale command and control like the JOC.

* Differentiating Factors Incorporated:
    * **Multi-Agency Integration**: Unlike Namola, which is primarily focused on personal safety and transport, our app coordinates responses between various emergency services.

    * **Community-Centric Reporting**: By leveraging community-based verification and user-generated reports, the system aims to reduce delays caused by centralized call centres.

    * **Adaptability to Local Challenges**: The app is tailored to address issues such as unclear addresses, limited infrastructure in informal settlements, and high call abandonment rates.

    * **Targeted Functionality**: Our app emphasizes rapid reporting and response, without replicating full JOC functionality. Agencies communicate externally through JOC for detailed coordination, minimizing our system’s scope.

    * **Local Context Adaptation**: Designed specifically for South African challenges—such as unclear addresses in informal settlements and high call abandonment rates in formal settlements—the system will be tailored to local needs.

* Feasibility Verdict:
The system feasibility is high. The focus on rapid reporting and multi-agency coordination is achievable using current technologies, and the design is well-tailored to address local challenges in South Africa.

#### 4.2 Technical Feasibility
* Hardware Requirements:
    * **Mobile Devices**: The app will run on Android devices equipped with GPS for accurate location tracking.
    * **Centralised Database**: The system will have a central database which will keep data updated across different machines.

* Software Requirements:
    * **Frontend**: A mobile application developed using frameworks like Flutter or React Native for cross-platform compatibility.
    * **Backend**: Server-side development using Node.js or Python, with Firebase to handle real-time operations.
    * **Mapping & Location Services**: Integration with Google Maps API or OpenStreetMap for live incident mapping.
    * **Security**: Multi-factor authentication and strict access controls to ensure compliance with POPIA and other security regulations.
    * **Simplified Verification**: Initially, the app will rely on manual and community-based report verification rather than advanced AI.

* Feasibility Verdict:
The technical feasibility is high. The required hardware and software components are available and widely used, and the focus on simplified, manual verification methods reduces technical complexity for the prototype phase.

#### 4.3 Economic Feasibility
* Affordability:
    * Team Composition: The project is being developed by a team of four final-year UJ students.

    * Budget Considerations: 
        * **Student Funding**: South African university projects typically have limited funding; our project may rely on minimal expenses (software licenses, cloud hosting credits, etc.).
        * **Estimated Costs**: Development over a year might incur cloud service expenses in the range of R5,000–R20,000, depending on usage. Additional costs such as hardware testing devices are minimal since most team members already possess smartphones or laptops.
    
    * Time Investment: 
        * The project is scheduled as a year-long effort. Considering that the team consists of four dedicated students, the manpower is considered adequate.
        * Time costs (in terms of effort) are balanced by integrating existing open-source tools and frameworks, minimizing custom development from scratch.
* Comparison with Industry Costs:

    If four junior developers in the industry were to develop a similar system, the project might cost between R100,000 and R200,000 due to higher labour rates, professional overhead, and commercial-grade infrastructure requirements. This comparison underscores the cost-effectiveness of the student-led project.

* Feasibility Verdict:

    The economic feasibility is high for the academic project. The cost is manageable within the constraints of student funding and resources, making it a viable solution compared to industry alternatives.

#### 4.4 Operational Feasibility
* User Adoption and Training:
    * **Intuitive Interface**: Designed for ease of use, ensuring minimal training is required for both community members and emergency responders.
    * **Inter-Agency Integration**: While detailed communication is handled via the JOC, the streamlined reporting and alert system will enhance operational efficiency.
    * **Support Structure**: Initial pilot deployment will include training sessions and support documentation to facilitate smooth adoption.
    * **Legal Considerations**: By limiting health data collection to non-sensitive, general categories, the system minimizes legal risks.

* **Human Factor**:

    Engagement with emergency services early in the pilot phase is planned to ensure the system meets operational needs. Feedback from these stakeholders will be critical to refining the system.

* **Feasibility Verdict**:

    The operational feasibility is high. With a focus on rapid reporting, minimal training requirements, and clear communication channels, the system is poised to integrate well into existing emergency response workflows.

#### 4.5 Risk Analysis
* Technical Risks:
    * Real-time data integrity and location tracking may face challenges in low-bandwidth areas.
    * Integrating with diverse hardware and varying network conditions may introduce inconsistencies.

* Economic Risks:
    * Budget constraints might limit access to high-performance cloud services or advanced AI features, though our focus on manual verification in the prototype mitigates this risk.

* Operational Risks:
    * Potential resistance from emergency services due to changes in established protocols. Early stakeholder engagement will be essential.
    * The risk of false or spam reports impacting reliability is addressed by a robust moderation system.

* Mitigation Strategies:
    * Utilize open-source tools and academic cloud credits to lower development costs.
    * Engage emergency service stakeholders early for feedback and training.
    * Begin with manual verification and simple prioritization methods, with the potential to integrate advanced features later.

## Conclusion

The development of the Crowdsourced Local Disaster Management App is deemed feasible on multiple fronts. The system's design—focusing on rapid incident reporting, multi-agency integration, community-centric verification, and adaptability to local challenges—addresses critical gaps in South Africa's current emergency response infrastructure. From a technical and economic standpoint, the project is well within reach for a student-led initiative. Operationally, the intuitive design and early stakeholder engagement will ensure smooth adoption. While challenges exist, they are mitigated through careful planning and phased implementation. Overall, the project is feasible and has the potential to significantly improve emergency response outcomes in South African communities.