---
date: 2017-05-21T18:42:19+02:00
title: Chapter 1 The Urban Mobile Cloud Computing (UMCC) Architecture
---

## 1.1 Introduction to the UMCC in a smart city scenario

The increasing urbanization level of the world population has driven the development of technology toward the definition of a smart city geographic system, conceived as a wide area characterized by the presence of a multitude of smart devices, sensors and processing nodes aiming to distribute intelligence into the city; moreover, the pervasiveness of wireless technologies has led to the presence of heterogeneous networks operating simultaneously in the same city area. One of the main challenges in this context is to provide solutions able to optimize jointly the activities of data transfer, exploiting the heterogeneous networks, and data processing, by using different types of devices. In this chapter, the UMCC framework is introduced, considering a mobile cloud computing model that describes the flows of data and operations taking place in the smart city scenario.

The challenges and the opportunities of exploiting the UMCC are discussed in relation to smart city solutions, highlighting the features that can affect the QoS of various types of smart city related services.

The UMCC sprang from the MCC, that is gaining an increasing interest in the recent years, due to the possibility of exploiting both cloud computing and mobile devices for enabling a distributed cloud infrastructure [9].
Considering the peculiarity of the MCC, we can observe that, on one hand, the cloud computing idea has been introduced as a mean for allowing a remote computation, storage and management of information, and, on the other hand, the mobility skill allows to gain by the most modern smart devices and broadband connections for creating a distributed and flexible virtual environment. 
At the same time, the recent advances in the wireless technologies are defining a novel pervasive scenario where several heterogeneous wireless networks interact among them, giving the users the ability to select the best network among those present in a certain area.

As a consequence, the development of the UMCC is introduced, gaining from both computing and wireless communication technologies. It is a challenging opportunity for the creation of smart city infrastructures, providing solutions fulfilling the urgent need for richer application and services, requested from citizens that, as mobile users, are facing many demanding tasks in relation to mobile device resources as battery life, storage and bandwidth.

### The triple role of Smart Mobile Devices

By analyzing the technology systems underlying a smart city framework, mobile devices can be considered in a three-fold way, as illustrated in fig.1:

- **Sensors**: They can acquire different types of data regarding the users and the environment, transmitting a large amount of information to the cloud in real time, by means of wireless communication systems. This is the underlying concept of IoT, profitably exploited to improve urban life, for instance for extracting descriptive and predictive models in the urban context of cities [10]. As well as the expansion of Internet-connected automation into a plethora of new application areas, IoT is also expected to generate large amounts of data from diverse locations, with the consequent necessity for quick aggregation of the data, and an increase in the need to index, store, and process such data more effectively.

- **Nodes**: 
They can form distributed mobile clouds where the neighboring mobile devices are merged for resource sharing, becoming integral part of the network. Furthermore, they can form VCNs offering content routing, security, privacy, monitoring, virtualization services [11], easy to be used for providing smart city services and applications, in particular for traffic and mobility control. This is the crucial concept of fog networking, where a collaborative multitude of users carry out a substantial amount of storage, communication, and data management in a collaborative way.

- **Outputs**: 
They can make the citizens aware of results and able to decide consequently, or become actuators without need of human intervention. This is the concept underlying M2M communications where computers, embedded processors, smart sensors, actuators and mobile devices acquire information and act in an autonomous way [12].

To perform this triple role, mobile devices have to become part of an infrastructure that is constituted by different cloud topologies and, at the same time, have to exploit heterogeneous wireless link technologies, allowing to address the different requirements of a smart city scenario. This infrastructure starts from the concept of MCC, where the cloud works as a powerful complement to resource-constrained mobile devices.

{{< figure src="../../figures/SMDclassification.png" title="Fig 1.1 - Mobile devices acting in the UMCC framework as (a) sensors, (b) nodes, (c) outputs." >}}

The vision of MCC has increasingly become a source of interest, beginning from the early 2000s, when Amazon realized that a huge amount of space on their premises was underused. This awareness pushed toward the implementation of remote services, gaining by the presence of storage space and computing power and creating a cloud system. Alongside with the expansion of wireless technologies, the cloud computing has been integrated through a broadband system, exploiting the opportunity of working in mobility. The SMDs, then, can use MCC devolving demanding tasks and referring to it for data storage.

### Computation Offloading

The strategy allowing to delegate to one or more cloud computing elements storage and computing functions is commonly called *cyberforaging* or *computation offloading*. It allows to tackle with the limited battery power and computation capacity of the SMDs, and plays a key role in a smart environment where wireless communication is of utmost relevance, particularly in mobility and traffic control domains [13]. If the storage is one of the most common and legacy activities that can be delegated to a remote cloud infrastructure, recently, thanks to modern programming paradigms, it is possible to allot even only a part of the computation load to a remote unit. This allows users to optimize the system performance by offloading only a fraction of the application to be computed, or distributing the application among different cloud structures. Offloading is an effective network congestion reduction strategy to solve the overload issue compared to scaling and optimization [14]. It enables network operators to reduce the congestion in the cellular networks, while for the end-user it provides cost savings on data services and higher bandwidth availability.

