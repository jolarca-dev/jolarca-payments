## Description

<!-- What does this change do? Why is it needed? -->

## PCI-DSS Impact

<!-- Which PCI-DSS requirement(s) does this change affect? -->
<!-- Example: Req. 3 (data protection), Req. 6.3 (change control), Req. 11 (testing) -->

- [ ] This change affects PCI-DSS requirements (check all that apply)
  - [ ] Req. 1 (network segmentation)
  - [ ] Req. 3 (data protection)
  - [ ] Req. 4 (encryption in transit)
  - [ ] Req. 6 (secure development / change control)
  - [ ] Req. 7 (access control)
  - [ ] Req. 8 (authentication)
  - [ ] Req. 10 (logging/monitoring)
  - [ ] Req. 11 (security testing)
  - [ ] Req. 12 (policy / incident response)

## Change Request

<!-- Link to the change request issue or document this PR addresses -->
<!-- Per CONTRIBUTING.md, all changes require a documented change request (PCI-DSS Req. 6.3) -->

Issue: #

## Compliance Gate Checklist

<!-- All boxes must be checked before merge -->

- [ ] **Secret scan**: `security` CI context is green (gitleaks full-history scan)
- [ ] **Code quality**: `ci` CI context is green (ruff, mypy, pytest, yamllint)
- [ ] **No secrets**: No credentials, tokens, keys, or cardholder data committed
- [ ] **No PAN**: No Primary Account Numbers anywhere in the repository
- [ ] **Documentation**: README/CONTRIBUTING updated if this change affects policy
- [ ] **Linear history**: PR will be squash-merged (one logical change)

## Additional Notes

<!-- Any other context, risks, or follow-up work -->
