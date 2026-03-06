# **File Analyzer** 

### Project Overview



File Analyzer is an Android-based cybersecurity application designed to analyze different types of files and detect potential malicious content using static analysis techniques. The application allows users to upload and scan files such as APKs, documents, images, audio, and video files. It evaluates the files using hash-based malware detection and provides security insights to the user.The system aims to improve mobile security by allowing users to verify whether files received from external sources are safe before opening or installing them.



#### Problem Statement



Mobile users frequently download and receive files from unknown or untrusted sources such as messaging apps, email attachments, or third-party downloads. These files may contain malicious code, malware, or harmful scripts that can compromise the device security and user data.

Currently, many users do not have access to lightweight tools that can quickly analyze files directly on their mobile devices.

The File Analyzer application solves this problem by providing an easy-to-use mobile solution for scanning and analyzing files before they are used.



#### Objectives



The main objectives of the project are:



To develop an Android application capable of scanning multiple file formats.

To perform static analysis on files to detect malicious content.

To provide real-time feedback on whether a file is safe or potentially harmful.

To generate scan reports for user reference.

To notify users when suspicious files are detected.

### 

### Key Features



1\. Multi-File Type Support



The application can analyze multiple file formats including:



APK files

PDF documents

Word documents

Images

Audio files

Video files

Other generic file formats



2\. Static Malware Analysis



The system performs static file analysis, which means it inspects files without executing them. This helps detect threats safely.



3\. SHA-256 Hash Detection



Each file is converted into a unique SHA-256 hash which is compared against a database of known malicious hashes.



4\. Malware Hash Database



A local database containing known malicious hashes is used to determine whether the scanned file is safe or malicious.



5\. Scan Result Display



After scanning, the system displays:



File status (Safe / Malicious)

Scan completion status



6\. Downloadable Scan Report



Users can generate a report that contains the scan results and file information.



7\. Background Notification Agent



A background service monitors scanning activities and notifies the user when suspicious files are detected.



#### System Architecture



The application architecture consists of the following components:



User Interface

Allows users to upload files

Displays scan results

File Scanner Engine

Performs static file analysis

Generates file hash values

Hash Checker

Compares generated hash with malicious hash database

Local Hash Database

Stores known malicious file signatures

Report Generator

Generates scan reports

Notification Service

Alerts users about suspicious files



#### Technologies Used



Android Studio     -	Application Development

Kotlin	           -    Programming Language

XML	           -    User Interface Design



#### Functional Requirements



The system should allow users to select files from the device.

The application should support scanning multiple file types.

The system should generate SHA-256 hash values for files.

The application should compare file hashes with the malicious database.

The system should display scan results to the user.

The system should generate downloadable scan reports.

The application should notify users if malicious files are detected.



#### Non-Functional Requirements



##### Performance



The system should perform file scanning efficiently with minimal delay.



##### Security



The application should not execute files during scanning to prevent malware activation.



##### Usability



The application interface should be simple and easy to use.



##### Reliability



The application should consistently detect malicious files based on the hash database.



#### Use Cases





##### File Upload



User selects a file from device storage.



##### File Analysis



The system analyzes the file and generates its hash value.



##### Malware Detection



The generated hash is compared with the malicious hash database.



##### Result Display



The system displays whether the file is safe or malicious.



##### Report Generation



Users can generate a scan report after analysis.



#### Advantages



Lightweight mobile malware detection system

Supports multiple file formats

Safe static analysis approach

Easy-to-use interface

Provides quick security insights





#### Future Enhancements



The following improvements can be added in future versions:



Integration with cloud malware databases

Machine learning-based malware detection

Advanced firewall protection

Integration with malware intelligence platform





#### Conclusion



The File Analyzer application provides a simple and effective solution for detecting potentially malicious files on Android devices. By using static analysis and hash-based detection techniques, the application helps users verify the safety of files before opening or installing them. This project demonstrates the application of cybersecurity principles in mobile application development.

