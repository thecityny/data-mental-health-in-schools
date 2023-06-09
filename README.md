Here is the data we used for our interactive database <a href="https://projects.thecity.nyc/school-mental-health/">How Well Does Your Child's School Support Student Mental Health?</a>. 

You can read our blog post that explains <a href="https://thecity.admin.usechorus.com/e/23474191">how we matched thousands of NYPD child in crisis calls</a> with the Department of Education data. 

You can also read our story on this subject <a href="https://thecity.admin.usechorus.com/e/23474364">NYC Schools Handcuff and Haul Away Kids in Emotional Crisis</a>.

## Files in the Directory
- **`schools-new.csv`** includes all datapoints displayed in our app.
- **`cic-matched-dbns.csv`** includes school campus names in the NYPD data that we could match with unique school identifiers called DBNs.
- **`cic-unmatched-dbns.csv`** includes school campus names for which we could not pinpoint a given school.

## Definitions:
## School Information
- **`Data Source`**: https://data.cityofnewyork.us/Education/2019-2020-School-Locations/wg9x-4ke6
- **`dbn`**: The DOE assigns each school a unique 6-character code called a DBN, short for District-Borough-Number 
- **`school `**: Official School Name
- **`Address`**: School address
- **`grades_final_text`**: Grades taught  
- **`longitude`**: school location longitude
- **`latitude`**: school location latitude

## 2021-22 School enrollment and demographics
- **`Data Source`**: https://data.cityofnewyork.us/Education/2017-18-2021-22-Demographic-Snapshot/c7ru-d68s
- **`enroll`**: Total enrollment in all grades  
- **`asian`**: Total number of Asian students
- **`black`**:  Total number of Black students
- **`hispanic`**: Total number of Hispanic students 
- **`multi`**:  Total number of Multiracial students
- **`native_a`**: Total number of Native American students
- **`white`**: Total number of white students
- **`iep`**: Total number of students with IEPs
- **`poverty_no`**: Total number of students below the poverty threshold
- **`eni`**: Economic Need Index in 2021-22 as calculated by the Department of Education

## 2021-22 Guidance Counselor
- **`Data Source`**:  https://infohub.nyced.org/reports/government-reports/guidance-counselor-reporting 
- **`total_gc_sw`**: Total number of guidance counselors and social workers, including part-time workers 
- **`gc`**:Total number of guidance counselors, including part-time counselors 
- **`sw`**: Total number of social workers, including part-time workers
- **`provider`**: Name of the school-based mental health clinic. THE CITY obtained this data from the Department of Education. The information can also be found on the DOE's <a href='https://www.schools.nyc.gov/schools/K001'>website</a>.
- **`school_psychologist_providing`**: Whether school psychologists are providing mandated counseling. This column is binary coded; 0 =no and 1=yes.
- **`lead_cbo_partner`**:The name of school's community-based organization partner for mental health support. THE CITY and Chalkbeat obtained the 2022-23 list exclusively from the DOE. `cs_director` values listed have community school directors who are directly employed by the DOE rather than a CBO. `no_cbo` means that the school is a community school but as of publication hasn't named a CBO yet. Previous reports can be found at this <a href='https://data.cityofnewyork.us/Education/2021-2022-Community-Schools-List/su38-ur5m/data'>data source</a>

## Temporary housing, 2021-22 school year
- **`Data Source`**: https://infohub.nyced.org/reports/government-reports/students-in-temporary-housing-reports
- **`pct_temp_housing`**: The percent of students experiencing housing instability.

# School Surveys
- **`Data Source`**: 
- **`s_rr`**: student response rate
- **`s_know_mh_re_ag`**: Students know about the mental health resources.

## Chronic Absenteeism, 2021-22 school year
- **`Data Source`**: https://infohub.nyced.org/reports/school-quality/information-and-data-overview/end-of-year-attendance-and-chronic-absenteeism-data
- **`pct_chronic_absent`**: Percent of students chronically absent – missed 10% of school days or more

## School Safety (NYPD activity in schools), First quarter 2016 to fourth quarter 2022
Definitions from the NYPD <a href='nyc.gov/assets/nypd/downloads/pdf/school_safety/student-safety-act-report-definitions.pdf'>here</a>
- **`Data Source`**: https://www.nyc.gov/site/nypd/stats/reports-analysis/school-safety.page
- **`cic`**:  "A student who is displaying signs of emotional distress who must be removed to the hospital for psychological evaluation. Only subjects for which mechanical restraints were used are reported here."

If you spot problems with the data, you can send us a pull request or issue here, or email us at [data@thecity.nyc](mailto:data@thecity.nyc).
