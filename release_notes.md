# What's New

1. **Introducing New Output Variable `recordIRIs`:**
   - We've introduced a new output variable called `recordIRIs` as an alternative to the existing `@id` for passing demo record IRIs from the records generation playbook to the scenario playbook.
   
        Going forward we'll be using the `recordIRIs` output variable for future releases.

2. **Handling Multiple Record Generation Playbooks:**
   - To handle scenarios with multiple record generation playbooks, we've updated the logic for collecting created record IRIs. Instead of a nested list, the IRIs are now stored as a single list in the *Created Records ID* field.

3. **Enhancing *Reset Scenario* Playbooks:**
   - The *Reset Scenario* playbooks have been enhanced to retain correlated MITRE records associated with the demo records. This ensures that relevant data is preserved during scenario resets.

4. **Update in *Run Scenario - Create Alerts* Playbook:**
   - In the playbook **Run Scenario - Create Alerts**, we've updated the value of `Parent Data Reference` field in the step *Launch Step Playbook* to `Input record only`.
