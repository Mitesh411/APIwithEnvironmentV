# Postman API Automation Integration with GitHub Actions

This repository serves as a proof of concept (POC) for integrating Postman-based API tests with GitHub Actions in a continuous integration workflow.

All test cases are authored in Postman and executed on a virtual machine using Newman in combination with the `newman-reporter-htmlextra` plugin. GitHub Actions is configured to trigger the test suite:

* Automatically on every push to the `main` branch
* Manually via the `workflow_dispatch` event
* On a scheduled basis using a cron job

Upon completion of each run, the generated HTML report is archived and made available in the **Artifacts** section for team download and review.

## 🌐 GitHub Pages

You can directly view the latest test report of the Postman Test here:  

👉 [https://mitesh411.github.io/APIwithEnvironmentV/](https://mitesh411.github.io/APIwithEnvironmentV/)

In addition, the latest report is distributed to team members via email using Gmail SMTP, ensuring timely visibility of test results and overall API quality status.

---
