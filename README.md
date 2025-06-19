
# AWS FinOps Cost Intelligence Dashboard

## Objective
To track and visualize daily AWS service-level spending, identify high-cost services, and uncover cost optimization opportunities using FinOps principles.

---

## Background

Cloud costs can spiral without visibility. By integrating AWS Cost Explorer with visual analytics, this dashboard empowers FinOps teams to monitor usage trends, detect anomalies, and support data-driven cloud budgeting.

---

## Tools & Technologies Used

- **AWS Cost Explorer API (boto3)** – Query cloud spend by service and date.
- **Python (pandas, matplotlib)** – Data wrangling and plotting.
- **Streamlit** – Interactive visual dashboard.
- **CSV Download** – Reporting feature for finance and engineering collaboration.

---

## Architecture

1. Query daily AWS cost data via `boto3.client('ce')`.
2. Group costs by **service type** and **date**.
3. Visualize cost trends and top consumers.
4. Allow CSV export of results.

---

## 📸 Screenshot

![AWS_FinOps_Dashboard_Annotated](https://github.com/user-attachments/assets/066cd0e9-7381-4ded-bba4-0f343f97dd98)




---

## Sample Insights

- S3 and EC2 accounted for 72% of spend in May 2024.
- Sudden spike in CloudWatch costs on May 14 due to log ingestion.
- Lambda remained under budget with < 1% overall cost impact.

---

## Skills Learned

- FinOps strategy and cost observability
- Service-level billing analysis using AWS Cost Explorer
- Python data analysis and visualization
- Streamlit-based dashboard design
- Identifying cloud waste and optimization opportunities
- Communicating cost insights between finance and engineering

---

## FinOps Principles Applied

- **Visibility**: Breakdown of spend per service and over time.
- **Optimization**: Spotting underutilized or overprovisioned resources.
- **Collaboration**: Exportable reports to align teams.
- **Forecasting**: Visual trends help anticipate budget shifts.

---

## 🔗 References

- [AWS Cost Explorer Documentation](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-explorer.html)
- [AWS Cost Explorer API (boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html)
- [FinOps Foundation](https://www.finops.org/)
- [AWS Billing CLI](https://docs.aws.amazon.com/cli/latest/reference/ce/)
