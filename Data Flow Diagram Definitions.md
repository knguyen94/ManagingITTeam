# Data Flow Diagram Definitions

## ENTITIES

External Repository - External locations of source code. This could include public and private repositories outside of the control of the organization. This could also include software received via software supply chains.

Corporate Managers - Internal corporate individuals who will be the recipients of the external software manifests. From these manifests, they can make corporately impactful decisions. However, these decisions are beyond the scope of the current system.

National Vulnerability Database - Stores software vulnerability information

NIST Database - Online database that stores vulnerability information

Source Code Database - Online database that containes source code information

Policy Document Database - Contains policy document information

Interweb - Internet

## DATA FLOWS

Source Query - Internally initiated request for external source

File - Source file

Package - Source package comprised of one or more files

Package Query - Grouping of packages

File SHA1 - Hash of file

File SHA1 Response - A yes/no response as to whether or not the hash of a file exists in the database.

File Copyright/License + Info - For any file that does not have a SHA1 in the database, a new record is created for that file.

Project Query - Request for software project

Project Info - Relevant information about a project. This includes copyright, license, and vulnerability information.

CPE Information - Downloadable file within the NIST database

License Info - License information received from FOSSology

CPE Info - Standardized method of describing and identifying classes of applications, operating systems, and hardware devices.

CPE Request - Prompt for CPE information

CPE Response - Response to prompt for CPE information

## DATA STORES

Risk Information - This is the database that is going to store information about files. This information is going to have to be stored in a standardized way.

NIST CPE Information - Database that provides vulnerability information

## PROCESSES

License Scanner - Provides license information for package uploads

Scan Code
- Initial Query
- SHA1 lookup (caching)
- File packaging
- Scanning for license and copyright
- Vulnerability look up
- Weakness look up
- Database writing

Create Project Information - Received provided project information and assemble and return discovered software license, copyright, vulnerability, and weakness information.

CVE Lookup - Receives CPE information and returns CVE information

Post Code Change Information - Receives package list from manager and sends license information to developer.

Policy Document Information - Receives policy document request, sends request to policy document database, receives policy document information, and returns policy document response to manager.

Source Code Lookup - Receives package request from developer, sends package information to source code database, receives source code information, and returns modified package to developer.

Post Source Code - Receives modified package from developer and posts modified package to interweb.
