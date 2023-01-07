# Virtual Machine (VM) Exercises

## :information_source: Read this before getting started
- The goal of exercises in case study is for learners to apply what was learned in the previous courses to new problems or situations. This is best pedagogical practice for retaining and building skills.
- We can only run free versions of BI software in our virtual machine exercises. In the case of Power BI, make sure the exercises can run on [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) without any additional paid products. 
- Unsure what the scope of an exercise should be? Here's an [example](https://campus.datacamp.com/courses/case-study-analyzing-customer-churn-in-tableau/exploratory-analysis-1?ex=4) from the Case Study: Analyzing Customer Churn in Tableau. The first chapter of most DataCamp courses are free, so take a look at our [BI courses](https://learn.datacamp.com/courses?technologies=Tableau&technologies=Power%20BI) to get a feel for how we assess and guide learners in **case studies**.

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
- [x] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix`

#### Learning Objective

*You will learn how to calculate Extended Cost and Full Cost from quotes data.*

#### Context

When making a Supply Chain decision, it is important to understand the full cost of any option. Full cost consists of two components: Extended cost (the total cost of products purchased) and non-recurring expenses (one-time expenses). 

You will first create an Extended Cost calculated column, then use that to create a Full Cost calculated column in the Quotes table. 
While it is possible to create a Full Cost column without adding the Extended Cost step, displaying the breakdown between Extended Cost and Full Cost is useful for informing future Supply Chain work such as price negotiations. 


#### Steps to be executed by the student (max 6)

*Each bulleted instruction is a complete sentence that describes a specific task.*

- Step 1: Create a simple table visual that includes columns for Supplier, Part, Volume, Quoted Price and Non-recurring-expenses. Make sure that the table does not summarize any of the variables, because you will want to see the results for each line.
- Step 2: Create a calculated column for Extended Cost. Extended cost is the quoted cost multiplied by the number of units quoted.  
Add the newly created column to your table visual.
- Step 3: Create a calculated column for Full Cost. Full cost is the total cost required to purchase the parts from the supplier - Extended Cost plus non-recurring expenses. 
Add the newly created column to your table visual.

#### Exercise question:
The New Product Launch team reports that we need 10,000 units of part P0914 (part name Chattlecrat). Which supplier has the lowest Full Cost, and what is it?

#### End goal:

*We could definitely ask the student for a more beautiful, fun visualization but I kept it simple for this first round. Additionally, the answer to the question is not included in the screenshot but would be available to the student by scrolling or filtering the table.* 

![image](https://user-images.githubusercontent.com/6133961/211061244-3e0b68b9-5198-4f63-be19-63d27047d73d.png)

## Finalized Workbook

I have created a workbook that showcases the volume parameter and how it affects the Supplier Selection decisions. In my course outline, the parameter is actually introduced _after_ calculating the Make option, but I thought this would be a better demonstration of the final output for the learner. 

#### Files
You can upload your final workbook in the exercises folder as `ex-final-sol.twbx` or `ex-final-sol.pbix`.

#### Explanation & Description
At the end of this lesson, the student will be able to identify the supplier for any given part-volume combination by using the full cost and extended cost. In a real supply chain situation, this maybe the first round that identifies which supplier to negotiate with or collaborate with on further design changes. In the context of Make vs. Buy analysis, the lowest cost external supplier option is typically measured against the best "Make" option. In the coming lessons, the student will learn how to calculate Extended Cost and Full Cost for internal options which are little complicated because the Full Cost of the Make option is dependent on existing resource capacity. 

#### End goal:

![image](https://user-images.githubusercontent.com/6133961/211120113-cab46d20-5bf2-47d4-86d0-abdae80f3b9a.png)