## 1.2 Cloud Topologies

In relation to the SMD's roles previous described, we take into account various cloud topologies. This is a different categorization with respect to the common taxonomy used for cloud computing - SaaS, PaaS and IaaS. It looks on the different interaction among the nodes that form the cloud, instead of the services provided by the cloud itself, so we can distinguish among centralized cloud, cloudlet, distributed mobile cloud and a combination of all, as shown in fig 2.

{{< figure src="../../figures/UMCC_topologies.jpg" title="Fig 1.2 - Cloud topologies in the UMCC framework: centralized cloud, cloudlet and distributed mobile cloud." >}}

### Centralized Cloud

A centralized cloud provides the citizens to interact remotely, e.g., for accessing to open data delivered by the public administrations. It refers to the presence of a remote cloud computing infrastructure having a huge amount of storage space and computing power, virtually infinite, offering the major advantage of the elasticity of resource provisioning. The centralized cloud infrastructure is often used for delivering the computing processes to remote clusters, owing a higher computing power, and/or for storing big amount of data. The centralized cloud allows to reduce the computing time by exploiting powerful processing units, but it could suffer from the distribution latency, due to the data transfer from the users to the cloud and vice versa, the congestion, due to the multiple users exploitations, and the resiliency, due to the presence of a single performing infrastructure leading to the SPOF issue.

### Cloudlet

One of the main drawback of the centralized cloud is the great distance between the mobile devices, requesting services, and the clusters, performing computation in the cloud. Even if the SPOF issue is often resolved by implementing mirroring or redundancy solutions, the big distance that may occur between users and centralized clouds can be better addressed by means of the introduction of cloudlets, representing small clouds installed in proximity of the users. Furthermore, the inclusion of cloudlets allows a most appropriate sizing depending on the number of contemporary requests of the users.

Cloudlets are fixed small cloud infrastructures installed between the mobile devices and the centralized cloud, limiting their exploitation to the users in a specific area. Their introduction allows to decrease the latency of the access to cloud services by reducing the transfer distance at the cost of using smaller and less powerful cloud devices.

### Distributed Mobile Cloud

A third configuration can address the issue of non persistent connectivity, whereas both the previous concepts must assume a durable state of connection. In a distributed mobile cloud the neighboring mobile devices are pooled together for resource sharing [15]. An application from a mobile device can be either processed in a distributed and collaborative fashion on all the mobile devices or handled by a particular mobile device that acts as a server.

The possibility of implementing a distributed mobile cloud infrastructure has become a reality since the introduction of smarter and powerful mobile devices, e.g., smartphones, tablet, phablet, having the ability, even if limited, of computing and storaging. Moreover, it has to be noted that their number is still increasing, leading to a pervasive presence and allowing to form a cloud of pervasive distributed devices that can interact among them. This fog network architecture uses one or a collaborative multitude of end-user clients or near-user edge devices to carry out a substantial amount of storage (rather than stored in centralized clouds), communication, and control, configuration, measurement and management [7], [8]. It can be seen as the fog layer that encapsulates phisical objects - equipped with computing, storage, networking, sensing, and/or actuating resources - and constitutes a piece of a wider CARS architecture [16], a geographically distributed platform that connects many billions of sensors and things, and provides multitier layers of abstraction of sensors and sensor networks, enabling the SenaaS.

### Combination of different topologies

The proposed framework foresees the joint exploitation of the three aforementioned topologies. As outlined before, they are characterized by different features, leading to a different usage depending on the scenario. Hence, a joint exploitation could steer to a more efficient usage aiming to achieve the performance goals of a certain application. As it will be better specified below, a smart city scenario is characterized by the presence of a lot of different applications, each one with different characteristics and requirements. An integrated UMCC framework composed by centralized clouds, cloudlets and distributed mobile clouds, as shown in fig 2, allows to respect the application requirements with regard to other solution in a more efficient way.

## 1.3 Types of RATs

In order to connect the devices, different types of RATs should be taken into consideration, providing a pervasive wireless coverage.

Multiple RATs, such as IEEE 802.11, mobile WiMAX, HSPA+, LTE and WiFi, have to be integrated to form a HetNet. For enhancing the network capacity, generally there is an increasing interest in deploying relays, distributed antennas and small cellular base stations - picocells, femtocells, etc - indoors in residential homes and offices as well as outdoors in amusement parks and busy intersections. These new network deployments, comprised of a mix of low-power nodes underlying the conventional homogeneous macrocell network, by deploying additional small cells within the local-area range and bringing the network closer to users, can significantly boost the overall network capacity through a better spatial resource reuse. Inspired by the attractive features and potential advantages of HetNets, their development have gained much momentum in the wireless industry and research communities during the past few years. The heterogeneous elements are distinguished by their transmit powers/coverage areas, physical size, backhaul, and propagation characteristics.

We can basically distinguish between two components, i.e., macrocells and small cells, where the former provide mobility while the latter boost coverage and capacity.

### Macrocells

