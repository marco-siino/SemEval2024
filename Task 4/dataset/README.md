## The Legal Argument Reasoning Task in Civil Procedure - Dataset
`Current version: 2.0.0`

This is the dataset for SemEval 2024 Task 5: Argument Reasoning in Civil Procedure

This version only contains the partitions **train** and **dev**, the **test** partition will be provided separately once the competition officially starts.

### General Information
| Column            | Train | Dev | Test | Description                                                              |
| ----------------- | ----- | --- | ---- | ------------------------------------------------------------------------ |
| idx               | ✔    | ✔   | ✔    | index                                                                    |
| question          | ✔    | ✔   | ✔    | question                                                                 |
| answer            | ✔    | ✔   | ✔    | answer candidate for question                                            |
| label             | ✔    | ✔   | ❌   | target label, answer candidate correct/incorrect = 1/0                   |
| analysis          | ✔    | ✔   | ❌   | excerpt from complete analysis relevant to answer candidate              |
| complete analysis | ✔    | ✔   | ❌   | Glannon's explanation for the solution of the question                   |
| explanation       | ✔    | ✔   | ✔    | topical introduction, additional context for question, potentially empty |


### Changes:
v 2.0.0 - 2023-07-26
- idx field moved to first column 
- datapoints from book chapter 26 have been removed, as they have been included unintentionally in version 1
- corrected missing explanation for 2 datapoints in the train partition
