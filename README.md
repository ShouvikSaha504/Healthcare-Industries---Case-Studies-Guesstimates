# Healthcare-Industries---Case-Studies-Guesstimates


# Overview
This repository contains case studies and guesstimates related to the healthcare industry, focusing on product dissection, database management, schema design, and revenue/profit growth strategies. The goal is to provide detailed insights and data-driven strategies to address real-world challenges in healthcare through the application of data science and advanced analytics.

The healthcare industry is a cornerstone of society, providing essential services that ensure the well-being and health of populations worldwide. In today's era, its importance has been underscored by the rapid advancements in medical technology and the increasing demand for quality healthcare services. The industry faces numerous challenges, including rising costs, ageing populations, and the need for more efficient patient care. 

Data scientists play a pivotal role in addressing these challenges, leveraging their expertise to analyse vast amounts of healthcare data. They help in predicting disease outbreaks, personalising treatment plans, and improving patient outcomes through predictive analytics. Additionally, data scientists optimise hospital operations, enhance diagnostic accuracy with machine learning algorithms, and contribute to the development of new medical treatments and drugs. By harnessing the power of data, they drive innovation, improve efficiency, and ensure the delivery of high-quality healthcare services, making a significant impact on the industry's growth and sustainability.

**Part I & Part II link:** https://github.com/ShouvikSaha504/Healthcare-Industries---Case-Studies-Guesstimates/blob/96c98d693ccb216c926bdb485e9849636ad1b029/Healthcare%20Industries%20-%20case%20study%20Shouvik%20Saha.docx

**PART - I**

**Product Dissection**

1. Platform Selection
Question: Choose a leading platform from a domain related to the e-commerce industry. Justify your selection by discussing the platform's popularity, impact, and relevance in its industry.

2. Core Features and Functionalities
Question: Research and list the core features and functionalities of the selected platform. Describe how these features contribute to the platform’s success and user engagement.

3. Real World Problems
Question: Identify the real-world problems that the platform aims to solve. Discuss how the platform addresses these problems through its features and functionalities.

**Database Management & Schema Design** 

4. Schema Design
Question: Based on the features and functionalities you have identified, design a schema that reflects the platform’s data structure. Define the key entities, attributes, and relationships that underpin these features.

5. ER Diagram Creation
Question: Utilise tools like the Miro platform or similar applications to create an illustrative Entity-Relationship (ER) diagram. This diagram should vividly depict the entities, attributes, and relationships present within your schema design.

**Revenue and Profit Growth Strategies**
Question: After completing the product dissection and schema design steps for the chosen platform, conduct a comprehensive case study on the above chosen industry. Your goal is to identify and propose strategies to increase the profit of the industry by at least 25%.

Create a detailed report summarising your findings and proposals. Include data-driven justifications for each proposed strategy and present your case study using visual aids such as charts, graphs, and diagrams to illustrate your points. Outline the steps, resources, and timeline required to achieve the desired revenue and profit growth.


# Project Objective

This project aims to dissect and analyze Apollo 24/7 Pharmacy as a leading platform in the healthcare e-commerce domain. It involves evaluating the platform’s features, functionalities, and impact, designing a relevant database schema, and proposing strategies for revenue and profit growth. Additionally, it includes estimating potential cost savings and revenue generation opportunities through various healthcare-related scenarios. The project leverages data-driven insights to enhance understanding of the platform's role in the healthcare industry and propose actionable strategies for improvement.

# Project Description

## 1. Platform Selection

**Apollo 24/7 Pharmacy** was chosen for this analysis due to its significant presence and impact in the healthcare e-commerce sector. It stands out for its innovative approach to providing healthcare services online, making it highly relevant in today’s digital age.

- **Popularity**: Apollo 24/7 Pharmacy has rapidly gained prominence in the online pharmacy market, leveraging the extensive network and trusted reputation of Apollo Hospitals. Its use of advanced technology and a robust supply chain ensures a wide range of medications and healthcare essentials with quick and reliable delivery, contributing to its widespread appeal among customers.

