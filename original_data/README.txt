Last update: 18.04.2019


# Dataset description

This dataset contains the issue reports from 8 different open source projects. The dataset provides a wide range of possible
scenarios in terms of project domain, number of issues, and developer experience. The open source projects included in the dataset are: 
* Aptana Studio (APSTUD), a web development IDE; 
* Dnn Platform (DNN), a web content management system; 
* Apache Mesos (MESOS), a cluster manager; 
* Mule (MULE), a lightweight Java based enterprise service bus and integration platform; 
* Sonatype’s Nexus (NEXUS), a repository manager for software artifacts required for development;
* Titanium SDK/CLI (TIMOB), an SDK and a Node.js based command-line tool for managing, building, and deploying Titanium projects; 
* Appcelerator Studio (TISTUD), an Integrated Development Environment (IDE); 
* Spring XD (XD), a unified, distributed, and extensible system for data ingestion, realtime analytics, batch processing, and data export. 

The dataset consist of four files:
* ```jiradataset_issues.csv``` contains data about the issue reports of all the projects.
* ```jiradataset_changelog.csv``` contains data about the changes made to the issue reports of all the projects.
* ```jiradataset_developers.csv``` contains data about the users (assignees, reporters, creators).
* ```jiradataset_sprints.csv``` contains data about the sprints and their dates.

The file ```jiradataset_issues.csv``` has the following fields:
* fields.assignee.name : Name of the user who has been assigned to the issue.
* fields.components: The list of software components related to the issue. 
* fields.created: Date when the issue was created.
* fields.creator.name: Name of the user who has created the issue.
* fields.description: Textual description of the issue, usually the body of the issue report.
* fields.fixVersions: Versions that are fixed by the issue.
* fields.issuetype.name: The type of issue report (e.g Bug, Story, Improvement, Task)
* fields.issuetype.subtask: The field indicates if the task is a subtask or not.
* fields.priority.name: Textual description of the priority assigned to the issue.
* fields.reporter.name: Name of the user who has reported the issue.
* fields.resolution.description: Reason why the issue has been marked as resolved.
* fields.resolution.name: Different categories of resolution (e.g. Complete, Fixed, Invalid)
* fields.resolutiondate: Date of resolution.
* fields.status.id
* fields.status.name: String that represents the status of the issue (e.g. TODO, DOING, In Progress)
* fields.status.statusCategory.name: ?
* fields.summary: The title of the issue report. 
* fields.updated: Date of last update.
* fields.versions: List of versions affected by the issue.
* fields.watches.watchCount: Number of users watching this issue report.
* key: unique identifier of the issue report
* storypoints: number of story points estimated by the users
* project: string indicating the project of the issue.
* sprint: string indicating the sprint which the issue belongs to

The file ```jiradataset_changelog.csv``` has the following fields:
* author: Name of the user who has made the change.
* created: Date when the change has made.
* field: Field of the issue that was affected by the change.
* fieldtype: Category of the field.
* from: Internal id representing the state previous to the change.
* fromString: String indicating the state previous to t he change. 
* key: Unique indentifier of the issue affected by the change.
* project: string indicating the project of the issue.
* to: Internal id representing the state after the change.
* toString: Internal id representing the state after the change.

The file ```jiradataset_sprints.csv``` has the following fileds:
* key: Issue key
* project: Name of the project.
* sprint.completeDate: Date when the sprint was completed.
* sprint.endDate: Date when the sprint end (planned date?).
* sprint.id: Internal id of the sprint.
* sprint.name: Name of the sprint.
* sprint.startDate: Date when the sprint started (planned date?).
* sprint.state: Current state of the sprint (e.g. CLOSED, OPEN)