The distance between the access points (base stations of the macrocells) is usually higher than 500~m. Thanks to this type of base stations the environment is completely covered and the devices can move by minimizing the handover frequency. On the other hand, in macrocells the system suffers for channel fading and traffic congestion. This leads to a lack of stability, not allowing to reach very high data rate. The technology used for this type of cells refers to the cellular networks, e.g. 3G and LTE.

### Small Cells

Small cells are characterized by low power radio access nodes, which have a cover range of about 100-200~m or less. We can distinguish between picocells, for providing hotspot coverage in public places - malls, airports and stadiums - without limits in terms of number of connected devices, and femtocells, for covering a home or small business area, available only for selected devices. Picocells and femtocells have been recently introduced as a way for increasing the coverage and maximize the resource allocation in LTE networks. We also consider WiFi access points as nodes with a small cover range (less than 100 m) which can typically communicate with a small number of client devices. However, the actual range of communication can vary significantly, depending on such variables as indoor or outdoor placement, the current weather, operating radio frequency, and the power output of devices.

## 1.4 Challenges of the UMCC

The UMCC approach foresees the definition of a scenario where smart city applications can exploit jointly the three topologies, as shown in fig.3, by distributing and performing among the different parts composing the framework. The application requested by a particular SMD, signed as the RSMD, is partitioned and distributed among the different clouds using the available RATs. In the example of fig.3, the application is divided among the centralized cloud, two cloudlets, and a distributed cloud formed by five devices. Furthermore, part of the application can be computed locally by the RSMD itself.

The main issue is that, for transferring data from the requesting mobile device to the selected cloud topology, a certain time is required. This mostly depends on some communication parameters of the selected RAT, such as the end-to-end throughput, the amount of users, the QoS management of a certain transmission technology between the user device and each type of cloud processing unit. Furthermore, in terms of energy consumption, it should be taken into account the tradeoff between the energy saved in offloading part of the application to the cloud and the energy spent in sending the data.

{{< figure src="../../figures/offloading-distribution.jpg" title="Fig 1.3 - The process of distributing and performing the application among different parts of the UMCC." >}}

Hence, when a RSMD needs to select the clouds infrastructures to be used for computing the smart city application, two main elements have to be taken into account:

- the processing and storage devices - smart mobiles, per se or together forming distributed mobile clouds, and cloud servers, constituting the cloudlets and the centralized cloud;

- the wireless transmission equipments, - different RAT nodes entailing diverse transmission speeds in relation to their own channel capacity and to the number of linked devices.

In fig.3, the UMCC framework is sketched by representing the functional flows of the architecture. Whenever a smart city application should be performed, the citizen within the UMCC can select among different MCC infrastructures, i.e., centralized clouds, cloudlets, and distributed mobile clouds, aiming to respect the requirements of the specific application depending on their features. The distribution depends on the application requirements, and the UMCC features; its optimization will be discussed in the Section 1.7.

Computation, storage, and tranmission features

The features of the selected processing and storage devices, considered per se or in a group forming cloud/cloudlets, are:


- **Processing Speed**: The processing speed corresponds to the performance speed of a device or a group of devices for processing the applications;

- **Storage Capacity**: The storage capacity corresponds to the amount of storage space provided by a device or a group of devices.

In the same time, the features of the transmission equipments to be taken into account are:

- **Channel Capacity**: The nominal bandwidth of a certain communication technology that can be accessed by a certain device;

- **Priority/QoS management**: The ability of a certain communication technology to manage different QoS and/or priority levels;

- **Communication interfaces**: The number of communication interfaces of each device, that impacts on the possibility of selection among the available heterogeneous networks.

## 1.5 The UMCC model

In this paragraph we focus on the different entities playing a role in the \gls{UMCC} framework, describing the functions and the interactions among them. First of all, we are focusing on an application ${App}$ requested by a \gls{RSMD}, defined through the number of operation to be executed, $O$, the amount of data to be exchanged, $D$, and the amount of data to be stored, $S$. An application can be seen as a smart city service, that can be executed either locally or remotely by exploiting the cloud infrastructures. Furthermore, each application has many requirements regarding the levels of \gls{QoS}. We have taken into account the following:

- the maximum accepted latency $T_\textit{app}$, intended as the interval between the request of performing an application and the acquisition of its results by the \gls{RSMD},

- the minimum level of energy consumption $E_\textit{app}$, that the \gls{RSMD} necessarily uses for performing the application itself,

- the throughput $\eta_\textit{app}$, intended as the minimum bandwidth that the application needs for being performed.

Hence, for highlighting the $\textit{App}$ dependence from the above measures, we can write: 
  $${App = App(O,D,S,T\_\textit{app},E\_\textit{app},\eta\_\textit{app})}$$

A foundamental entity acting in the system is the \gls{RSMD} requesting the $\textit{App}$, we named $\textit{Dev}$, characterized by certain features that are involved in the offloading operation: the power to compute applications locally, $P\_l$, the power used for transferring data towards clouds, $P\_{\textit{tr}}$, the power for idling during the computation in the cloud, $P\_{\textit{id}}$, the computing speed to perform locally the computation, $f\_{\textit{l}}$, and the storage availability, $H\_{\textit{l}}$. Furthermore, also the time-varying position of the device plays an important role in the system interactions. Hence, we can write:


