# Use Case Description

Access by physician to patient's full medical history during one on one consultation.

For that:
- The patient has a [policy](policy-01.ttl) allows her health data to be read for primary care.
- The physician issues a [request](request-01.ttl) to read health data for primary care with consent as the legal basis.

TODO: The expected agreement , i.e., generated by matching policy and request, should also be part of this benchmark.

## Use Case Requirements:

- N/A - non applicable requirements
- TODO - we still need to think about how to integrate that into an ODRL policy
- TODO-EHDS - required to assess whether EHDS is applicable, still needs to be incorporated 

### Subject/holder policy

- Data subject: <https://example.org/patient>
- Data/Personal data: <https://example.org/health-data>
- Processing operation: `odrl:read`
- Purpose: `sector-health:PrimaryCareManagement`
- Pseudo/Anonymisation as a duty: N/A
- Recipient: N/A
- Duration: N/A
- Frequency: N/A
- Retrospective/prospective data: Both -- TODO

### Request

- Data controller: <https://example.org/physician>
- Data subject (type): <https://example.org/patient>
- Data/Personal data: <https://example.org/health-data>
- Personal electronic health data: TODO-EHDS
- Non-personal electronic health data: TODO-EHDS
- Processing operation: : `odrl:read`
- Purpose: `sector-health:PrimaryCareManagement`
- Primary/Secondary use: Primary -- still needs to be expressed in the policy though
- Legal basis: `eu-gdpr:A9-2-a`
- Pseudo/Anonymisation as a duty: N/A
- Recipient: N/A
- Data source: N/A
- Duration: N/A
- Frequency: N/A
- Events/Activities: N/A