### 28-Jan-24-Sun

## Describe security and compliance concepts

[Describe security concepts and methodologies - Training | Microsoft Learn](https://learn.microsoft.com/en-us/training/modules/describe-security-concepts-methodologies/)

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/8de25d76-f925-486f-8b46-cdcfd96cf0f6)

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/1633bcee-de53-4ac1-9866-4f52749c5225)

### Introduction

**1 minute**

As more business data is being accessed from locations outside of the traditional corporate network, security and compliance have become overriding concerns. Organizations need to understand how they can best protect their data, regardless of where it's accessed from, and whether it sits on their corporate network or in the cloud. In addition, organizations need to ensure they're compliant with industry and regulatory requirements to ensure the protection and privacy of data.

This module introduces some important security and compliance concepts. You'll learn about the shared responsibility model, defense in depth, and Zero Trust model. You'll be introduced to the concepts of encryption and hashing as ways to protect data. Lastly, you'll learn about concepts that relate to compliance.

After completing this module, you'll be able to:

- Describe the shared responsibility and the defense in-depth security models.
- Describe the Zero-Trust model.
- Describe the concepts of encryption and hashing.
- Describe some basic compliance concepts.

### Describe the shared responsibility model

**3 minutes**

In organizations running only on-premises hardware and software, the organization is 100 percent responsible for implementing security and compliance. With cloud-based services, that responsibility is shared between the customer and the cloud provider.

The shared responsibility model identifies which security tasks are handled by the cloud provider, and which security tasks are handled by you, the customer. The responsibilities vary depending on where the workload is hosted:

- Software as a Service (SaaS)
- Platform as a Service (PaaS)
- Infrastructure as a Service (IaaS)
- On-premises datacenter

The shared responsibility model makes responsibilities clear. When organizations move to the cloud, some responsibilities transfer to the cloud provider and some to the customer organization.

The following diagram illustrates the areas of responsibility between the customer and the cloud provider, according to where data is held.

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/479d899e-2c73-454a-899f-4a1ae585d42e)

- **On-premises datacenters.** In an on-premises datacenter, you have responsibility for everything from physical security to encrypting sensitive data.

- **Infrastructure as a Service (IaaS).** Of all cloud services, IaaS requires the most management by the cloud customer. With IaaS, you're using the cloud provider’s computing infrastructure. The cloud customer isn't responsible for the physical components, such as computers, the network, or the physical security of the datacenter. However, the cloud customer still has responsibility for software components running on that computing infrastructure such as operating systems, network controls, applications, and protecting data.

- **Platform as a Service (PaaS).** PaaS provides an environment for building, testing, and deploying software applications. The goal of PaaS is to help you create an application quickly without managing the underlying infrastructure. With PaaS, the cloud provider manages the hardware and operating systems, and the customer is responsible for applications and data.

- **Software as a Service (SaaS).** SaaS is hosted and managed by the cloud provider, for the customer. It's usually licensed through a monthly or annual subscription. Microsoft 365, Skype, and Dynamics CRM Online are all examples of SaaS software. SaaS requires the least amount of management by the cloud customer. The cloud provider is responsible for managing everything except data, devices, accounts, and identities.

For all cloud deployment types you, the cloud customer, own your data and identities. You're responsible for protecting the security of your data and identities, and on-premises resources including mobile devices, PCs, printers, and more.

In summary, responsibilities always retained by the customer organization include:

- Information and data
- Devices (mobile and PCs)
- Accounts and identities

The benefit of the shared responsibility model is that organizations are clear about their responsibilities, and those of the cloud provider

### Describe defense in depth

**4 minutes**

Defense in depth uses a layered approach to security, rather than relying on a single perimeter. A defense in-depth strategy uses a series of mechanisms to slow the advance of an attack. Each layer provides protection so that, if one layer is breached, a subsequent layer will prevent an attacker getting unauthorized access to data.

Example layers of security might include:

- **Physical** security such as limiting access to a datacenter to only authorized personnel.
- **Identity and access** security controls, such as multifactor authentication or condition-based access, to control access to infrastructure and change control.
- **Perimeter** security of your corporate network includes distributed denial of service (DDoS) protection to filter large-scale attacks before they can cause a denial of service for users.
- **Network** security, such as network segmentation and network access controls, to limit communication between resources.
- **Compute** layer security such as securing access to virtual machines either on-premises or in the cloud by closing certain ports.
- **Application** layer security to ensure applications are secure and free of security vulnerabilities.
- **Data** layer security including controls to manage access to business and customer data and encryption to protect data.

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/b9e850b3-5eab-41a8-81ab-1e2fed128bfd)

**Confidentiality, Integrity, Availability (CIA)**

As described above, a defense in-depth strategy uses a series of mechanisms to slow the advance of an attack. All the different mechanisms (technologies, processes, and training) are elements of a cybersecurity strategy, whose goals include ensuring confidentiality, integrity, and availability; often referred to as CIA.

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/fa700017-c8e1-494e-b3b5-7c7f293778a9)

- **Confidentiality** refers to the need to keep confidential sensitive data such as customer information, passwords, or financial data. You can encrypt data to keep it confidential, but then you also need to keep the encryption keys confidential. Confidentiality is the most visible part of security; we can clearly see need for sensitive data, keys, passwords, and other secrets to be kept confidential.

- **Integrity** refers to keeping data or messages correct. When you send an email message, you want to be sure that the message received is the same as the message you sent. When you store data in a database, you want to be sure that the data you retrieve is the same as the data you stored. Encrypting data keeps it confidential, but you must then be able to decrypt it so that it's the same as before it was encrypted. Integrity is about having confidence that data hasn't been tampered with or altered.

- **Availability** refers to making data available to those who need it, when they need it. It's important to the organization to keep customer data secure, but at the same time it must also be available to employees who deal with customers. While it might be more secure to store the data in an encrypted format, employees need access to decrypted data.

While the goals of a cybersecurity strategy are to preserve the confidentiality, integrity, and availability of systems, networks, applications, and data; it's the goal of cybercriminals to disrupt these goals. Microsoft’s portfolio includes the solutions and technologies to enable organizations to deliver on the goals of the CIA triad.

### Describe the Zero Trust model

**5 minutes**

Zero Trust assumes everything is on an open and untrusted network, even resources behind the firewalls of the corporate network. The Zero Trust model operates on the principle of “trust no one, verify everything.”

Attackers’ ability to bypass conventional access controls is ending any illusion that traditional security strategies are sufficient. By no longer trusting the integrity of the corporate network, security is strengthened.

In practice, this means that we no longer assume that a password is sufficient to validate a user but add multi-factor authentication to provide additional checks. Instead of granting access to all devices on the corporate network, users are allowed access only to the specific applications or data that they need.

This video introduces the Zero Trust methodology:

https://www.microsoft.com/en-us/videoplayer/embed/RE4J3ms?postJsllMsg=true

### Zero Trust guiding principles

The Zero Trust model has three principles which guide and underpin how security is implemented. These are: verify explicitly, least privilege access, and assume breach.

- **Verify explicitly.** Always authenticate and authorize based on the available data points, including user identity, location, device, service or workload, data classification, and anomalies.
- **Least privileged access.** Limit user access with just-in-time and just-enough access (JIT/JEA), risk-based adaptive policies, and data protection to protect both data and productivity.
- **Assume breach.** Segment access by network, user, devices, and application. Use encryption to protect data, and use analytics to get visibility, detect threats, and improve your security.

### Six foundational pillars

In the Zero Trust model, all elements work together to provide end-to-end security. These six elements are the foundational pillars of the Zero Trust model:

- **Identities** may be users, services, or devices. When an identity attempts to access a resource, it must be verified with strong authentication, and follow least privilege access principles.
- **Devices** create a large attack surface as data flows from devices to on-premises workloads and the cloud. Monitoring devices for health and compliance is an important aspect of security.
- **Applications** are the way that data is consumed. This includes discovering all applications being used, sometimes called Shadow IT because not all applications are managed centrally. This pillar also includes managing permissions and access.
- **Data** should be classified, labeled, and encrypted based on its attributes. Security efforts are ultimately about protecting data, and ensuring it remains safe when it leaves devices, applications, infrastructure, and networks that the organization controls.
- **Infrastructure,** whether on-premises or cloud based, represents a threat vector. To improve security, you assess for version, configuration, and JIT access, and use telemetry to detect attacks and anomalies. This allows you to automatically block or flag risky behavior and take protective actions.
- **Networks** should be segmented, including deeper in-network micro segmentation. Also, real-time threat protection, end-to-end encryption, monitoring, and analytics should be employed.

![image](https://github.com/r1skkam/Microsoft-Security-Compliance-and-Identity-Fundamentals/assets/58542375/6e8e8007-40ab-4aab-894a-c4ed4e8b941b)

A security strategy that employs the three principles of the Zero Trust model across the six foundational pillars helps companies deliver and enforce security across their organization.