- **Impact**: Apollo 24/7 Pharmacy has made a notable impact by setting new standards for accessibility and efficiency in medication delivery. Its integration of advanced technology, such as real-time inventory management and personalized health recommendations, has influenced other pharmacies to elevate their services, enhancing customer satisfaction and loyalty.

- **Relevance**: The platform’s connection with Apollo Hospitals enhances its operational efficiency and service quality. By incorporating sophisticated tools like real-time inventory tracking and data-driven insights, Apollo 24/7 Pharmacy meets the urgent needs of modern consumers, solidifying its role in the digital healthcare landscape.

## 2. Core Features and Functionalities

We explored the core features and functionalities of Apollo 24/7 Pharmacy, which include:

- **Online Consultation Services**: Facilitates remote consultations with healthcare professionals.
- **Medicine Delivery**: Provides timely delivery of prescribed medications.
- **Health Records Management**: Enables users to manage and access their health records easily.
- **Personalized Healthcare**: Offers tailored health advice and treatment plans based on user data.

### Contribution to Success and User Engagement

- **Accessibility**: Fast delivery and a broad selection of medications meet the critical need for immediate access to health products.
- **Improved User Experience**: An intuitive interface, customized recommendations, and real-time order tracking enhance user satisfaction.
- **Customer Retention**: Promotions, discounts, and auto-refill options encourage repeat purchases and foster loyalty.
- **Operational Excellence**: Integration with Apollo Hospitals ensures reliable service and operational efficiency.
- **Personalized Health Insights**: Data-driven recommendations cater to individual needs, increasing engagement.

## 3. Real-World Problems

Apollo 24/7 Pharmacy addresses several real-world problems such as:

- **Access to Healthcare**: Overcomes geographical barriers with remote consultations.
- **Medication Adherence**: Ensures timely delivery of medications to improve adherence.
- **Efficient Health Management**: Simplifies management and access to health records.

### Solutions to Challenges

The platform’s features and functionalities tackle these challenges by:

- **Enhancing Accessibility**: Provides healthcare services online, eliminating geographical and time-based barriers.
- **Streamlining Processes**: Simplifies obtaining medications and consultations.
- **Improving Health Outcomes**: Offers personalized healthcare and efficient health record management.

## 4. Schema Design

To design a schema for Apollo 24/7 Pharmacy, the following key entities, attributes, and relationships are defined:

- **User**
  - `User_ID` (Primary Key)
  - `Name`
  - `Email`
  - `Password`
  - `Phone`
  - `Address`
  - `RegistrationDate`

- **Product**
  - `Product_ID` (Primary Key)
  - `Name`
  - `Description`
  - `Price`
  - `Category`
  - `Stock Quantity`

- **Order**
  - `Order_ID` (Primary Key)
  - `User_ID` (Foreign Key)
  - `Order Date`
  - `Total Amount`
  - `Status`

- **Order_Detail**
  - `Order_Detail_ID` (Primary Key)
  - `Order_ID` (Foreign Key)
  - `Product_ID` (Foreign Key)
  - `Quantity`
  - `Price`

- **Cart**
  - `Cart_ID` (Primary Key)
  - `User_ID` (Foreign Key)
  - `Created_Date`

- **Cart_Item**
  - `Cart_Item_ID` (Primary Key)
  - `Cart_ID` (Foreign Key)
  - `Product_ID` (Foreign Key)
  - `Quantity`
  - `Brand`

- **Circle_Membership**
  - `User_ID` (Foreign Key)
  - `Order_ID` (Foreign Key)
  - `Membership_Type`
  - `Membership_Description`

- **Promotion**
  - `Promotion_ID` (Primary Key)
  - `Code`
  - `Description`
  - `Discount_Percentage`
  - `Start_Date`
  - `End_Date`

- **User_Promotion**
  - `User_Promotion_ID` (Primary Key)
  - `User_ID` (Foreign Key)
  - `Promotion_ID` (Foreign Key)
  - `Usage_Date`

### Relationships

