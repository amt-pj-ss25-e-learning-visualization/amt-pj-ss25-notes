#### Main functionality

- **Continue within a partially completed course**  
  Recommend modules from a course where the student has already completed some content, assuming they haven't finished the course yet.

- **Recommend based on topic interest (utilizing LOM)**  
  When a student has completed several modules with specific keywords (e.g., `botanic`, `mathematics`), we assume an interest in that subject.  
  → Recommend modules from other courses that share similar subjects.  
  → Requires categorization of all modules via the "keywords"-field in the LOM metadata.

- **Review based on forgetting curve**  
  Recommend repeating previously completed modules based on a model of forgetting (e.g., the Ebbinghaus forgetting curve) to help consolidate knowledge.

The first two functions will require more synthetic courses and modules besides the current "Baumchirurg"-course. 

#### Optional

- **Review based on poor performance**  
  Recommend repeating a module if the student performed poorly (e.g., score falls below a set threshold compared to the average).
