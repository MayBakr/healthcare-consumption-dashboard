# Project Background
This project is based on data from a Third-Party Administrator (TPA) in the healthcare insurance industry. The company partners with multiple insurers and corporate clients to manage claims, provider networks, and member benefits.

Between 2018 and 2025, the TPA served almost 30,000 beneficiaries and processed more than 140,000 claims annually. Core business metrics include active membership growth, claims utilization rate, average claim cost per beneficiary, and approval vs. rejection ratio. Additional insights cover demographic distribution, cost breakdown by service category, and provider performance.

Key business metrics include:
- **Membership Growth Rate:** tracking the number of active beneficiaries year-over-year.
- **Claims Utilization Rate:** measuring the frequency and intensity of healthcare service use.
- **Average Claim Cost per Beneficiary:** providing insight into the financial burden per active member.
- **Claims Approval vs. Rejection Ratio:** reflecting service quality, eligibility compliance, and adjudication efficiency.
- **Inpatient vs. Outpatient Cost Share::** highlighting the distribution of healthcare spending across major service categories.

An interactive Power BI dashboard used to report and explore healthcare consumption trends can be found here [[link](https://app.powerbi.com/view?r=eyJrIjoiNTgxMGQ2MGYtM2Q3ZS00YmFjLTk3OGUtOTZkMDAwNjYyMWIzIiwidCI6ImE0MWU5ZTIwLTUxNjYtNGUwZC1hYmU3LTBmYjFmNWZlN2E2MCJ9)].

# Data Structure & Initial Checks

The database consists of four tables (~140K rows in total) that capture beneficiary information, policy relationships, and healthcare consumption data:
- **Beneficiaries:** contains demographic and enrollment details for each member, serving as the reference point for linking utilization records.
- **Consumption:** holds detailed records of healthcare service usage (inpatient, outpatient, pharmacy, etc.), including service type, provider, and cost.
- **Policy Holder Records:** derived from the Beneficiaries table, this table groups members under their respective policy holders, enabling analysis at the policy or corporate level.
- **Beneficiary Records:** integrates beneficiary and consumption details, creating standardized records that allow one-to-many mapping between members and their service usage.
  
<img width="1460" height="703" alt="image" src="https://github.com/user-attachments/assets/feef1701-b4a8-4b57-8669-95dee218adda" />


# Executive Summary

### Overview of Findings

Analysis of healthcare consumption between 2018–2025 revealed that outpatient and pharmacy services represent the highest share of utilization and costs, while inpatient services, though less frequent, are the largest cost drivers per case. Utilization patterns vary significantly across policy holders, with a small percentage of members accounting for a disproportionately high share of total costs. These insights highlight opportunities for cost containment, benefit optimization, and targeted provider negotiations.



# Insights Deep Dive
### Policy Holder & Member Insights

* **Utilization varies significantly by policy holder.** The three largest corporate clients, each with more than 5,000 active members, account for 71 million in total utilization, underscoring their outsized impact compared to smaller groups.
  
* **Age groups influence cost distribution.** Members aged 30–44 years account for 44% of total costs (37 million out of 85 million), highlighting the significant healthcare utilization of this mid-age group.
  
* **Dependent members drive outpatient visits.** Dependent members have minimal impact on outpatient costs. While dependents (spouses and children) account for 200,000 in outpatient payable amounts, this represents less than 1% of total outpatient spending, indicating a relatively minor financial impact.

  <img width="1042" height="731" alt="489006761-5f18a0d1-1468-4075-88f8-3ae0a48b3335-2" src="https://github.com/user-attachments/assets/3e208cb7-d66f-4e7c-bc90-dcdcaa97d4bb" />


### Healthcare Consumption Trends (2018–2025)

* **Outpatient services dominate utilization.** Outpatient services dominate utilization. Outpatient claims accounted for nearly 32% of the total payable amount across 2018–2025. This reflects a strong financial share for outpatient care compared to other services.
  
* **Inpatient services remain the top cost driver.** Inpatient claims accounted for 45% of total payable amounts (38 million out of 85 million) across 2018–2025, underscoring their disproportionate impact on overall healthcare spending compared to other service categories.
  
* **High-cost members drive a disproportionate share.** The top 3 beneficiaries account for 86% of total claims cost, with the majority of expenses linked to chronic conditions and repeated admissions. This concentration highlights opportunities for targeted cost management.
  

<img width="1037" height="732" alt="image" src="https://github.com/user-attachments/assets/611ae4ae-7ec1-4a8f-bac2-4f45763d7279" />


### Top Utilizers Insights

* **Utilization is concentrated among a few providers.** The top 10 small hospitals account for 71% of total hospital costs (20 million out of 28 million), highlighting members’ strong reliance on a limited set of facilities.
  
* **High concentration of spend among few members.** The top 6 beneficiaries account for around 18M in payable amounts — nearly 21% of the total spend (85M). This signals a strong cost concentration within a small segment of the member base, pointing to potential high-risk or chronic cases that require closer monitoring.
  
* **Service-level trends show concentration.** A few services make up the bulk of costs, with noticeable shifts in demand over time.
  
     <img width="566" height="646" alt="image" src="https://github.com/user-attachments/assets/ea5b1a1d-9014-4931-bdf3-84fac7df815b" />


# Final Recommendations

Based on the analysis of healthcare consumption (2018–2025), the following actions are recommended to optimize costs, improve member outcomes, and strengthen provider partnerships:

* **Focus on cost drivers** Prioritize interventions in inpatient care and chronic medication usage, which account for the largest share of total costs despite lower utilization volume.

* **Target high-cost members** Develop chronic disease management and wellness programs aimed at the top 10% of members driving the majority of costs. This will help reduce avoidable admissions and improve long-term health outcomes.

* **Optimize provider network** Expand contracts in underserved regions and negotiate preferred pricing agreements with high-volume hospitals and pharmacies to minimize cost variation.

* **Support preventive care** Encourage policy holders to adopt wellness and preventive benefits, which are already linked to lower inpatient admission rates in certain groups.

# Dashboard
The dashboard is available on Power BI Public. It allows users to filter by plan, beneficiary, and provider, with a focus on trends and values across marketing, signup, and claim metrics.