- `User` to `Order`: One-to-Many
- `Order` to `Order_Detail`: One-to-Many
- `Product` to `Order_Detail`: Many-to-One
- `User` to `Cart`: One-to-Many
- `Cart` to `Cart_Item`: One-to-Many
- `Product` to `Cart_Item`: Many-to-One
- `User` to `User_Promotion`: One-to-Many
- `Promotion` to `User_Promotion`: One-to-Many
- `Circle_Membership` to `User`: One-to-One
- `Circle_Membership` to `Order`: One-to-Many

This schema captures the essential data interactions and relationships within Apollo 24/7 Pharmacy, ensuring efficient data management and supporting the platform’s features and functionalities effectively.

**ER Diagram link:** https://github.com/ShouvikSaha504/Healthcare-Industries---Case-Studies-Guesstimates/blob/a27ca05126df471687bfc01cb111ad30d2adfee6/ER_Diagram.JPG


**ER Diagram:**
![image](https://github.com/user-attachments/assets/f4ce25be-aa98-4066-b837-0470e8f5fc02)

## Analyzing How to Increase Apollo Pharmacy's Profit by 25%

### Focus of the Problem Statement

To address the challenge of boosting Apollo Pharmacy's profit by 25%, we implemented an inside-out approach. This strategy focuses on evaluating internal factors first, such as analyzing company expenses, customer behavior, and revenue strategies, to enhance profitability.

### I. Analyzing Apollo Pharmacy's Current Status

To assess Apollo Pharmacy's current status and devise a strategy to boost its profit by 25%, we need to perform a comprehensive analysis of the company's present situation. This involves evaluating its current profit, identifying sources of revenue and expenses, and examining customer acquisition and retention strategies.

#### Current Financial Data

| **Category**        | **Details**                                                                                                              |
|---------------------|--------------------------------------------------------------------------------------------------------------------------|
| **Revenue**         | Apollo Pharmacy achieved a total revenue of ₹74,537 million in FY2024. Major revenue streams include sales from pharmaceuticals, healthcare products, Circle Membership, and additional services. |
| **Expenses**        | Apollo Pharmacy spent a total of ₹61,251 million in FY2024 on COGS, supply chain management, employee salaries, finance costs, marketing, and other operational expenses. |
| **Profit Calculation** | Total Revenue (FY2024): ₹74,537 million <br> Total Expenses (FY2024): ₹61,251 million <br> Profit Before Tax (PBT): ₹13,286 million <br> Profit After Tax (PAT): ₹10,105 million |
| **Profit Trends**    | **Year-on-Year Analysis:** <br> FY2024 - ₹10,105 million <br> FY2023 - ₹10,848 million (6.85% decline) <br> **Quarter-on-Quarter Analysis:** <br> Q2 - ₹3,633 million <br> Q3 - ₹3,682 million (1.35% growth) |

#### Sources of Revenue

| **Revenue Stream**          | **Details**                                                                                                             |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------|
| **Sales from Pharmaceuticals** | Primary revenue source, including prescription and over-the-counter drugs.                                             |
| **Sales from Health Care Products** | Includes health and wellness products, nutritional supplements, and personal care items.                                 |
| **Circle Membership**        | Subscription-based program offering health services and additional benefits.                                             |
| **Additional Services**      | Diagnostic services, health check-ups, and consultation fees.                                                            |

#### Top Products/Services

| **Top-Selling Products**                 | **Most Popular Subscription Plans**                                          |
|------------------------------------------|------------------------------------------------------------------------------|
| **Prescription Medications**             | Includes drugs for chronic diseases (e.g., Metformin, Amlodipine, Atorvastatin) |
| **Over-the-Counter (OTC) Drugs**          | Pain relievers (e.g., Paracetamol), cough and cold remedies, antacids            |
| **Health and Wellness Products**         | Multivitamins, dietary supplements, personal care products                       |
| **Circle Membership Plans**               | Benefits include 24/7 access to doctors, free lab tests, discounts on medicines, and more. |

#### Sources of Expenses

| **Expense Category**         | **Details**                                                                                                               |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Cost of Goods Sold (COGS)** | ₹19,990 million in FY2024, covering procurement and production of pharmaceutical and grocery items.                   |
| **Supply Chain Costs**       | Approximately ₹4,957.65 million, including logistics, warehousing, and transportation expenses.                           |
| **Marketing and Advertising**| Approximately ₹1,531.28 million on advertising, promotions, and customer acquisition campaigns.                           |
| **Employee Salaries**        | ₹14,252 million in FY2024, covering salaries, wages, benefits, and other employee-related expenses.                      |
| **Other Operational Expenses** | ₹20,521 million in FY2024, including rent, utilities, administrative costs, and miscellaneous expenses.                     |

#### Improving Cost Efficiency

1. **COGS**: Negotiate better supplier prices, buy in bulk, and reduce waste.
2. **Operational Expenses**: Invest in energy-saving technologies, streamline operations, and renegotiate leases.
3. **Employee Salaries**: Use performance-based pay, invest in training, and consider outsourcing non-core activities.
4. **Supply Chain Costs**: Optimize logistics, improve supplier relationships, and use technology for better inventory control.
5. **Marketing and Advertising**: Emphasize cost-effective digital marketing, track ROI, and leverage in-house resources.

#### Customer Acquisition & Retention

| **Category**                      | **Details**                                                                                                         |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **Customer Acquisition Channels** | ApolloPharmacy.com receives new customers through referrals, Google search, targeted advertising, and word of mouth. |
| **Effectiveness of Channels**     | **YouTube**: Engages audience through interactive content. <br> **Google Search Engine**: Captures high-intent users. <br> **Word of Mouth**: Cost-effective but hard to quantify. <br> **Advertising Program**: Expensive but broad reach. |
| **Customer Data**                 | **Purchase History**: Frequent purchases of pharmaceuticals and healthcare products. <br> **Feedback**: Evaluates customer satisfaction and areas needing improvement. |
| **Retention Rates**               | Approximately 75% retention rate. <br> **Factors Contributing to Loyalty**: High-quality services, Circle Membership benefits, personalized experiences. |
| **Churn Analysis**                | **Reasons for Churn**: Competition, price sensitivity, lack of engagement. <br> **Strategies to Reduce Churn**: Competitive pricing, addressing feedback, enhancing loyalty programs. |

### II. Focus Areas for Increasing Apollo Pharmacy's Profit by 25%

To boost Apollo Pharmacy’s profit by 25%, the company needs to strategically concentrate on several critical areas. These include internal operations, product development strategies, market expansion, post-sales management, and branding.

#### Focus Areas and Measures

| **Category**                     | **Focus Area**                       | **Measures**                                                                                                                                                                          |
|----------------------------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Internal Operations**          | **Process Optimization**            | Refine workflows, eliminate bottlenecks, and implement automation to improve efficiency.                                                                                             |
|                                  | **Quality Control**                 | Implement quality control measures to ensure high standards and reduce errors.                                                                                                        |
|                                  | **Cost Control**                    | Identify and cut unnecessary expenses, optimize inventory, and reduce waste.                                                                                                         |
| **Human Resource Management**    | **Training and Development**        | Invest in regular training and development to improve employee skills and efficiency.                                                                                                 |
|                                  | **Strategic Hiring**                | Hire skilled employees efficiently to meet company needs.                                                                                                                             |
|                                  | **Performance Management**          | Use performance management systems to set goals, provide feedback, and assess performance.                                                                                           |
| **Logistics and Operations Management** | **Supplier Coordination**         | Enhance supplier relationships, negotiate better terms, and improve procurement processes.                                                                                           |
|                                  | **Logistics Optimization**          | Streamline transportation, warehousing, and inventory management to improve efficiency and reduce costs.                                                                             |
| **Product Development**          | **Product Optimization**            | Cut down underperforming products and focus on successful ones.                                                                                                                       |
|                                  | **Product Design**                  | Introduce combo packages for essential health products to increase sales.                                                                                                            |
| **Market Expansion**             | **Regional Expansion**              | Extend reach to new regions or countries.                                                                                                                                             |
|                                  | **Market Penetration**              | Increase market share within existing regions through local advertising and expanding product lines.                                                                                 |
| **Post-Sales Management**        | **Customer Satisfaction**           | Collect feedback, provide responsive customer support, and ensure high service standards.                                                                                            |
|                                  | **Customer Retention**              | Implement loyalty programs and personalized follow-ups to keep customers engaged.                                                                                                      |
| **Branding and Marketing**       | **Brand Visibility**                | Use digital marketing, SEO, and partnerships to increase brand reach and engagement.                                                                                                 |
|                                  | **Word of Mouth and Referrals**     | Implement referral programs and encourage positive reviews to build trust and attract new customers.                                                                                  |

### III. Defining Strategies

| **Category**                | **Details**                                                                                                                                                              |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Optimize Expenses**       | **Cost Reduction**: Negotiate better terms with suppliers, streamline logistics, and adopt cost-effective technologies. <br> **Efficiency Improvements**: Optimize inventory management, reduce waste, and streamline operations. |
| **Enhance Revenue Streams** | **Upselling and Cross-Selling**: Implement a recommendation engine for enhanced order value. <br> **New Revenue Streams**: Launch subscription services and telemedicine. <br> **Pricing Strategies**: Implement dynamic pricing to attract more customers. |
| **Improve Customer Satisfaction and Retention** | **Personalized Experiences**: Use purchase history to provide tailored recommendations and discounts. <br> **Loyalty Programs**: Launch a points-based program and offer additional points for referrals. <br> **Customer Feedback**: Conduct surveys and use feedback for service improvements. |

By focusing on these strategic areas, Apollo Pharmacy can achieve a 25% increase in profitability while maintaining high standards of customer care and service. This data-driven approach ensures sustainable growth and strengthens Apollo Pharmacy’s market position.

**PART - II**

**Guesstimates**

1. Question 1: Estimate the potential annual cost savings for a hospital if it reduces its readmission rate by 10%.

2. Question 2: Estimate the potential annual revenue generated by a hospital if 20% of its consultations are shifted to telemedicine.
3. Question 3: Estimate the potential annual market size (in dollars) for a new medical device designed for diabetes management in the United States.
4. Question 4: Estimate the potential additional annual revenue for a clinic from implementing preventive care programs.
5. Question 5: Estimate the potential annual cost savings for a hospital from optimizing its supply chain management.

**Flowchart for Guesstimation:** 

| Step               | Description                                            |
|--------------------|--------------------------------------------------------|
| Approach Selection | Choose between Demand Side or Supply Side Approach    |
| Define Starting Points | Start with definite numbers like population/city area |
| Estimation Steps   | Break down the estimation into smaller steps          |
| Calculation        | Apply ratios and aggregate data                       |
| Final Estimation   | Calculate the final percentage                        |

**Method:** To solve these questions, we implemented a demand-side approach. We started with the total population and bifurcated it at each step to arrive at the final answer.


## Conclusion

## Conclusion

The **Healthcare-Industries---Case-Studies-Guesstimates** project encapsulates a comprehensive exploration of the healthcare sector through detailed case studies and guesstimates, with a specific focus on Apollo 247 Pharmacy. By examining product dissection, database management, schema design, and revenue/profit growth strategies, this repository offers valuable insights and data-driven approaches to address real-world challenges within the industry.

Apollo 247 Pharmacy, a significant player in the healthcare sector, is at the forefront of addressing the needs of a rapidly evolving market. The project highlights the critical role of data science in optimizing pharmacy operations, enhancing customer experience, and driving revenue growth. Through detailed analysis and innovative strategies, this project underscores how leveraging data can lead to more efficient operations, better decision-making, and improved patient outcomes.

By focusing on Apollo 247 Pharmacy, the project provides a strategic framework for navigating the complexities of the healthcare industry, demonstrating how data-driven insights can foster growth and sustainability in a competitive landscape. This repository not only offers practical solutions for Apollo 247 Pharmacy but also serves as a model for similar organizations striving to enhance their impact in the healthcare sector.


