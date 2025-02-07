# Google Summer of Code 2025

## [![Google Summer of Code 2025](https://github.com/Sing-Li/bbug/raw/master/images/gsoclogo.jpg)](https://summerofcode.withgoogle.com)

## How to apply

Rocket.Chat is applying to become a participating mentoring open source organization for [Google Summer of Code 2025](https://summerofcode.withgoogle.com/), helping to usher in a new generation of open source contributors and enthusiasts.

For timeline, see [Official Google Summer of Code 2025](https://developers.google.com/open-source/gsoc/timeline) Timeline for more details.

Almost anyone in the world [over 18 years of age](https://opensource.googleblog.com/2021/11/expanding-google-summer-of-code-in-2022.html) who loves coding and wants to explore the incredible world of open source can join us as a GSoC 2025 contributor.

Most exciting news for the 2025 season is a new [focus on ML/AI plus security projects, and the continued support for a small project type with a 90 hours duration](https://opensource.googleblog.com/2023/11/google-summer-of-code-2025-celebrating-20th-year.html); allowing participation from those who can only  devote part of their summer to exploring open source.

For details and rules of Google Summer of Code 2025, please see the [GSoC 2025 Official Website](https://summerofcode.withgoogle.com/). For timeline, see [Official Google Summer of Code 2025 Timeline](https://developers.google.com/open-source/gsoc/timeline) for more details.

### **Contacting Rocket.Chat**

For general information, please visit our 24 x 7 community channel for Google Summer of Code 2025 : [https://open.rocket.chat/channel/gsoc2025](https://open.rocket.chat/channel/gsoc2025)

Join our [Google Summer of Code 2025 Team ](https://open.rocket.chat/channel/gsoc2025) today, introduce yourself to the friendly community, and interact with over **110 like-minded** contributors/mentors (as of January 27, 2025)  and meet the team in the [20+ team channels](https://open.rocket.chat/channel/gsoc2025/team-channels).

If you have ideas and proposals that are not on our idea list, or if a mentor is not available, you can also email to:

gsoc+2025@rocket.chat

But better yet, you can post your idea in the [New GSoC 2025 Ideas looking for mentors](https://open.rocket.chat/channel/New-GSoC-2025-Ideas-looking-for-mentors) channel and possibly getting some immediate community feedback or support for your idea.

Interested contributors are also encouraged to interact directly with our team and community on the team channels:

[https://open.rocket.chat/channel/gsoc2025/team-channels](https://open.rocket.chat/channel/gsoc2025/team-channels)

As well as on GitHub:

[https://github.com/RocketChat/Rocket.Chat](https://github.com/RocketChat/Rocket.Chat)

Those who prefers forums can post messages on our GSoC forum channel (although as the leading open source team chat project we prefer you use Rocket.Chat channels above to reach us instantly).

-----

### **Latest update**

As of January 27th 2025  checkout our [GSoC 2025  Contributors Leaderboard](https://gsoc.rocket.chat/), to see the amazing contributions by our GSoC 2025 community: we already have over 100 contributors and mentors ready to join us for this season, active in our [team channels](https://open.rocket.chat/channel/gsoc2025/team-channels).

## 📂 Project Ideas

> This is an early draft of the GSoC 2025 project ideas list for Rocket.Chat,  the projects are expected to go through constant rapid changes during the application period - as mentors and potential contributors discuss and evolve the project descriptions.



### 📅  Message Timestamp Date Picker Components

👥 **Mentor(s):** [Martin Schoeler](https://open.rocket.chat/direct/martin.schoeler)

💬 **Description:**
Currently Rocket.Chat has a feature that allows users to send timestamps on messages, but not in an intuitive way. To send a timestamp you need to manually write it down with the correct date code. For example `<t:1732557600:t>`.
This feature was added for Rocket.Chat Apps engine, but users can benefit from this too. The objective of this project is to create a new `MessageToolBar` item that displays a calendar and let the users select the date and time they would like to share, both in the desktop app and mobile apps.

Some examples of the usage of the timestamp feature (you can test them today on the open.rocket.chat server!)

Pattern: <t:{timestamp}:?{format}>

- {timestamp} is a Unix timestamp
- {format} is an optional parameter that can be used to customize the date and time format.

**Formats**

| Format | Description               | Example                                 |
| ------ | ------------------------- | --------------------------------------- |
| `t`    | Short time                | 12:00 AM                                |
| `T`    | Long time                 | 12:00:00 AM                             |
| `d`    | Short date                | 12/31/2020                              |
| `D`    | Long date                 | Thursday, December 31, 2020             |
| `f`    | Full date and time        | Thursday, December 31, 2020 12:00 AM    |
| `F`    | Full date and time (long) | Thursday, December 31, 2020 12:00:00 AM |
| `R`    | Relative time             | 1 year ago                              |

The creation of tests for the new component is also expected, both end to end and unit if applicable.

💪 **Desired Skills:** React, Typescript, React Native

🎯 **Goals/Deliverables:** A new component on the `MessageToolBar` that allows users to add timestamps to their messages, both in desktop and mobile.

⏳ **Project Duration:** 90 hours. (Small)

📈 **Difficulty:** Easy/Intermediate

-----


### 💡On-Vacation Helper App 

👥 **Mentor(s):** Jeffrey Yu

💬 **Description:**  

This LLM-powered app will suggest interesting events and happenings for users during their vacation.   

Details:

* While on vacation, a user can take a photo of his surroundings and upload it to a channel
* The app will first process the image by passing it to an image reasoning multi-modal LLM to ascertain the location or point of interest or event venue (perhaps reinforced by GPS location information).  
* Then in a second step an(other) LLM's tools/function-calling capability is used to fetch up-to-date events and happening information over the Internet, catering for the user's current interest. 
* Finally, a friendly report is produced by an(other) LLM as the last step of a RAG pipeline. 
* This app should never produce erraneous output. It should know its own limitaion and decline to report if in doubt.   


💪 **Desired Skills:**  

- Rocket.Chat Apps Engine (TypeScript)  
- Familiarity with the "RAG" agentic workflow  
- Intermediate prompt engineering Skills   
- Experience with image reasoning capabilities of modern open source multi-modal LLMs  
- Experience with tools/function-calling capabilities of modern LLMs

🎯 **Goals/Deliverables:**  

- A working Rocket.Chat App that assists users with latest happenings around them wherever they may be while on vacations. 

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Intermediate/Advanced  

-----


### 💡Embedded Chat 2025

👥 **Mentor(s):** Zishan Ahmad

💬 **Description:**

Improvement to the EmbeddedChat project this year includes:
- Upgrading the current API and auth packages to use the latest Rocket.Chat SDK packages like `ddp-client`, and aligning other components to use other abstraction provided by Rocket.Chat, ensuring these packages will be managed internally moving forward.
- Making the EmbeddedChat fully mobile-responsive for a seamless experience across all devices.
- Improving the UI and adding more customization options to enhance the user experience.

💪 **Desired Skills:**

React.Js

🎯 **Goals/Deliverables:**

- Integration of the latest Rocket.Chat SDK packages
- Fully mobile-responsive EmbeddedChat
- Improved UI with more customization options

⏳ **Project Duration:** 90 hours (Small)

📈 **Difficulty:** Easy/Intermediate

-----

### 💡 Receipts Processor and Reporting App powered by Multi-modal LLMs 

👥 **Mentor(s):** Maria Khelli

💬 **Description:**  

While attending a busy conferences or event, the need to keep track of receipts and then having to adding them up manually to fill in expense reports is a very common and tedious problem.  This project is a Rocket.Chat app that completely automate the process.   

Details:

* The user will be able to take pictures of restaurant receipts on their phone and upload it into a specific channel (representing a single event, duration of time, or trip, and so on...).  

* Upon request, the app should  read and sum all the receipts producing a detailed report.  Ideally, the input format and image size should be flexible and the report format should be customizable via templates.  

* The app should never produce erraneous result under any circumstances, it should be able to recognize its limitation and decline to complete the task instead of giving potentially erraneous output.  

💪 **Desired Skills:**  

- Rocket.Chat Apps Engine (TypeScript)  
- Intermediate prompt engineering Skills   
- Experience with image reasoning capabilities of available open source multi-modal LLMs  


🎯 **Goals/Deliverables:**  

A working Rocket.Chat app that will scan and sum all the restaurant receipts uploaded to a specific channel.

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Easy/Intermediate  

-----

### 💡End to End Encrypted Message Handling for Ruqola on KDE

👥 **Mentor(s):** [Montel Laurant](https://github.com/Montel),  Aaron Ogle  

💬 **Description:**  

Add end to end encrypted message feature to the [Ruqola client](https://github.com/KDE/ruqola) on KDE.  Ruqola is the de-facto standard Rocket.Chat client running on KDE.   This project will be co-mentored by an expert mentor from KDE.

Details:
- some UI elements to handle E2E encrypted messages is already in place
- careful consideration for key management is essential to a successful implementation
    - how does the user get the key?  what happens when he/she loses the key?  
    - what UI is needed to support re-generation of key?
    - how does one display a channel with messages that may be encrypted by different keys? 

💪 **Desired Skills:**  
- Rocket.Chat API programming (REST and DDP) 
- Solid experience with C++ programming
- Experience with large and complex C++ projects
- Working experience with KDE on Linux (such as kubuntu) 
- Ideally already user of Ruqola

🎯 **Goals/Deliverables:**  
Add support for E2E Encrypted messages in Ruqola.

⏳ **Project Duration:** 175 hours (Medium)  

📈 **Difficulty:** Advanced  

----

### 💡 AI Docs Assistant App

👥 **Mentor(s):** [Dnouv](https://open.rocket.chat/direct/evan.shu)  

💬 **Description:**  

This project aims to build a Rocket.Chat App that provides a **natural language interface** for querying Rocket.Chat Docs (docs.rocket.chat). Instead of manually searching for answers, users can simply ask the app, and it will return a **relevant, structured response** based on the documentation.  

Key Features:  

- **Retrieval-Augmented Generation (RAG)** approach to search and retrieve a summary of docs.    
- **Local embedding model** (running on CPU) to generate query representations.  
- **In-memory vector store** to efficiently match queries to relevant documentation.  
- **Context-aware responses** to handle follow-up questions naturally.
- (Exploration) **Graph** mapping the relationships between different pages, the LLM maps through the relationship edges, chooses the nodes related to the user query, and calls Web APIs to fetch those pages. 
- **Tool Calling** to retrieve the latest page contents from Web 

💪 **Desired Skills:**  

- Rocket.Chat Apps Engine (TypeScript)  
- Natural Language Processing (NLP)  
- Vector search (HNSW, LSH, or similar techniques in JS)  
- Web Storage & IndexedDB (for caching, if needed)
- Web Search APIs
- (Exploratory) Familiarity with Graph Theory

🎯 **Goals/Deliverables:**  

- A Rocket.Chat App that enables users to query Rocket.Chat Docs via natural language.  
- **Efficient RAG-based retrieval** with an in-memory vector store. 
- A **lightweight, CPU-friendly embedding model** for query similarity matching.  
- **Interactive chat interface** that tracks context for follow-up queries.
- **Graph-Based Document Mapping (Exploratory):**
  - Builds a graph where nodes represent documentation pages and edges represent semantic or topical relationships.
  - Supports multi-hop reasoning by guiding the retrieval process through related content.
  - In certain scenarios can complement embedding-based retrieval by providing explicit structural context.
 

**Scenario:**

A user inquires, "How do I configure MongoDB for Rocket.Chat?"

**Graph-Based Approach:**

1. **Graph Construction:**
   - **Nodes:** Each documentation page is a node.
   - **Edges:** Connections between nodes represent relationships, such as prerequisites or related topics.

   For instance:
   - **Node:** "Deploy Rocket.Chat"
   - **Node:** "Setup and Configure"
   - **Node:** "MongoDB Configuration"
   - **Edges:** "Deploy Rocket.Chat" → "Setup and Configure" → "MongoDB Configuration"

2. **Query Processing:**
   - The system identifies the "MongoDB Configuration" node as directly relevant to the user's query.

3. **Graph Traversal:**
   - The system traverses to connected nodes to gather additional context, such as "Setup and Configure," ensuring comprehensive information retrieval.
  
4. **Call Web Tool:**
    - The system calls the web to fetch the latest docs page to generate an answer
  
 
**Embedding-Based Approach:**
1. The system identifies the top relevant doc sources based on the summary of stored pages
2. The system calls the Web tool to fetch the latest doc
3. Generate an answer

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Intermediate/Advanced  

---

### 💡Google Summer of Code Community Hub 2025

👥 **Mentor(s):** Ashutosh Singh Chauhan

💬 **Description:**  

Continuing our work on a "full stack component framework" in which a scalable website can be created by non-technical users using drag-and-drop components that not only include UI and client-side logic, but also pre-scaled server-side behaviors (or serverless impl). 

The ultimate use-case we have been working on is the community hub for Rocket.Chat Google Summer of Code. It will link all the despearate servers into one easy to customize and maintain uniform scalable web app (comprise of a set of full-stack components).

This year's work will include:
- rebasing of the existing platform and components on Svelte 5
- moving the WYSIWYG "Syntax Sweetening" work done last year to this new platform
- implementation of auth via OIDC
- migrate over the event poster component (used for our demo day)
- migrate over the video-meet-your-mentor component
- implement the gsoc leaderboard component
- implement embeddedchat component

💪 **Desired Skills:**  

- Advanced Typescript
- Svelte 5
- AST concepts  

🎯 **Goals/Deliverables:**  

A functional community hub website that we will use for 2026; showcasing the platform and new components.  

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Easy/Intermediate  

---


### 💡AI Chat Workflows Automation App with multi-step reasoning

👥 **Mentor(s):**  Hardik Bhatia

💬 **Description:**  

Build a Rocket.Chat app that will monitor messages in specified channels (possibly sent by specified individuals, possibly within certain specified time period, and so on... )  and then (as a second step) perform additional messaging operations based on those messages.  Command should be issued in simple English. Bonus point for more than 2 steps in the reasoning.

Some examples:

    "whenever @sing.li posts any welcome messages in #gsoc2025, immediately DM him with a thank-you note"

    "if any picture is uploaded to the #pets channel, send a message that says meow! if the pet is a cat, and a woof! otherwise"

    "whenever a message is posted that contains a four letter word beginning with letter F, delete that message immediately"

    "if my wife messaged with 'arrived' before I do, DM her sorry I will be late after 1 minute" 

Recommended approach:

- leverage the latest open source specialized multi-step reasoning LLMs such as the DeepSeek distilled models 
- make intelligent use of tools/function-calling and structured inference    
- be sure to built in safety to offset erraneous output and/or hallucinations 

💪 **Desired Skills:**  

- Rocket.Chat Apps Engine (TypeScript)  
- Rocket.Chat messaging APIs
- Advanced prompt engineering Skills   
- Experience with image reasoning capabilities of available open source multi-modal LLMs
- Experience working with multi-step reasoning LLMs
- Experience with tools/function-calling capabilities of modern LLMs
- Expereince with code generation and code completion LLMs
- Understanding of how to implement "safety first" when creating AI apps that may permenantly change the state of a production system

🎯 **Goals/Deliverables:**  

Platform for generating functional automated chat workflows using LLMs.

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Intermediate/Advanced  


---

### 💡On-device client side LLM inference and API Access Enablement 

👥 **Mentor(s):** Sing Li

💬 **Description:**  

Analyze and modify current deployment workflows for Rocket.Chat to enable browser based client-side on-device LLM inference.  

Details:

- high performance lightweight models became available in second half of 2024, making on-device inference possible  (requiring about 2GB additional memory and GPU on client)
- webgpu and webllm technology matured and now in-browser inference and LLM API access is a practicing reality
- Rocket.Chat administrators/installers should be able to OPTIONALLY enable client-side inference
- on-device/client-side implementation should detect device capabilities before downloading the LLM weights; only enabling it if there is enough compute and memory available on the client 

💪 **Desired Skills:**  

- Rocket.Chat Deployment Flows
- DevOps: docker, helm, snaps, and so on. 
- Advanced Typescript
- Awareness of WASM and webllm 
- Python 

🎯 **Goals/Deliverables:**  

Ability to deploy client-side/on-device in-browser LLM for rapid development and efficient scaling of AI apps.

⏳ **Project Duration:** 90 hours (Small)  

📈 **Difficulty:** Advanced  

---
