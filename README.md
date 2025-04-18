<p align="center">
  <a href="https://www.pega.com">
    <img src="https://www.pega.com/themes/custom/pegawww_theme/images/pega-logo.svg" alt="pega" width="500">
  </a>
</p>

# Modern Data Storage Technologies

Database systems have transformed dramatically from their inception in the 1960s to the cloud-based platforms of today. This evolution has been driven by growing demands for **scalability**, **performance**, **flexibility**, and the ability to handle ever-**increasing** **volumes** of data. Over the decades, the dominant database models have shifted from early navigational (hierarchical and network) databases, to the relational model, and more recently to NoSQL and cloud-based solutions. Each stage in this journey was influenced by the limitations of the previous generation and the emerging needs of the time.

Over the course of this 3-hour interactive session, we will learn:
* modern storage technologies and
* apply them to the designed system.

# Prerequisites

* **A Laptop**
* **Basic Command-Line Skills**: Comfortably navigate directories and execute simple terminal commands.
* **Git Fundamentals**: Familiarity with cloning repositories, committing changes, and pushing to remote branches.
* **GitHub Account**: If you don’t already have one, create a free account on GitHub.
* **Access to draw.io**: A tool for creating and collaborating on diagrams.

# Agenda

## High-level

Below is a high-level breakdown of the 3-hour bootcamp session:
* Storage: A Historical overview and evolution
* Key characteristics of different storage technologies
* Modern storage solutions
* Designing the **Nerby Friends** application

## Schedule

| Time (Approx.) | Activity                              |
| -------------- | ------------------------------------- |
| 16:00 (20 min) | Short intro & ice breaker             |
| 16:20 (40 min) | Historical overview & Modern storages |
| 17:00 (30 min) | Designing the app, part 1             |
| 17:30 (15 min) | Pizza time 🍕                         |
| 17:45 (60 min) | Designing the app, part 2             |
| 18:45 (15 min) | Summary & Closing Remarks             |

# Storage historical overview and its evolution

