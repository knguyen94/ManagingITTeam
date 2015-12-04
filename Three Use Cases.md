This is the list of use cases.

Use Case 1
  ●	Title: Determine License and Vulnerability Information
  ●	Primary Actor: Corporate Manager
  ●	Goal in Context: The corporate manager is able to determine license and vulnerability information from provided project information
  ●	Stakeholders:
    ○ Corporate Manager: To receive clear and relevant project information
    ○	Corporate Developer: To provide the relevant file/package level information
    ○ Project Owner: To clearly understand corporate manager decisions to green/red light a project
  ●	Preconditions:
    ○	Relevant file/package information is in the SPDX database
    ○	Proper project information has been provided
  ●	Main Success Scenario: Corporate manager receives inaccurate or invalid license and vulnerability information for the requested project packages
  ●	Trigger: Corporate manager uploads or identifies project information to which license and vulnerability information is provided
  

  
//Edited by Justin, 12/4
Use Case 2
  ●	Title: Create Repository
  ●	Primary Actor: Corporate Developer
  ●	Goal in Context: Corporate Developer creates repo for the use of open source.
  ●	Stakeholders:
    ○ Corporate Manager: To receive clear and relevant project information
    ○	Corporate Developer: Set aside time and/or resources to create the repo.
    ○ Project Owner: To clearly understand the use of the repo so it is properly managed
  ●	Preconditions:
    ○	Relevant file/proper information to be put in repo unless left blank initially.
  ●	Main Success Scenario: Repository is properly created for use. 
  ●	Trigger: Approval to create repo from corporate manager.

Use Case 3
  ●	Title: Install database software.
  ●	Primary Actor: Corporate developer
  ●	Goal in Context: 
  ●	Stakeholders: Create/setup system system to handle database
    ○ Corporate Manager: To receive clear and relevant project information
    ○	Corporate Developer: To provide the relevant file/package level information
    ○ Project Owner: To clearly understand corporate manager decisions to green/red light a project
  ●	Preconditions:
    ○	System be Linux based or Windows based. Linux is prefered becasue it is free and supports many toos for the task. 
    ○	If Linux is decided use Ubuntu, FreeBSD, or CentOS.
    ○	Repository installed on system.
    ○ Ability ot run root commands on system.
    ○	System must have internet access capabilities.
    ○	 Must have database software installed on system. 
  ●	Main Success Scenario: System now capable of creating/mangaging database adn can be checked for vulnerabilities
  ●	Trigger: Approval to install system from corporate manager.
