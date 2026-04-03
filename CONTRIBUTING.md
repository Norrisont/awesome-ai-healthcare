# How to Contribute to Awesome AI for Healthcare

Thank you for helping make this list better! Anyone can contribute — you do not need to be an expert.

---

## Who Should Contribute?

- A developer who found a free FHIR library or health API
- - A researcher with a useful open dataset
  - - A clinician who knows a helpful clinical tool
    - - A startup founder sharing an open-source project
     
      - ---

      ## How to Add a Resource

      **Step 1 — Fork this repo**
      Click the **Fork** button at the top right of this GitHub page.

      **Step 2 — Edit README.md**
      Find the right section and add your resource in this format:

      ```
      - **[Tool Name](https://verified-link.com)** — One sentence on what it does.
        > *Why it matters: One sentence on real-world US healthcare impact.*
      ```

      **Example:**
      ```
      - **[OpenEMR](https://www.open-emr.org/)** — Free, ONC-certified EHR used by thousands of US clinics.
        > *Why it matters: The most accessible open-source EHR for community health centers.*
      ```

      **Step 3 — Open a Pull Request**
      Click Contribute then Open Pull Request. Use a short title like:
      `Add OpenEMR to EHR section`

      We review and merge within a few days.

      ---

      ## Rules

      - Link must be verified and working — test it before submitting
      - - Tool must be free, open-source, or have a meaningful free tier
        - - Must be relevant to US healthcare (HIPAA, Medicaid, FHIR, CMS)
          - - Plain English only — no unexplained jargon
            - - Must be actively maintained (last update within 2 years)
              - - No fully paid commercial tools
                - - No self-promotion without writing `[Disclosure: I built this]`
                 
                  - ---

                  ## Writing Good Descriptions

                  Write plainly — as if explaining to someone who is not a developer.

                  | Good | Bad |
                  |---|---|
                  | Reads chest X-rays and flags pneumonia | CNN-based pulmonary pathology detection engine |
                  | Free, HIPAA-compliant, used by 10,000+ US clinics | Enterprise-grade compliance-ready SaaS platform |
                  | Connects your app to Medicare patient data | Federated CMS beneficiary attribution API |

                  ---

                  ## Disclosing Your Own Projects

                  You are welcome to add your own open-source tools. Just add `[Disclosure: I built this]` at the end of your description so readers know.

                  ---

                  ## Fixing Broken Links

                  Fork the repo, fix the URL or remove the entry, then open a PR titled:
                  `Fix broken link: Tool Name`

                  ---

                  ## Suggesting New Sections

                  Open an **Issue** (not a PR), describe the section you want, and list 3 to 5 example resources you would include.

                  ---

                  ## Code of Conduct

                  Respectful and constructive conversation only. No discrimination of any kind.

                  ---

                  *Maintained by [Morris Kithinji](https://github.com/Norrisont) and contributors*
