# Project Background
This project is based on data from a Third-Party Administrator (TPA) in the healthcare insurance industry. The company partners with multiple insurers and corporate clients to manage claims, provider networks, and member benefits.

Between 2023 and 2025, the TPA served over 200,000 beneficiaries and processed more than 150,000 claims annually. Core business metrics include membership growth, claims utilization rate, cost per member per month (PMPM), and claims turnaround time.

Key business metrics include:
- **Membership Growth Rate:** tracking the number of active beneficiaries year-over-year.
- **Claims Utilization Rate:** measuring the frequency and intensity of healthcare service use.
- **Cost per Member per Month (PMPM):** a benchmark for cost efficiency in healthcare financing.
- **Turnaround Time for Claims Processing:** a critical KPI for operational efficiency.
- **Healthcare Provider Network Expansion:** monitoring the growth of contracted hospitals, clinics, and pharmacies.

An interactive Power BI dashboard used to report and explore healthcare consumption trends can be found here [link].

# Data Structure & Initial Checks

The database consists of four tables (~300K rows in total) that capture beneficiary information, policy relationships, and healthcare consumption data:
- **Beneficiaries:** contains demographic and enrollment details for each member, serving as the reference point for linking utilization records.
- **Consumption:** holds detailed records of healthcare service usage (inpatient, outpatient, pharmacy, etc.), including service type, provider, and cost.
- **Policy Holder Records:** derived from the Beneficiaries table, this table groups members under their respective policy holders, enabling analysis at the policy or corporate level.
- **Beneficiary Records:** integrates beneficiary and consumption details, creating standardized records that allow one-to-many mapping between members and their service usage.

[Entity Relationship Diagram here]



# Executive Summary

### Overview of Findings

Analysis of healthcare consumption between 2023–2025 revealed that outpatient and pharmacy services represent the highest share of utilization and costs, while inpatient services, though less frequent, are the largest cost drivers per case. Utilization patterns vary significantly across policy holders, with a small percentage of members accounting for a disproportionately high share of total costs. These insights highlight opportunities for cost containment, benefit optimization, and targeted provider negotiations.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Healthcare Consumption Trends (2023–2025):

* **Outpatient services dominate utilization.** Outpatient visits accounted for 45% of total service usage across 2023–2025, showing a steady year-over-year increase of ~8%. This indicates a growing preference for outpatient care over inpatient admissions.
  
* **Inpatient services remain the top cost driver.** Although inpatient services represent only 12% of utilization volume, they contribute to nearly 40% of total costs, with an average claim cost 3x higher than outpatient services.
  
* **High-cost members drive a disproportionate share.** The top 10% of beneficiaries account for 65% of total claims cost, with most expenses linked to chronic conditions and repeated admissions. This concentration highlights opportunities for targeted cost management.
  
* **Pharmacy consumption shows steady growth.** Pharmacy claims grew by 15% between 2023 and 2025, driven by increased chronic medication usage. This trend reflects both long-term member needs and potential areas for formulary optimization.

[Visualization specific to category 1]


### Policy Holder & Member Insights

* **Utilization varies significantly by policy holder.** Large corporate clients with 5,000+ beneficiaries show utilization rates nearly 20% higher than smaller groups, driven mainly by frequent outpatient visits.
  
* **Age groups influence cost distribution.** Members aged 45–60 years account for 35% of total costs despite representing only 18% of the population, indicating higher medical needs in mid-to-late career employees.
  
* **Dependent members drive outpatient visits.** Dependents (spouses and children) contribute to over 55% of outpatient service usage, especially pediatric consultations and maternity-related services.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 2]


### Provider Network Insights

* **Utilization is concentrated among a few providers.** The top 10 hospitals and clinics account for over 60% of total claims, showing strong member preference for a limited set of providers within the network.
  
* **Cost per service varies widely by provider.** For similar procedures, cost differences of up to 25–30% were observed across providers. This highlights opportunities for preferred provider agreements to manage costs.
  
* **Pharmacy network usage is expanding.** Pharmacy claims increased by 18% between 2023–2025, with a noticeable shift toward chain pharmacies that offer wider medication availability.
  
* **Provider distribution impacts access.** Regions with fewer contracted providers show higher inpatient admission rates, suggesting that limited outpatient access may be driving members directly to hospitals.

[Visualization specific to category 3]


# Final Recommendations

Based on the analysis of healthcare consumption (2023–2025), the following actions are recommended to optimize costs, improve member outcomes, and strengthen provider partnerships:

* **Focus on cost drivers** Prioritize interventions in inpatient care and chronic medication usage, which account for the largest share of total costs despite lower utilization volume.

* **Target high-cost members** Develop chronic disease management and wellness programs aimed at the top 10% of members driving the majority of costs. This will help reduce avoidable admissions and improve long-term health outcomes.

* **Optimize provider network** Expand contracts in underserved regions and negotiate preferred pricing agreements with high-volume hospitals and pharmacies to minimize cost variation.

* **Support preventive care** Encourage policy holders to adopt wellness and preventive benefits, which are already linked to lower inpatient admission rates in certain groups.
