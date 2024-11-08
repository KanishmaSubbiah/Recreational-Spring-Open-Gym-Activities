                                **ETL Optimization and Predictive Analysis for Recreational Spring Open Gym Activities**

**Overview:**

This project analyzes Recreational Spring Open Gym Activities data from Kaggle. By cleaning, normalizing, and visualizing the data, it aims to provide insights into activities, locations, timings, and participants during the spring season.

**Abstract:**

This project explores Recreational Spring Open Gym Activities data, using Extract, Transform, Load (ETL) processes and visualization techniques for valuable insights into various activities during the spring season.

**Problem Statement:**

The dataset initially presented challenges related to cleanliness, normalization, and visualization. Issues included combined address fields, redundant information, and the need for a structured data model. Addressing these challenges was crucial for deriving meaningful insights and presenting information effectively.

**Normalization:**

**1. Why is this table not in 1NF?**

Combining house number and street violated atomicity.
Two address columns hinted at repeating groups; removing one addressed this, adhering to 1NF.

**2. 0NF – 1NF**

Data was restructured into separate columns for clarity.

**Find all Functional Dependency:**

B, L -> C, D, E, F, G
A, I, J, K, L, M -> H

**Find the minimum cover:**

B, L -> C, D, E, F, G
A, I, J, K, L, M -> H

**Eliminating Redundancy:**

B, L -> C, D, E, F, G
A -> H
I -> H
J -> H
K -> H
L -> H
M -> H

**Super Key:**

B -> C, D, E, F, G
L -> C, D, E, F, G
A -> H
I -> H
J -> H
K -> H
L -> H
M -> H


**Normalization:**

The dataset was normalized to adhere to the principles of the First Normal Form (1NF), Second Normal Form (2NF), and Third Normal Form (3NF).

**2NF:**
Now, each relation is in 2NF because all non-prime attributes depend on the entire candidate key.

**3NF:**
There is no transitive dependency, making it comply with 3NF.

**Final Relations:**
R(BLCDEFG)
R(AIJKMLH)

**Data Visualization:**

Data visualization plays a crucial role in conveying insights from the processed data in a comprehensible and visually appealing manner.

1) Pie Chart: Represents the frequency of each activity conducted in recreational centers.
2) Bar Chart: Displays the age distribution based on the count of each age group.
3) Geographical Map: Illustrates areas with the highest concentration of recreational centers.
4) Table Visualization: Presents the days of the week with the highest activity counts.
5) Dashboard: Introduction Dashboard -The poster provides insights into various exercise and fun options, emphasizing the availability of activities across community centers in Pennsylvania, Wisconsin, and Maryland.
6) Dashboard: Recreational and Activity Dashboard - A dynamic visualization tool offering a comprehensive overview of Recreational Spring Open Gym Activities. Enhances understanding of activity popularity, geographic concentrations, and age preferences.

**Conclusion:**

The dataset and visuals offer insights into diverse exercise options at community centers, promoting community engagement. The user-friendly dashboards encourage exploration for a healthier and more connected community through accessible recreation.
