
# Project I - INTRODUCTION TO INFORMATICS - TBD (DCC 601)

**UFMG - 2024.2**

## SISU Data Analysis

**Submission Date:** 01/25/2024

The objective of this project is to apply the concepts of Data Science to analyze data from a sample of SISU 2021 candidates who took the ENEM exam in Brazil, using the **LEMONADE** platform. The data used for this analysis were obtained from the following URL:

[Access SISU Data](https://dadosabertos.mec.gov.br/sisu/item/206-2021-relatorio-sisu-chamada-regular-2-2021)

Students must submit a report by **01/25/2025**, presenting the results obtained along with a discussion of the analyses conducted. The report should be submitted on the Moodle platform in **PDF format only** (submissions in other formats WILL NOT be accepted). The report must include all generated graphs and analyses, screenshots of tables, and your workflow. If graphs and tables from LEMONADE are not included, a portion of the final grade will be deducted.

The data file to be used is: **SISU2021.csv**, available on the [LEMONADE Platform](https://lemonade.org.br).

---

## Data Dictionary

| **Data**                | **Field Name**          | **Data Type**    | **Description**                                                                                       |
|--------------------------|-------------------------|------------------|-------------------------------------------------------------------------------------------------------|
| **Year**                | ANO                  | Numeric          | The year of the selection process.                                                                   |
| **Institution Sigla**   | SIGLA_IES            | Alphanumeric     | Abbreviation of the higher education institution as per e-MEC registration.                          |
| **Campus Name**         | NOME_CAMPUS          | Alphanumeric     | Name of the campus of the higher education institution as per e-MEC registration.                    |
| **Campus State**        | UF_CAMPUS            | Alphanumeric     | State abbreviation (UF) where the campus is located.                                                 |
| **Campus City**         | MUNICIPIO_CAMPUS     | Alphanumeric     | Name of the municipality where the campus is located.                                                |
| **Course Name**         | NOME_CURSO           | Alphanumeric     | Name of the course offered by the institution.                                                       |
| **Degree**              | GRAU                 | Alphanumeric     | Degree offered by the course.                                                                        |
| **Shift**               | TURNO                | Alphanumeric     | Shift during which the course is offered (e.g., morning, evening).                                   |
| **Competition Mode**    | MOD_CONCORRENCIA     | Alphanumeric     | Type of competition mode offered for the course.                                                     |
| **Seats Offered**       | QT_VAGAS_CONCORRENCIA| Numeric          | Number of seats offered for the respective mode of competition.                                      |
| **Gender**              | SEXO                | Alphanumeric     | Gender of the student, as filled out in the ENEM/INEP socioeconomic questionnaire.                   |
| **Date of Birth**       | DATA_NASCIMENTO      | Numeric          | Date of birth of the student.                                                                        |
| **Age**                 | IDADE                | Numeric          | Age of the student as of July 30, 2021.                                                              |
| **Candidate State**     | UF_CANDIDATO         | Alphanumeric     | State of residence of the candidate as filled out in the questionnaire.                              |
| **Candidate City**      | MUNICIPIO_CANDIDATO  | Alphanumeric     | City of residence of the candidate as filled out in the questionnaire.                               |
| **Option**              | OPCAO                | Numeric          | Indicates whether it's the first or second option for the candidate.                                 |
| **Language Score**      | NOTA_L               | Numeric          | Score obtained in the Language test.                                                                 |
| **Humanities Score**    | NOTA_CH              | Numeric          | Score obtained in the Humanities test.                                                              |
| **Science Score**       | NOTA_CN              | Numeric          | Score obtained in the Science test.                                                                 |
| **Math Score**          | NOTA_M               | Numeric          | Score obtained in the Mathematics test.                                                             |
| **Essay Score**         | NOTA_R               | Numeric          | Score obtained in the Essay test.                                                                   |
| **Candidate Score**     | NOTA_CANDIDATO       | Numeric          | Average score for the selected course, calculated based on weights defined by institutions.         |
| **Cut-off Score**       | NOTA_CORTE           | Numeric          | Minimum score required for admission to the course.                                                  |
| **Ranking**             | CLASSIFICACAO        | Numeric          | Candidate's rank among all applicants for the same course.                                           |
| **Approved**            | APROVADO             | Alphanumeric     | Indicates whether the candidate was approved in the regular round.                                   |
| **Enrollment Status**   | MATRICULA            | Alphanumeric     | Indicates enrollment status, such as "enrolled" or "rejected documentation".                         |

---

## Tools

To answer the listed questions, students must use the **LEMONADE** platform with the **SPARK** execution option. Create a workflow for the semester being analyzed. Initial workflows for two analyses will be provided on Moodle, which must be modified/completed to answer all questions.

---

## Analysis Questions

### **Analysis I - Candidate and Seat Profiles**
a) What is the age distribution of candidates by gender?  
b) What is the distribution of enrollment/ranking, considering gender separately?  
c) How many candidates are grouped by shift? Considering ranking?  
d) How many seats were offered by state (UF) where the campus is located, considering shifts?  
e) What is the distribution of candidates per seat?  
f) What is the gender distribution of candidates in the Library Science course?  

### **Analysis II - Performance and Candidate Distribution**
a) Considering only confirmed enrollments, how many candidates scored above the average? For these candidates, who chose the course as their first option, what was their average age?  
b) What are the top 5 cities where campuses offered the most seats?  
c) What is the name of the campus and city with the lowest cut-off score among confirmed enrollments?  
d) How many candidates scored 900 or higher in the essay?  
e) What is the name of the course with an integral shift that achieved the highest score in Sciences? What is the minimum and maximum age range for this course and shift?  
f) What are the municipalities of the top 3 candidates with the highest average scores, considering the "Ampla Concorrência" mode?  
g) What percentage of courses had 800 or higher essay scores among female candidates?  
h) For candidates who did not enroll, what was the average Language score, and what are the respective cities of residence?
