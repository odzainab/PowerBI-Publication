# Content Publication & Member Engagement Dashboard

_Uncovering how content, creators, and membership strategies drive audience engagement and platform value._

---

## Quick Look

- **Total Reach:** 1.45M views, 779K reads  
- **Growth:** +93.4% YoY views, +82.3% YoY reads  
- **Member Engagement:** +40.1% YoY member reads  
- **Top Content Type:** Tutorials & how-to guides  
- **Peak Months:** October & November  
- **Key Challenge:** Declining read rate (-5.8% YoY)  
- **Tools Used:** Power BI, Power Query
- **Raw Dataset:** [View Dataset](https://github.com/powerbi-masterclass/2026-new-year-report-challenge)
- **Dashboard:** [View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDk4MzRmNzEtYTE3NS00NWZhLWIxYWMtM2JkMDk2OWI4ODg3IiwidCI6IjdlMGI1ZmNmLTEyYzQtNGVmZi05NmI2LTQ2NjRmMjVkYzdkYSIsImMiOjEwfQ%3D%3D)
- **Full Analysis:** [Medium](https://medium.com/@odzainab1/behind-the-numbers-how-power-bi-can-master-content-engagement-and-retention-70d48f342930)


---

## Introduction

Digital publishing platforms rely on data-driven strategies to balance **audience growth, engagement, and membership monetization**. This analysis evaluates story performance using readership, engagement, and metadata attributes to understand how different content types and authors contribute to platform value.

The goal is to surface **actionable insights** that guide editorial decisions, content gating strategies, and creator investment.

---

## Business Objective

- Identify which content and creators drive meaningful engagement  
- Understand differences between member and non-member behavior  
- Support editorial, promotional, and membership strategy optimization  

---

## Dataset & Tools

### Dataset 1: Story Engagement Metrics
- StoryId  
- Time attributes (Year, Month, Period)  
- Views (Total, Member, Non-Member)  
- Reads (Total, Member, Non-Member)  

### Dataset 2: Story Metadata & Interaction
- StoryId, Title, Author  
- Member-only indicator  
- Publish date  
- Classification (JSON)  
- Claps and Responses  

### Tools
- Power Query – Data cleaning and transformation  
- Power BI – Data modeling, DAX measures, and visualization  

---

## Data Preparation & Validation

1. **DimDate Table Creation**
   - Extracted Year, Month, Period  
   - Created month names, month numbers, and quarters  
   - Removed duplicates to ensure accurate time analysis  

2. **DimClassification Table**
   - Parsed JSON classification field  
   - Extracted MustRead, Level, Category, Tags, Promotion  
   - Flattened arrays into readable text  
   - Replaced nulls with defaults (e.g., “Unknown”)  

3. **Data Cleaning**
   - Handled null JSON values and duplicates  
   - Ensured all transformations were robust and error-safe  

4. **Relationships**
   - StoryStats → Story → DimClassification  
   - StoryStats → DimDate  

This structure supports accurate time-based analysis, member segmentation, and content performance tracking.

---
## Data Visualization


![PowerBI January Challenge-1_page-0001](https://github.com/user-attachments/assets/f2daaa72-7595-4ce2-97ce-316c30394e2c)

![PowerBI January Challenge-2_page-0001](https://github.com/user-attachments/assets/aff31f8e-2e5d-4832-9f8e-ac935917bd01)

## Key Insights

- **Strong Growth:** Views and reads increased significantly, signaling expanding reach and engagement.  
- **Engagement Gap:** Read rate declined, suggesting content visibility is rising faster than content consumption.  
- **Member vs Non-Member:** Members engage more deeply per story, while non-members drive most traffic.  
- **Seasonality:** Engagement peaks in October and November; December shows the lowest activity.  
- **Top Content:** Educational and tutorial-based stories dominate top performers.  
- **Low Interaction:** High claps but low responses indicate approval without deep conversation.  
- **Author Consistency:** Most authors contribute sporadically; a few dominate output.  
- **Content Classification Issues:** Large portion of stories labeled “Unknown,” limiting topic-level analysis.

---

## Recommendations

1. **Strengthen Member-Only Content** – Expand premium, niche, and high-value content offerings.  
2. **Boost Non-Member Conversion** – Use previews, limited-time access, and frictionless sign-ups.  
3. **Plan for Seasonality** – Release high-impact content during peak months and tailor off-peak strategies.  
4. **Improve Read Rate** – Refine content structure, visuals, and value clarity.  
5. **Increase Author Consistency** – Incentivize regular contributions from high-performing authors.  
6. **Fix Content Classification** – Rebuild categorization to eliminate “Unknown” labels.  
7. **Encourage Interaction** – Add prompts, polls, and CTAs to increase responses.

---

## Next Steps

- Build editorial pipelines around high-performing content models  
- Launch targeted conversion experiments  
- Audit and standardize content classification  
- Introduce author recognition programs  
- Track engagement trends continuously  

---

## Conclusion

The platform is experiencing **strong growth in reach and engagement**, driven largely by non-members and high-performing educational content. However, declining read rates, low interaction depth, and inconsistent author contributions highlight opportunities for improvement.

By strengthening premium content, refining content quality, improving classification, and investing in creators, the platform can enhance engagement, improve member conversion, and scale long-term value.
