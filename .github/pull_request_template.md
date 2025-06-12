# Description

<!--
Describe what your PR does.  Please do not leave this blank!
This PR [adds/removes/fixes/replaces] the [feature/bug/etc].
-->

# Related Tickets & Documents

[Jira Ticket](https://hiddenlayersec.atlassian.net/browse/<XX-XXXX>)

# API Design Review Checklist

- [ ] I have referred to our [API Design Guidelines](https://hiddenlayersec.atlassian.net/wiki/spaces/HIDDENLAYE/pages/1366097944/REST+API+Guidelines+-+Condensed) and believe that this PR follows our conventions correctly.
  - The [REST API Review Checklist](https://hiddenlayersec.atlassian.net/wiki/spaces/HIDDENLAYE/pages/1366097957/REST+API+Review+Checklist) provides a concise list of key things to look for.
- [ ] Any exceptions to the guidelines are documented in the code and/or mentioned below.
- [ ] I have generated derefenced json files for my changes
  - If you don't see the generated files, you can run `npm ci` to install githooks so this to happens for you automatically on commits or you can run `npm run deref:json` manually.
- [ ] If changes were made to the `generated/api-deref-json/v3/model-scanner-hl-sor.json` file, I have [prepped contract tests in hiddenlayer-sor for this and confirmed the tests pass in that repository](https://github.com/hiddenlayer-engineering/hiddenlayer-sor/blob/main/README.md#how-do-i-get-set-up).
  - This is so I can quickly merge the updated tests and avoid blocking hiddenlayer-sor PRs for an extended period of time.
  - Any change to `generated/api-deref-json/v3/model-scanner-hl-sor.json` will require a [version bump of this file](https://github.com/hiddenlayer-engineering/hiddenlayer-sor/blob/main/tests/contract-tests/contract-version.txt), some changes will require the tests to be refactored.
  - See our [confluence documentation for more information on our contract testing approach and common issues you may run into](https://hiddenlayersec.atlassian.net/wiki/spaces/HIDDENLAYE/pages/622919686/Test+Approach+Contract+Test).

## Exceptions to the Guidelines

<!--
If you have any purposeful exceptions that go against our API design guidelines, mention them here.
Would be best if they were also explained in comments in the API docs directly.
-->
