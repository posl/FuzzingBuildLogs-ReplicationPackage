## Replication package for the paper: My Fuzzers Won’t Build: An Empirical Study of Fuzzing Build Failures

## Files
- Labeling-Results.csv: This file contains the result of the annotators' labeling process. Each project has one randomly sampled failing build log
    - Project: OSS-Fuzz project name
    - Label: Label agreed upon by the annotators
    - Url: Url to view the build log online

## Labeling Process

### Label Creation
- The annotators only created new labels when an exisiting one could not properly describe the error properly
- The new label must be as descriptive of the build failure as possible

### Labeling Methodology
1. Open the build log and search for the error(s)
2. If only a single error can be identified and is clearly described by the error message then label accordingly.
3. If multiple errors are shown in the build log, label according to the first error triggered during the build process
4. If the annotators cannot understand the error messages or cannot figure out the root cause of failures
5. The authors must look online for the error messages using resources such as stackoverflow, the official OSS-Fuzz GitHub repository and the project's repository
6. If there is still uncertainty after looking online, the authors must label as "Label as not information"

At the end of the labeling process, similar labels were merged together based on the root cause that caused the failures.
