#### Implemented Recommenders

- **Recommend based on similar students (Jaccard Index)**  
  Recommend modules that students with a similar learning history have completed, but the current student has not.  
  → Based on overlap in completed modules across students (using statements with verb `"completed"`).  

- **Recommend based on topic interest**  
  When a student has completed several modules that belong to the same subject (e.g., `horticulture`, `it`), we assume an interest in that subject.  
  → Recommend modules from other courses that share similar subjects.  
  → Utilizes the IMS Common Cartridge element `catalog` in the manifest file of the corresponding course  
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;→Stored within column `subject` in the `courses` database table.

- **Review based on forgetting curve**  
  Recommend repeating previously completed modules based on the last module performance (assumes good score means less forgetting) and the `forgettingEffect` function that is being used for calculating the `masteryEbbinghaus` metric.
