# Student Robotics Dev Team Proposal

This document aims to solve the important issue of development by outlining the formation of a number of smaller sub-groups within Student Robotics:
- The Development Coordination Team.
- A number of _project groups_.

## The Development Coordination team

The Development Coordination team (a.k.a. the _Dev Team_) is a group of volunteers that are chosen annually in a similar fashion to the formation of the _Core Team_, although they may be responsible for projects beyond the annual timescale.

The goals of the _Dev Team_ are to ensure the long-term longevity of Student Robotics by organising projects that enhance the experience for SR’s competitors and volunteers in line with its values, and enable SR’s long term growth. Additionally they will aim to fulfill the values of Student Robotics, in particular our goal of reflecting reality by incorporating the latest technology whenever feasible.

## Project Groups

A _project group_ is a smaller group of self-selected volunteers who have a particular interest in working on something together. The _project group_ should report progress regularly to the _Dev Team_. The _Dev Team_ oversees the various _project groups_ to ensure that they are on track and aligned with the goals of the charity. _Project groups_ are responsible for maintaining projects that they have.

### Formation of a Project Group

A group of volunteers decides that they would like to work on a project. They communicate their ideas to the _Dev Team_ and the _Dev Team_ will decide whether the project is beneficial to the organisation. A schedule for the project will be discussed between the _Dev Team_ and the _project group_. A _project group_ may apply to the _Dev Team_ for budget for specific purchases for their project, given sufficient justification. The _Dev Team_ should also keep in mind the future needs of _project groups_ when planning their budget.

Alternatively, the _Dev Team_ may identify the need for a project within the organisation and will find interested volunteers to form a group to do the project.

## Budgeting

The _Dev Team_ is allocated a budget, to be agreed with the Trustees. The scope of this budget is to cover costs incurred for development activities only, and not the cost of deploying any completed projects which would be arranged between the trustees and _Core Team_.

For the purposes of budgetary accountability, the _Dev Team_ will select a Chair and Treasurer. (How the budget is managed is between the _Dev Team_ and the Trustees.) In practice, unlike the _Core Team_ budget which is fairly detailed (e.g. £x on Kickstart, £y on Competition, £z on other) and is approved in advance, _Dev Team_ purchasing will be defined at a higher level (maybe some “infrastructure” budget for a dev server and some dev tools but not £a for Project A, £b for Project B. Unlike the _Core Team_, this will not be a rolling budget, but a “pot” that gets topped up in each accounting period to allow for projects to be budgeted over multiple years.

## Accountability

1. Much like _Core Team_, minutes and reports from the _Dev Team_, and its various sub-groups will be available to view by the general public. Sensitive data, such as budgeting, may be exempt from this.
2. The _Dev Team_ will submit regular progress reports to the Trustees.
3. As well as regular volunteers, the _Dev Team_ may contain trustees and members of the _Core Team_, however volunteers should bear in mind any potential conflicts of interest that may arise as a result of this.
4. Members of the _Dev Team_ should abstain from financial decisions where they are directly involved with the _project group_ of concern. In an event when all members of the _Dev Team_ have to abstain, the decision should be passed to the _Core Team_ or Trustees.
5. The _Dev Team_ is responsible for the oversight of the various project groups within Student Robotics. The _project groups_ should report their progress regularly to the Dev Team.

## Relationship to the Core Team

- The _Dev Team_ is independent from the _Core Team_, but will work closely with them in certain situations.
- The _Core Team_ will also communicate priorities for projects to be completed by the next competition cycle. In the event of a Kit Deployment, the _Core Team_ is responsible for budgeting, manufacture, deployment and testing.

## Getting Things Done

For new projects, there is a process to follow to ensure they receive sufficient review and testing before they are implemented. This is shown in the examples below.

For each _project group_ it is recommended that a “Project” is opened and actively maintained with high-level progress updates in the `srobo` GitHub organisation - even the “nice to haves” - if there are good ideas being worked on which get parked here, at least there will be some documentation to pick up on.

Examples of what may be in scope for SR2020: Python 3, new brain board, new IDE.

### Project of significant impact: New brain board

- A group of volunteers decide they’d like to work on finding a new single board computer which can serve as the brain board, and port/upgrade software to work on it.
- New / Updated ticket in srobo/dev-tasks.
- The volunteers develop a brief specification, including information like:
    - Functional requirements (e.g. compatible with the rest of the kit, can be powered from Power Board, runs our API, camera isn’t made slower, form factor)
    - Scope (e.g. excludes any changes to modular kit or API, independent of Python 3 project)
    - Deliverables (e.g. Board, Software, Documentation for students and volunteers)
    - Testing requirements (e.g. is demonstrated to run a defined piece of software on a test robot without fault, with a certain response time for libkoki markers, etc.)
- The _Dev Team_ may also define some limits, such as:
    - Cut-off date for deployment at SR2020
    - Cost per unit limit
    - Evidence shown that more than one board has been considered
- The _Dev Team_ may consult the _Core Team_ or Trustees to assist them with requirements. For example, in the case of a Project that would have a high implementation cost, the _Dev Team_ would need to communicate the feasibility of it with the Trustees.
- This specification is presented to and ratified by the _Dev Team_ (either on the _Dev Team_ mailing list or at a _Dev Team_ meeting)
- Development work happens.
- If changes to the specification are needed, these can be discussed with the _Dev Team_.
- Development reaches a point where the project group is happy the work is done and is shippable.
- _Dev Team_ reviews the equipment against the agreed specification and decides whether to recommend it to the _Core Team_.
- The process is now passed onto the _Core Team_ who are responsible for deciding when and how to deploy it (e.g for SR 2020).
    - If it meets the needs of the competition, it is the _Core Team_’s responsibility to ensure new kit is purchased, tested and deployed (although it’s likely to be the _project group_ who do this).
    - If it doesn’t, the _Core Team_ must decide whether to proceed anyway at risk, or to continue with the existing kit and pause expansion.

### Project of minor impact: Addition to the API (e.g. making an “R.ruggeduinos[0].PWM()” )

As this is notionally a simpler thing, but still in scope as it impacts the competition cycle, the process can be simpler.

- Developer wants to add the feature and contacts the appropriate _project group_ or creates one if it does not exist.
- The _project group_ determines that there is no need for a specification due to minor impact.
    - A change of minor impact does not have significant cost or change to the working of the competition.
    - The _Dev Team_ may determine that a project is of minor impact and require a specification.
- Developer updates/opens a new ticket in the appropriate GitHub Project.
- The _project group_ will define testing and documentation requirements.
- Developer submits a pull request. 
- The _project group_ checks it meets the requirements and approves or rejects.
- The _Dev Team_ will review the new version and decides whether to recommend it to the _Core Team_.
- Software may be continuously developed throughout the competition, but it only deployed at the discretion of the _Core Team_. The _Core Team_ may choose to not upgrade software or equipment if it is not deemed beneficial.
- When deploying, the _Core Team_ will update the kit to use the latest stable version of the software.
