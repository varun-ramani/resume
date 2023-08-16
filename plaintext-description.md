# Overview
My name is Varun Ramani. I'm an aspiring software engineer.

## Education
I am about to enter my fourth year of a computer
science degree at the University of Maryland, College Park, and I have a GPA of
3.875 on a 4.0 scale. I've taken computer science coursework in algorithms,
machine learning, cryptography, compilers, networks, data structures, operating
systems, and data science. I've taken math courswork in abstract algebra, linear
algebra, calculus, number theory, statistics, and harmonic analysis.

## Experience
### Naval Research Laboratory
During my tenure spanning from May to August 2023, I undertook an internship at
the U.S. Naval Research Laboratory (NRL). Within this period, I focused on the
modernization of a critical system: a Windows Forms application implemented in
C#. This application interfaces with a C++ program operational on a dedicated
hardware "box" via TCP connections. The specific role of this C++ program
entails communication with FPGAs situated within the box. My assignment
encompassed the transformation of the existing C# application into a
contemporary manifestation utilizing web-based technologies. This endeavor
necessitated the conception, design, and implementation of a diverse array of
solutions.

To realize this evolution, I undertook a comprehensive exploration of the
prevailing landscape of web development. Subsequently, I orchestrated the
development of the web application utilizing a curated stack, including React,
Mantine, and TypeScript.

However, a pivotal distinction emerged: conventional web applications are
constrained to HTTP communication, precluding the use of TCP connections. In
light of this, I embarked on a systematic reverse-engineering process,
discerning the communication protocol employed between the C# application and
the C++ backend via Wireshark analysis. This investigation unveiled a surplus of
redundant data transmission.

Consequently, I devised a novel communication protocol founded upon HTTP
principles, thereby facilitating seamless integration with the React
application. In parallel, I architected a Rust-based server component. This
server, coexisting as a sibling process to the C++ backend on the hardware box,
assumed the role of translating and relaying messages between the two protocols,
essentially bridging the gap between HTTP and TCP communication paradigms.

Further augmenting the application's capabilities, I introduced a robust user
authentication mechanism utilizing the Department of Defense's Common Access
Cards (CAC). This feat was accomplished by harnessing Nginx to seamlessly imbue
mutual TLS (mTLS) authentication into the application. The encryption keys,
stored within the DOD CAC, were pivotal in this endeavor, enabling authorized
users equipped with CACs to effortlessly access the application.

Collaborating on the expansion of the incumbent C# application, I embarked on a
journey to comprehend both the intricacies of the C++ backend and the C#
application itself, ensuring a cohesive integration.

In addressing the inefficiencies encountered in the software development
lifecycle, particularly in relation to the C++ application, I introduced a
paradigm shift. Previously, developers were tasked with manually copying code to
a VMware image, compiling it, and then manually transferring the resulting
artifacts. In response to their concerns, I automated this process through
Dockerization. This entailed the formulation of a Dockerfile that replicated the
VMware environment, subsequently encapsulating all Docker commands within a
Python-based build system. This transformation distilled a cumbersome sequence
into a singular, streamlined command within the build system.

The same principles were applied to the web application and Rust server, with
Docker and Python-based build systems facilitating effortless generation of RPM
packages.

In anticipation of potential challenges faced by non-technical end users during
software deployment, I conceived a deployment utility leveraging Tauri, akin to
Electron. This utility empowers users to effortlessly select and install a
singular bundle provided by us, a process I aptly facilitated through the
development of the corresponding program generating the installation bundle.

### Meta
During my internship at Meta from May to August 2022, my primary task was to
enhance user privacy within the identity matching system. This involved
transitioning from plaintext user identifiers to hashed user device identifiers
by contributing to Meta's Hack codebase.

In addition to this technical upgrade, I conducted a series of experiments to
assess the impact of these changes on the existing identity matching backend. I
also developed an experimentation framework using Python, facilitating the
deployment of similar trials by other developers. This internship provided me
with valuable insights into privacy-focused technology integration and hands-on
experience in experimental design and implementation.

### Teaching Assistant
From January 2023 to May 2023, I served as a teaching assistant for Introduction
to Systems at the University of Maryland. As a TA, I led discussion sections
with up to 40 students, efficiently and accurately graded hundreds of exams and
worksheets, and mentored innumerable students in office hours for this class of
over 600 students. The section I led boasted high exam averages, and I
repeatedly received praise on my capacity for intuitively explaining complex
concepts.

From September 2022 to December 2022, I served as a teaching assistant for
Introduction to Data Science at the University of Maryland. I graded hundreds of
projects and exams, and mentored countless students in office hours.

### Undergraduate Researcher
From August 2020 to December 2021, I participated in the FIRE program at the
University of Maryland, focused on engaging freshmen in research. Within this
program, I co-created a UNet-based machine learning model for semantic
segmentation of LIDAR data. Our goal was to densely classify individual points
within a LIDAR point cloud, and we showcased our accomplishments at an
undergraduate research summit.

## Projects
### Memaid
Collaborated with a team of three to develop an
innovative dementia aid, integrating computer vision, speech-to-text, and
natural language processing (NLP) technologies. Designed to enhance memory
recall, the app swiftly learns faces upon initial encounter, linking them to
names and capturing essential conversation elements. In subsequent interactions,
the application autonomously recognizes individuals, delivering pertinent
information through connected headphones. Secured recognition among 91 competing
teams.

I personally led the integration of computer vision, speech-to-text, and NLP
functionalities. Orchestrated the design of an intuitive system that rapidly
associates faces with names. Played a pivotal role in the app's capacity to
listen, store, and recall meaningful conversational details.

We achieved top placement among 91 competing teams in a challenging contest,
securing the best hack for social good prize.

### Maskif.ai
I collaborated with a team of three peers to conceive and develop an innovative
IoT product driven by computer vision technology, aimed at enhancing
accessibility. The focal point of this endeavor was to address the challenges
posed by anti-maskers in the context of the ongoing pandemic. The resultant
product seamlessly integrates with connected smart locks and employs intelligent
detection to identify unmasked individuals approaching a door. Through this
intelligent system, the door remains securely locked when an unmasked person is
detected and automatically unlocks once they depart.

This project was selected first place against 42 other teams.

### Intellicity
As part of Intellicity's top 30 selection at PennApps 2019
(gh:varun-ramani/intellicity), I played a pivotal role in a dynamic team of
four, contributing to the creation of an advanced mobile map application. Our
collaborative effort yielded a transformative product that harnesses
crowdsourced insights and cutting-edge computer vision to enhance Google Maps
with detailed, user-contributed information. This encompasses a wide array of
data, ranging from precise geolocations of amenities like trash bins, bathrooms,
safety hazards, and parking spots. This resourceful augmentation empowers users
to navigate unfamiliar territories with utmost assurance, swiftly locating
essentials at their fingertips.

In a competitive field of 242 teams, our innovation emerged as a standout,
reflecting the potency of our solution. To bring this vision to life, I
proficiently employed Dart/Flutter for intuitive mobile development, harnessed
Python 3 for backend functionality, utilized MongoDB for efficient data
management, and leveraged Flask for seamless integration. This project
underscores my commitment to collaborative excellence and the skillful
utilization of diverse technologies to craft solutions that empower and enhance
user experiences.

## Skills
I know the following languages: Rust, Python, Java, JavaScript, TypeScript,
C/C++, Go, OCaml, Ruby, SQL, MATLAB

I know the following frameworks: Flask, React, React Native, Flutter, Keras

I know the following tooling: Git, Docker, AWS, Google Cloud Platform, Linux

I know the following libraries: pandas, NumPy, matplotlib