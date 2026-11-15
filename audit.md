# EU AI Act Audit: ChatGPT Analysis of the Online Retail Dataset

Audit date: 11 November 2026

| Field | Detail |
| --- | --- |
| Workflow | chatgpt-online-retail-analysis |
| Risk tier | Minimal: general-purpose AI used for a classroom data analysis exercise with no decisions about people |
| Owner | Student (me), as part of a Big Data course |
| Frequency | One-off class exercise |
| Last audit | 2026-11-11 |

## Use case

I used ChatGPT to explore and interpret the "Online Retail" dataset (transactions from a UK-based, non-store online retailer, 2010 to 2011, published by the UCI Machine Learning Repository and mirrored on Kaggle as "E-Commerce Data"). This was an in-class exercise for a Big Data course, looking at how AI tools can help interpret large data files. My role under the Act is a user of a general-purpose AI system (a deployer in a learning context); OpenAI is the provider.

## Risk classification

Minimal risk. The output does not decide anything about anyone's rights, money, health, jobs, or access to services, and none of the uses fall under Article 5 (prohibited practices) or Annex III (high-risk areas). No fundamental rights impact assessment is needed. The transparency duties for chatbots (Article 50) sit with OpenAI as the provider. The remaining relevant duty is AI literacy (Article 4), which falls on the course provider.

## Obligations that apply

- AI literacy (Article 4): users should understand the tool's capabilities and limits, including that its calculations can be wrong.
- GDPR still applies alongside the AI Act: CustomerID is pseudonymised, so it is still personal data.
- No high-risk obligations (risk management, human oversight, logging, FRIA) apply to this use.

## Five-point hygiene check

| Check | Result | Evidence |
| --- | --- | --- |
| Bias | FAIL | Around 90% of transactions are from UK customers, and there is no recorded check of this skew before drawing conclusions from the data. |
| Privacy | PASS | No names or contact details; CustomerID is pseudonymised. It still counts as personal data under GDPR, so it should be handled with care. |
| Consent | PASS | The data is used within its public release for research and education (UCI, CC BY 4.0); the legal basis for collecting it sits with the publisher. |
| Attribution | FAIL | The work does not record a citation for the dataset (Chen, Sain and Guo, 2012, UCI) or say which ChatGPT model was used and when. |
| Transparency | PASS | The only audience is the class and the instructor, who know the work was done with AI. |

## Remediation (do these in order)

1. Add a source and AI-use statement to the submission: cite the dataset (Chen, Sain and Guo, 2012, UCI Machine Learning Repository) and name the ChatGPT model, the date, and what it was asked to do.
2. Check the bias: report the share of rows per country, and state that the conclusions describe UK customers or caveat them for other markets.
3. Verify ChatGPT's figures by re-running the key calculations (totals, top products, returns) yourself in Python or Excel, and note any differences.
4. Before uploading any dataset next time, turn off "Improve the model for everyone" in ChatGPT's data controls, and do not upload data that is not already public.

## Note

This is general education on the EU AI Act, not legal advice.
