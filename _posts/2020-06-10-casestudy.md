---
layout: post
title: Zero Trust Networks - Case Study
excerpt: "Usable Security"
categories: [Usable Security]
comments: true
image:
  feature: https://images.pexels.com/photos/950241/pexels-photo-950241.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940
  credit: 
  creditlink: 
---

# Zero Trust Networks

## Usable Security - Case Study

### Abstract:

The zero trust security concept is centered around the idea that companies or organizations should not automatically place trust in anything inside or outside their network perimeter. Instead organizations should continually verify anything that is connected to their network. Implementing zero trust technology is not an easy or straight forward process and zero trust may not be the right fit for everyone. This paper will cover the different ways trust is established, why the traditional network architecture approaches trust wrong, and examples of zero trust deployed in industry.    

### Section 1: Trust

Trust is not only defined as the absence of risk and uncertainty, but is also defined as a complex human response to situations that contain this risk and uncertainty. To establish trust there are a few requirements that must be fulfilled. The first requirement is vulnerability. When people are vulnerable, trust inherently exists. When establishing trust both parties are vulnerable to the betrayal of the other party. If there was a guarantee that a party would act in accordance with the other party's interest, then there would be no need for trust. The second requirement to establish trust is optimism. In a trusting relationship there needs to be some level of optimism that the other party will have a motive for action on other parties' behalf. The third and last requirement needed to establish trust is competency which is the assumption that individuals will possess the relevant skills or ability needed to perform an action. 1 

The two general types of trust are (human-to-human) interpersonal trust and (human-to-system) system trust. An interpersonal trust relationship develops over a period of time when an expectation of trustworthy behavior is fulfilled between two individuals. However, it is important to note that interpersonal trust relationships are highly dependent on the specific situations in different social interactions. A system trust relationship on the other hand does not develop over time or depend heavily on different social interactions. A system trust relationship contains a complex layered arrangement of systems and networks. These arrangements carry different layers of trust. This can be seen in protocols that often presume there is a reliable and trustworthy relationship between these networks.2 

There are two requirements needed to establish trust in a network environment. The first requirement is secure end-to-end communication. The second requirement is that security is created with no expense to survivability. Security should not be confused with privacy. Security enables the control of digital information while privacy requires that an individual be able to control their personal digital information.  Survivability is the idea that any network should be able to degrade gracefully rather than failing critically. Survivability can be established with distribution and graceful degradation. Graceful degradation means that when one section or device of a network fails this does not affect the rest of the network. The actions of one person does not alter the access of others. 3 

The three-dimension model of trust in a system or network is based on risks rather than user perception of risk and require privacy, security, and reliability. Privacy is based around vulnerability and optimism. Security must be based around motivation and competence. While reliability is there result of the belief in integrity and competency of a party. Trust in a network is mostly influenced by the humans, organizations and governments that control them rather than the network itself. 4 

A traditional network places trust in the network itself, while a zero-trust network secures the network communication and access so that the physical security of the transport layer can be disregarded. 5 A zero-trust network will not assume the actors, systems, or services should be trusted just because they operate within the perimeter of the network. A zero-trust networks architecture is built on five main fundamental assertions. The fist being that the network is always assumed to be hostile. Second the external and internal threats exist on the network at all times. Third the network locality is not sufficient for deciding trust in a network. Fourth every device, user, and network flow is authenticated and authorized. And fifth the policies must be dynamic and calculated from as many sources of data as possible.6 

### Section 2: Issues with Trust in Networks

Now with an understanding of trust and how it relates to network environments, we can examine the issues that trust brings with it to networks. 

One of the most important aspects of a trust relationship are the origins of the commitment and its context.7 Often to complete some general “task”, there usually must be some trust agreement between the parties involved but this can be easily undermined when the ends of the agreement are just for completing said task. For example, in the event of a new hire, the new employee will likely agree to any password policy just because they want the job, so they begin a trust relationship without necessarily fulfilling the original agreement. In some situations, no matter how the original commitment is formed, there is no ability to build trust.  

Overreliance on assurances is another large issue with trust.8 Assurances can range from contract or user agreements to social norms. This brings problems when we blindly accept people’s trust based on social agreements or contracts because we see only the agreements instead of what’s happening in reality. The social contract view provides us with an example of a male employer who is “extra” nice to female co-workers to make it seem like he's treating employees equally.9 Though this still results in sexist behavior and he fails to build trust because the employer is trying to take advantage of our social contract.  

