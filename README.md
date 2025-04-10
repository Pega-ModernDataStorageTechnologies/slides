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
* Wrap-Up

## Schedule

| Time (Approx.) | Activity |
| -------------- | --------------------------------------- |
| 0:00 - 0:20    | Short intro & ice breaker |
| 0:20 - 0:40    | Historical overview |
| 0:40 - 1:00    | Modern storages |
| 1:00 - 2:40    | Designing the **Nearby Friends** application |
| 2:40 - 3:00    | Summary & Closing Remarks |

# Storage historical overview and its evolution

Have you ever wondered how our data storage capabilities transformed from bulky magnetic **tapes** and basic hard disk drives (**HDDs**) to the lightning-fast **NVMe** solutions we rely on today? Since the dawn of computing, storage has been both a fundamental challenge and a catalyst for technological advancement. Early systems were constrained by **expensive hardware** and **limited capacity** - so engineers turned to Redundant Array of Independent Disks (**RAID**) to increase **reliability**, **availability**, and **performance**. By uniting multiple hard drives into a single logical unit, RAID laid the groundwork for more robust and fault-tolerant storage architectures.

As demand for speed and efficiency soared, Solid-State Drives (**SSDs**) heralded a major breakthrough with their **superior data access**, **lower latency**, and **improved durability**. The unceasing pursuit of higher performance then inspired the creation of Non-Volatile Memory Express (**NVMe**), a protocol that capitalizes on **high-speed PCIe connections**. This development propelled storage technology into a new era of capacity, throughput, and reliability — one that continues to evolve today.

# Modern storages

When you think about the countless apps, services, and systems in use today, all of them rely on one unifying element: **storage**. It’s the bedrock that preserves the “**state**” of any application or platform, enabling everything from tiny web services to massive enterprise data centers. Building on the foundations of RAID, SSDs, and NVMe, today’s storage ecosystem has evolved into a diverse toolkit designed to meet every conceivable need. Whether you’re working with **object storage** for unstructured data, **block storage** for virtual machines, **file storage** for shared directories, or one of the many flavors of **databases** - **SQL, NoSQL, or distributed** - you’re tapping into decades of innovations in performance and reliability. Even **data warehouses** that drive analytics at scale and **queue systems** that orchestrate event-driven architectures owe their existence to these foundational breakthroughs. This talk will explore how the remarkable ways data is stored, managed, and transformed today.

# Designing the Nearby Friends application
> System design is a structured process for planning and implementing software solutions that meet user needs while accommodating **growth**, **performance**, and **security** considerations. It involves translating **requirements** into a cohesive **architecture**, determining how to break the system into logical **components**, choosing appropriate **data stores** (relational vs. NoSQL), and selecting **communication** protocols (REST, gRPC, etc.). Each decision carries its own trade-offs around **cost**, **scalability**, **complexity**, and **reliability**.

Imagine you are a software engineer at a big tech company. You’ve been presented with an exciting challenge: **implement a Nearby Friends feature** in an existing messaging application. This functionality must aggregate and display real-time location data for users who have opted in and granted permission. The system must be robust enough to handle large volumes of updates, efficient enough to provide near-instant feedback to users, and secure enough to protect sensitive location data.

## Functional requirements
* **User Visibility**: Users should be able to see a list of nearby friends on their mobile apps.
* **Distance & Timestamp**: Each friend in the list displays a distance value and a timestamp indicating when that distance was last updated.
* **Frequent Updates**: The nearby friends list should refresh every few seconds to maintain up-to-date location information.

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
    <td align="right" style="width:120px;">
      <img 
        src="https://1drv.ms/i/c/c525bab12e40b0f3/IQRl57PRSj7nQ4pVMnbJtQyVAVfxCahSgrcctLJ15zTt1gU?width=1024"
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
