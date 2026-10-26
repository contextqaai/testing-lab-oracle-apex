# Oracle APEX Customers: browser workflow

Status: public installable sample and exercises; no workspace import or live run verified.

Use the Customers starter under `starter-apps/customers`. Match this branch's APEX version to the target workspace; do not assume a newer export imports into an older runtime. Follow the [original import instructions](../starter-apps/customers/readme.md) using App Builder or the supported SQLcl path. Preserve UPL and third-party notices.

A compatible APEX workspace, schema and dedicated test identity are needed before the app has a crawlable URL. An APEX Customers exercise does not demonstrate Fusion ERP, EBS or Oracle Forms. Publishing/import rights and fixture cleanup must be established separately.

## Proposed assertions

1. **Create customer:** A synthetic customer is saved and can be found after navigating away and back.
2. **Search and filter:** The chosen fixture appears under its matching customer report filter.
3. **Contact association:** A synthetic contact is associated with the intended customer.
4. **Activity history:** The selected synthetic activity is visible under that customer.
5. **Required-field validation:** The chosen required field is enforced without saving an incomplete record; verify the configured rule before running.

Use synthetic data. Start with read-only navigation, review generated actions, then authorize writes against disposable fixtures. Capture app export version, build/commit, workspace version, role, fixture, assertions and actual report. Private credentials and tenant URLs stay out of public issues. No ContextQA evidence is included yet.