A third problem surrounding trust is inferring trust. Inferred trust can be both implicit and explicit (signals/cues vs. ratings/reviews) although in either case they can lead to deception, exploitation & misinterpretation. Any of these inferred results can be extremely damaging in a network setting since it will turn into a significant vulnerability that an attacker could exploit. If you were to assume every review on Amazon was a legitimate user, you could very easily be led into a disappointing purchase of something that you had inferred would be something else. 

The last issue is the idea of an “All-or-Nothing" trust systems. In traditional network environments it is very common to design the network to have a secure perimeter around your assets. The idea of a castle surrounded by a moat. This has the inevitable failing of once that perimeter is broken all the assets are then accessible. This clearly causes huge security risk in that in the event your network gets comprised, everything gets comprised.  

All these issues present massive vulnerabilities and with constantly evolving infrastructure, we see organization re-thinking their trust models. This is the basis to why there is a push to remove trust completely from corporate environments. 

### Section 3: Case Studies of Zero Trust: Google, Microsoft and WWU Zero Trust

Zero Trust is a relatively new concept for protecting and securing networks, and as such large corporations with a wide attack surface are the primary developers of standards and best practices. The Zero Trust ideology was first introduced by Google under the name BeyondCorp which was a response to the Advanced Persistent Threat (APT) attack by China in 2009 codenamed Operation Aurora.10 Unlike the traditional perimeter security model, BeyondCorp dispels the notion of network segmentation as the primary mechanism for protecting sensitive resources. Instead, all applications are deployed to the public Internet, accessible through a user and device-centric authentication and authorization workflow.11  

<img src="/img/ztn1.png" width="100%" />

There are several novel systems Google employs for this authentication and authorization, namely the access proxy and the access control engine. Gaining access to a resource on the network begins with the access proxy which incorporates several well-established security solutions like Single-Sign On (SSO) and device certificates. When the user attempts to connect to the BeyondCorp network the access proxy negotiates the device certificate with a database of known managed device, then it will redirect the user to the SSO system. Once the device certificate is found and the user is properly authenticated the access control engine is the next step in the process. The access control engine confirms the following information: 
* The user is in the correct group to access the resource. 
* The user has a sufficient trust level. 
* The device is managed and in good standing. 
* The device has a sufficient trust level.  

If all these checks pass then the user and device can access the resource, if any single one fails the request to access the resource is denied.12 

Google BeyondCorp’s transparency has allowed many organizations to capitalize on this new ideology of security, notably Microsoft who has published their own papers detailing their principles of Zero Trust. Microsoft keeps their specific implementation of Zero Trust opaque and instead opts to give out more general guidelines, standards and principles. Microsoft also offers a maturity model so that organizations can determine their own level of adoption of the Zero Trust ideology. The first level is a Traditional network security architecture consisting of: 
* On-premises identities with static rules and some SSO. 
* Limited visibility into devices, cloud environments and logins. 
* A flat network infrastructure.  

The second level is Advanced which involves the following: 
* Hybrid identities are formed from multiple data sources fine-tuned access policies for access. 
* Devices are managed and registered in a database. 
* Networks are segmented and cloud environments are monitored. 
* User behavior analysis is implemented to proactively identify threats. 

The third level is the Optimal implementation which includes: 
* Cloud identities with analytics and dynamic access to apps, networks and data. 
* Data access decisions governed by policy engine with encryption and tracking. 
* Trust has been removed from the network entirely with micro-perimeters and segmentation as well as encryption. 
* Automatic threat detection and response are implemented.13 

<img src="/img/ztn2.png" />

Microsoft’s optimal implementation of Zero Trust shown above focuses more on robust policy formed from different sources to create comparisons than Googles frontloaded access control. With more endpoint visibility than any other organization, it makes sense that Microsoft advocates for monitoring and real-time threat intelligence since they can pull from more data sources than most. This makes their implementation of Zero Trust increasingly interesting to examine. Their emphasis on building policy from as many sources as possible and maintaining it in real-time is a far stretch for most organizations.  

When comparing Google and Microsoft’s Zero Trust solutions there are several key similarities and differences that are worth noting. Starting with the similarities, Google and Microsoft’s implementations are highly centralized with a system that acts as a kind of overseer. These centralized systems gather similar data like SSO, device identity and trust/risk, and user identity and trust/risk. They then both use this data to confirm with the policy that this is allowed and if it is then the user/device is let through.14 The differences begin with how often the data is collected, they are both collecting similar data, but Google only does this on-demand as resources are accessed, Microsoft outlines that they are constantly monitoring even after the resource has been accessed. Additionally, Microsoft draws upon its vast computational resources in the cloud to conduct real-time threat analysis detection and protection, whereas Google is mute on this point. 15 

