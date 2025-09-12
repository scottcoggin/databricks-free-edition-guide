# Databricks Free Edition Setup Instructions

## Overview

Databricks Free Edition is a serverless-only, quota-limited environment designed for learning, experimentation, and non-commercial use. Your workspace comes pre-configured with serverless compute and default storage, allowing you to begin working immediately.

## Prerequisites

- Valid email address
- Web browser (Chrome, Firefox, Safari, or Edge)
- Internet connection

## Getting Started

### 1. Sign Up for Databricks Free Edition

1. Visit the [Databricks Free Edition signup page](https://databricks.com/try-databricks)
2. Select your preferred signup method:
   - Email with one-time password (OTP)
   - Google account
   - Microsoft account
3. Complete the registration process
4. Your workspace is created immediately upon signup

### 2. Access Your Workspace

1. Log in to your Databricks account
2. You'll be taken to your workspace dashboard
3. Note your workspace URL for future access
4. No additional compute configuration is needed - serverless compute is ready to use

### 3. Create Your First Notebook

1. Go to "Workspace" in the sidebar
2. Click "Create" → "Notebook"
3. Name your notebook
4. Select your preferred language (Python or SQL)
5. The notebook automatically attaches to serverless compute

### 4. Verify Setup

Run this simple test in a new notebook cell:

```python
# Test cell
print("Hello Databricks!")
spark.sql("SELECT 'Setup Complete!' as status").show()
```

## What's Included

Free Edition provides access to:

- **Collaborative notebooks** - Real-time teamwork on data science projects
- **SQL editor** - Query and explore data interactively
- **Databricks Assistant** - In-product coding help with suggestions and fixes
- **Interactive dashboards** - Create visualizations via natural-language prompts with Genie
- **Data pipelines** - Design ingestion and transformation workflows
- **AI capabilities** - Data preparation and foundation model experimentation

## Limitations

Free Edition has several constraints to be aware of:

### Compute Limits
- Serverless compute only (no custom clusters or GPUs)
- All-purpose clusters limited to small sizes
- One SQL warehouse (max 2X-Small)
- Maximum 5 concurrent job tasks
- One active pipeline per pipeline type

### Feature Restrictions
- **Languages**: Python and SQL only (no R or Scala)
- **Authentication**: Email OTP, Google, or Microsoft only (no SSO/SCIM)
- Single workspace and metastore per account
- No account console or API access
- No private networking or custom security settings

### Usage Policies
- Non-commercial use only
- Fair usage policy enforced - exceeding quotas triggers daily compute shutdown
- Inactive accounts subject to deletion
- No SLA or official support coverage

## Useful Resources

- [Databricks Free Edition Documentation](https://docs.databricks.com/aws/en/getting-started/free-edition)
- [Free Edition Limitations](https://docs.databricks.com/aws/en/getting-started/free-edition-limitations)
- [Apache Spark Documentation](https://spark.apache.org/docs/latest/)
- [Databricks Community Forums](https://community.databricks.com)