# Kubernetes Bug Localization Replication Package
This package provides the replication data for the hybrid approach presented in our currently-under-review research paper.

## Package Detail
The package consists of two zip files: 
1. LocalizationDataset.zip and 
2. LocalizationSource.zip

### LocalizationSource.zip
This zip contains a single text file Source.txt that contains text for all source files used in the localization research. Each line represents a source file. Each line is in the following format:

<p align="center">{{File Id}}##{{Comma separated source code text}}</p>

### LocalizationDataset.zip
This zip contains 1,868 directories each representing a issue for Kubernetes. Each directories consists of four files:

1. BugReport.txt: The file contains the bug report for the issue. The bug report is split using camel-case splitter, stemmed, and stop-words removed,
2. FileList.txt: The file contains the name of all source files in the system and the custom ids (Index) generated for each,
3. RelevantList.txt: The file contains the names of the relevant files and the custom ids (Index) associated with them,
4. SourceNum.txt: The file contains the file numbers for the source files that makes up the system's source. The text content for each file can be found in Source.txt.

## Package Link
http://seel.cse.lsu.edu/data/tosem19.zip