Have you ever wondered how our data storage capabilities transformed from bulky [**magnetic tapes**](https://en.wikipedia.org/wiki/Magnetic_tape) and basic [hard disk drives (**HDDs**)](https://en.wikipedia.org/wiki/Hard_disk_drive) to the lightning-fast [**NVMe**](https://en.wikipedia.org/wiki/NVM_Express) solutions we rely on today? Since the dawn of computing, storage has been both a fundamental challenge and a catalyst for technological advancement. Early systems were constrained by **expensive hardware** and **limited capacity** - so engineers turned to [Redundant Array of Independent Disks (**RAID**)](https://en.wikipedia.org/wiki/RAID) to increase **reliability**, **availability**, and **performance**. By uniting multiple hard drives into a single logical unit, RAID laid the groundwork for more robust and fault-tolerant storage architectures.

As demand for speed and efficiency soared, [Solid-State Drives (**SSDs**)](https://en.wikipedia.org/wiki/Solid-state_drive) heralded a major breakthrough with their **superior data access**, **lower latency**, and **improved durability**. The unceasing pursuit of higher performance then inspired the creation of Non-Volatile Memory Express (**NVMe**), a protocol that capitalizes on [**high-speed PCIe connections**](https://en.wikipedia.org/wiki/PCI_Express). This development propelled storage technology into a new era of capacity, throughput, and reliability — one that continues to evolve today.

# Modern storages

When you think about the countless apps, services, and systems in use today, all of them rely on one unifying element: [**storage**](https://en.wikipedia.org/wiki/Data_storage). It’s the bedrock that preserves the “[**state**](https://en.wikipedia.org/wiki/State_(computer_science))” of any application or platform, enabling everything from tiny web services to massive enterprise data centers. Building on the foundations of RAID, SSDs, and NVMe, today’s storage ecosystem has evolved into a diverse toolkit designed to meet every conceivable need. Whether you’re working with [**object storage**](https://en.wikipedia.org/wiki/Object_storage) for unstructured data, [**block storage**](https://en.wikipedia.org/wiki/Block_(data_storage)) for virtual machines, [**file storage**](https://en.wikipedia.org/wiki/File_system) for shared directories, or one of the many flavors of [**databases**](https://en.wikipedia.org/wiki/Database) - **[SQL](https://en.wikipedia.org/wiki/SQL), [NoSQL](https://en.wikipedia.org/wiki/NoSQL), or distributed** - you’re tapping into decades of innovations in performance and reliability. Even [**data warehouses**](https://en.wikipedia.org/wiki/Data_warehouse) that drive analytics at scale and [**queue systems**](https://en.wikipedia.org/wiki/Message_queue) that orchestrate event-driven architectures owe their existence to these foundational breakthroughs. This talk will explore how the remarkable ways data is stored, managed, and transformed today.

# Designing the Nearby Friends application

> System design is a structured process for planning and implementing software solutions that meet user needs while accommodating **growth**, **performance**, and **security** considerations. It involves translating **requirements** into a cohesive **architecture**, determining how to break the system into logical **components**, choosing appropriate **data stores** (relational vs. NoSQL), and selecting **communication** protocols (REST, gRPC, etc.). Each decision carries its own trade-offs around **cost**, **scalability**, **complexity**, and **reliability**.

Imagine you are a software engineer at a big tech company. You’ve been presented with an exciting challenge: **implement a Nearby Friends feature** in an existing messaging application. This functionality must aggregate and display real-time location data for users who have opted in and granted permission. The system must be robust enough to handle large volumes of updates, efficient enough to provide near-instant feedback to users, and secure enough to protect sensitive location data.

## Functional requirements

* **User Visibility**: Users should be able to see a list of nearby friends on their mobile apps.
* **Distance & Timestamp**: Each friend in the list displays a distance value and a timestamp indicating when that distance was last updated.
* **Frequent Updates**: The nearby friends list should refresh every few seconds to maintain up-to-date location information.

## Characteristics to choose from

| Characteristic             | Description                                                                                                                                                                     |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| performance                | The amount of time it takes for the system to process a business request.                                                                                                       |
| responsiveness             | The amount of time it takes to get a response to the user.                                                                                                                      |
| availability               | The amount of uptime of a system; usually measured in 9's (e.g., 99.9%).                                                                                                        |
| fault tolerance            | When fatal errors occur, other parts of the system continue to function.                                                                                                        |
| scalability                | A function of system capacity and growth over time; as the number of users or requests increase in the system, responsiveness, performance, and error rates remain constant.    |
| elasticity                 | The system can expand and respond quickly to unexpected or anticipated extreme loads (e.g., going from 20 to 250,000 users instantly).                                          |
| data integrity             | The data across the system is correct and there is no data loss in the system.                                                                                                  |
| data consistency           | The data across the system is in sync and consistent across databases and tables.                                                                                               |
| adaptability               | The ease in which a system can adapt to changes in environment and functionality.                                                                                               |
| concurrency                | The ability of the system to process simultaneous requests, in most cases in the same order in which they were received; implied when scalability and elasticity are supported. |
| interoperability           | The ability of the system to interface and interact with other systems to complete a business request.                                                                          |
| extensibility              | The ease in which a system can be extended with additional features and functionality.                                                                                          |
| deployability              | The amount of ceremony involved with releasing the software, the frequency in which releases occur, and the overall risk of deployment.                                         |
| testability                | The ease of and completeness of testing.                                                                                                                                        |
| abstraction                | The level at which parts of the system are isolated from other parts of the system (both internal and external system interactions).                                            |
| workflow                   | The ability of the system to manage complex workflows that require multiple parts (services) of the system to complete a business request.                                      |
| configurability            | The ability of the system to support multiple configurations, as well as support custom on-demand configurations and configuration updates.                                     |
| recoverability             | The ability of the system to start where it left off in the event of a system crash.                                                                                            |
| feasibility (implicit)     | Considering timeframes, budgets, and developer skills when making architectural choices; tight timeframes and budgets make this a driving architectural characteristic.         |
| security (implicit)        | The ability of the system to restrict access to sensitive information or functionality.                                                                                         |
| maintainability (implicit) | The level of effort required to locate and apply changes to the system.                                                                                                         |
| observability (implicit)   | The ability of a system or a service to make available and stream metrics such as overall health, uptime, response times, performance, etc.                                     |

--- 

# Meet your hosts

<div align="center">
<table style="width:100%; margin-bottom: 1em;">
  <tr>
    <td>
      <strong>Michal Łukowicz</strong><br>
      <em>Fellow DevOps Engineer</em><br>
      Bio
    </td>
    <td align="left" style="width:120px;">
      <img 
        src="https://drive.google.com/uc?export=view&id=1e56uM4XRdFCvmA64YeWi5cVVduVGBKFm"
        alt="Michal Łukowicz" 
        width="100" 
        style="border-radius: 50%;" 
      />
    </td>
  </tr>
</table>
<table style="width:100%; margin-bottom: 1em;">
  <tr>
    <td align="left" style="width:120px;">
      <img 
        src="https://substack-post-media.s3.amazonaws.com/public/images/4d17c584-3500-4a83-9db9-f826c356ee62_2000x2000.png" 
        alt="Jakub Słyś" 
        width="100" 
        style="border-radius: 50%;" 
      />
    </td>
    <td>
      <strong>Jakub Słyś</strong><br>
      <em>Senior Principal Software Engineer</em><br>
      Bio
    </td>
  </tr>
</table>
</div>