From these similarities we can determine some best practices and necessary design choices for building and implementing a Zero Trust Network, as follows: 
* There must be a stored identity for both user and device. 
* Both the device and the user must have a trust or risk score associated with their identity. 
* The identity of the user and device must be verified by tokens or keys associated with their identity. 
* There must be a robust, dynamic policy that allows or restricts access based on identity, role, and trust/risk score.  

The final case we will study was built using these design specifications and best practices, although it is still in the Traditional stage of Zero Trust maturity according to Microsoft’s system. The WWU Zero Trust Network is a project that Sam Dinkelman, Scarlette Anderson, John Traner and Josh Stuifbergen have worked on for the past year as their senior capstone project. The Zero Trust Network began with incorporating the above best practices into a system that would be simpler for small to medium sized organizations to implement, the specifications of which are outlined below: 

<img src="/img/ztn3.png" />

The Trust Engine, Policy Engine and Network Agent all represent the various design choices that make up the best practices for Zero Trust. The Trust Engine assigns every user and device an explicit trust score based on metrics gathered from managed end-user devices incorporating both Google and Microsoft’s database of managed devices. This Zero Trust design emphasizes Microsoft’s approach to constantly monitoring the device and user and creating a trust score from the Trust Engine every time a resource is accessed as well as periodically every 30 minutes. The Policy Engine then is like Microsoft and Google’s approach; however, our implementation is much more elementary in practice, we don’t have a robust or vast array of data to draw upon or rich information security policy to draw on. The Network Agent comes directly from Google’s BeyondCorp and mirrors the functionality of the access proxy which can redirect requests with insufficient information or access to different systems. These requests can be redirected to the SSO system so that identity can be verified before they can access the resource, additionally if they do not have the permissions to access the resource their request can be dropped by the Network Agent. The entire system is automated to the end-user who doesn’t have to interact with any system except the Network Agent which simply forwards their requests on their behalf. 

Overall, the design choices for building Zero Trust networks remain largely a by-product of the specific needs of the network and organization. Smaller and medium sized organizations will need less strict and dynamic policies while large organization like Google and Microsoft can draw on their vast collections of data and metrics. As the design of networks begins to shift it becomes important to recognize the specific distinctions between old ideologies of trust in systems and networks and the new ideas that attempt to remove the trust from the systems and networks, with these distinctions in mind we can begin to create new designs for secure networks. 

### Bibliography

[1] McLeod, Carolyn, "Trust", The Stanford Encyclopedia of Philosophy (Fall 2015 Edition), Edward N. Zalta (ed.), URL = <https://plato.stanford.edu/archives/fall2015/entries/trust/>. 

 

[2] Cheshire, Coye. (2011). Online Trust, Trustworthiness, or Assurance?. Daedalus. 140. 49-58. 10.1162/DAED_a_00114. 

 

[3] Camp, L. Jean, Design for Trust. TRUST, REPUTATION AND SECURITY: THEORIES AND PRACTICE, Rino Falcone, ed., Springer-Verlang (Berlin), 2003. Available at SSRN: https://ssrn.com/abstract=627610 

 

[4] Gilman, E., & Barth, D. (2017). Zero trust networks: building secure systems in untrusted networks. Sebastopol, CA: OReilly Media. 

 

[5] Zero Trust Maturity Model. (n.d.). Retrieved June 10, 2020, from https://go.microsoft.com/fwlink/p/?LinkID=2109181&clcid=0x409&culture=en-us&country=US 

 

[6] Ward, R., & Beyer, B. (2014). BeyondCorp: A New Approach to Enterprise Security. Retrieved June 10, 2020, from https://storage.googleapis.com/pub-tools-public-publication-data/pdf/43231.pdf 

 

[7] Dinkelman, S., Stuifbergen, J., Traner, J., & Anderson, S. (2020, June 3). WWU Zero Trust Networks. Retrieved June 10, 2020, from https://wwuzerotrust.com/Documentation/ 

 

[8] Baier, A. C., 1986. “Trust and Antitrust,” Ethics, 96: 231–260. 

 

[9] –––, 1991. “Trust and Its Vulnerabilities” and “Sustaining Trust,” Tanner Lectures on Human Values, Volume 13, Salt Lake City: University of Utah Press. 

[10] –––, 1995. Moral Prejudices: Essays on Ethics, Cambridge, MA: Harvard University Press. 

[11] –––, 2004. “Demoralization, Trust, and the Virtues,” in Calhoun (ed.) 2004. 

[12] Run Zero Trust Security Like Google. (2018). Retrieved June 10, 2020, from https://www.beyondcorp.com/ 