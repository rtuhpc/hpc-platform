
# Introduction to Learning Tools Interoperability (LTI) for Instructional Designers teaching High-Performance Computing (HPC)

![](./images/lti-01.png)


## Introduction:
Learning Tools Interoperability (LTI) is a technology standard widely used in the education sector to enhance the interoperability and integration of various learning tools and systems. LTI enables seamless connectivity between learning management systems (LMS) and external learning tools/resources, allowing instructors and learners to access multiple educational resources and services within their LMS environment. This brief guide will provide an overview of LTI and its benefits for instructional designers.

### 1. What is LTI?
LTI, or Learning Tools Interoperability, is a standard protocol developed by the IMS Global Learning Consortium. It enables the integration of external learning tools, such as interactive modules, assessments, simulations, and more, into an existing learning management system. LTI establishes a secure and standardized way for individual learning content providers and platforms like Moodle, Canvas LMS, Sakai, Blackboard, etc., to communicate, ensuring seamless interoperability.

### 2. How does LTI work?
LTI relies on a simple yet powerful mechanism called "launching." When an instructor selects an external tool within their LMS, the LMS launches it in a separate frame or tab. LTI passes essential information, such as user identity and context, from the LMS to the tool, allowing it to provide personalized and contextualized learning experiences. This seamless integration eliminates the need for multiple logins or navigating between different platforms.

### 3. Benefits of LTI for Instructional Designers:
- Enhanced Tool Selection: LTI opens up a vast ecosystem of educational tools and resources that instructional designers can integrate into their courses. This flexibility allows for more varied and engaging learning experiences.
- Streamlined Workflow: LTI eliminates the need for manual data transfers or managing multiple platforms separately. Instructional designers can focus on designing effective content without worrying about technical implementation and integration into the learning ecosystem.
- Personalization and Contextualization: LTI enables transferring user data, such as roles, grades, and progress, between the LMS and external tools. Instructional designers can leverage this data to create personalized and adaptive learning experiences for learners.
- Scalability and Updates: LTI-compatible tools can be easily added or replaced within an LMS, providing scalability and the ability to adapt to changing instructional needs. When teaching-learning tools are updated, the changes are reflected seamlessly across courses using LTI integration.

### 4. LTI Integration Process:
To integrate an external tool using LTI, instructional designers typically follow these steps:
1. Obtain an LTI-compatible tool or content from a vendor or create one in-house.
2. Configure the LTI tool within the LMS by providing must-have information, such as the tool's launch URL, consumer key, and secret.
3. Test the integration to ensure the tool is launching correctly and receiving the necessary user data.
4. Collaborate with the tool provider to customize the tool's behaviour and appearance within the LMS environment.

### Conclusion:
Learning Tools Interoperability (LTI) empowers instructional designers by seamlessly integrating external tools and resources into learning management systems. By leveraging LTI, designers can enhance their courses with a wide range of educational resources while maintaining a streamlined workflow. LTI promotes personalization, contextualization, scalability, and the ability to meet evolving instructional needs. Embracing LTI opens doors to a world of possibilities for instructional designers to create engaging and compelling learning experiences.

## Challenges for Instructional Designers Using LTI in High-Performance Computing Teaching

![](./images/lti-02.png)

When instructional designers use Learning Tools Interoperability (LTI) in teaching High-Performance Computing (HPC), they may encounter several challenges. Here are some common challenges:

1. Technical Compatibility: LTI relies on the compatibility between the learning management system (LMS) and the external HPC tools. Ensuring the HPC tools are LTI-compatible and can seamlessly integrate with the LMS may require technical expertise and coordination with tool providers.

2. Complex Configuration: High-Performance Computing often involves complex software installations and configurations. Integrating HPC tools with an LMS through LTI may require additional configuration steps, such as setting up secure connections, managing authentication mechanisms, and handling large-scale data transfers. Instructional designers may need IT or HPC specialists' assistance to navigate these complexities.

3. Data Security and Privacy: High-Performance Computing often deals with sensitive data, such as research or user information. Instructional designers must ensure that LTI integrations maintain data security and privacy standards. This includes encryption of data transfers, adherence to data protection regulations, and secure user authentication mechanisms.

4. User Authentication and Access Control: HPC systems typically require specific user access privileges and authentication mechanisms. Integrating HPC tools through LTI may require careful consideration of how user authentication and access control are managed within the LMS environment. Instructional designers must ensure that only authorized users can access the HPC resources and that appropriate access controls are in place.

5. Resource Availability and Scalability: HPC resources are often limited and highly demanded. Instructional designers must consider the scalability and availability of HPC tools when integrating them through LTI. Ensuring that the tools can handle multiple concurrent users, manage resource allocation efficiently, and accommodate varying levels of computational demand can be challenging.

6. Training and Support: Instructional designers and faculty may require training and support in using HPC tools integrated through LTI effectively. Providing comprehensive documentation, tutorials, and user support resources can help address any challenges and ensure a smooth user experience.

7. Keeping Pace with Technological Advances: High-Performance Computing rapidly evolves, and new tools and techniques are constantly emerging. Instructional designers using LTI for HPC teaching must stay updated with the latest advancements to provide learners with relevant and up-to-date resources.

Overcoming these challenges requires collaboration between instructional designers, IT professionals, HPC experts, and tool providers. By actively addressing these challenges, instructional designers can leverage LTI to enhance the teaching and learning experiences in High-Performance Computing.


## We use LTI version 1.3

 - *LTI 1.3 offers*: 
Improved security based on OAuth2 and JSON Web Tokens makes security updates safer and more accessible. 
Improved documentation and directions for implementation.
Since LTI 1.3 is built on LTI 1.1, it provides an easier upgrade path, allowing for more straightforward adoption and requiring a smaller learning curve. 

- *LTI Advantage*:
LTI 1.3 improves existing services by allowing new extensions to be layered on the existing launch mechanism. Currently, there are three extensions available in LTI 1.3 and more planned. This bundle of extensions evolves outside the LTI specification and is called LTI Advantage.

- *Deep Linking Service*, which makes it easier to provide links to specific content. This was named a content item previously.

- *Name and Role Provisioning* makes obtaining a list of course participants and roles easier and sends defined information to the learning tools. This extension was also known as *membership service* previously.
  
- *Assignment and Grade Service* makes passing grade information between the tool and the Learning Platform easier. This extension was named the outcome service previously.  
