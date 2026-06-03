# Splunk Universal Forwarder — Recommended Versions

**Last reviewed:** May 2026
**Scope:** Universal Forwarder (UF) only — not applicable to Heavy Forwarder or Splunk Enterprise
**Architecture:** x86_64 / x64 (64-bit) unless stated
**Sources:** Splunk official compatibility matrix · [Splunk Support Policy](https://www.splunk.com/en_us/support-and-services/support-programs.html)

---

## Status Key

| Label | Meaning |
|---|---|
| **Supported** | Actively supported — security patches issued by vendor |
| **EOL** | End of Life — vendor no longer issues security patches |
| **ELS** | Extended Life Support — paid Red Hat programme, limited patches |
| [UNTESTED] | Recommendation based on official compatibility matrix only — not independently verified. Test before deploying at scale. |

---

## Windows Universal Forwarder Recommendations

**Note:** Windows Server 2016, 2019, and 2022 all share the NT 10.0 kernel and use the same UF installer package.

**Official download page OS labels** (verified directly from Splunk previous releases page):

| UF Version | Official Windows Label |
|---|---|
| 10.2.3 | Windows 10, Windows Server 2019, 2022, 2025 |
| 9.4.11 | Windows 10, Windows Server 2019, 2022 |
| 9.3.12 | Windows 10, Windows Server 2019, 2022 |
| Older than 9.3 | Labels not available — previous releases page does not list them |

| OS Version | Microsoft Status | Recommended UF Version | Splunk Status | Notes | Download |
|---|---|---|---|---|---|
| Windows Server 2003 x86 (32-bit) | **EOL** Jul 2015 | **6.6.2** | **EOL** Oct 2019 | [UNTESTED] — label not verifiable (pre-9.3) | [splunkforwarder-6.6.2-x86-release.msi](https://download.splunk.com/products/universalforwarder/releases/6.6.2/windows/splunkforwarder-6.6.2-4b804538c686-x86-release.msi) |
| Windows Server 2003 x64 (64-bit) | **EOL** Jul 2015 | **6.6.4** | **EOL** Oct 2019 | [UNTESTED] — label not verifiable (pre-9.3) | [splunkforwarder-6.6.4-x64-release.msi](https://download.splunk.com/products/universalforwarder/releases/6.6.4/windows/splunkforwarder-6.6.4-00895e76d346-x64-release.msi) |
| Windows Server 2008 x64 | **EOL** Jan 2020 | **8.2.9** | **EOL** Oct 2023 | [UNTESTED] — label not verifiable (pre-9.3) | [splunkforwarder-8.2.9-x64-release.msi](https://download.splunk.com/products/universalforwarder/releases/8.2.9/windows/splunkforwarder-8.2.9-4a20fb65aa78-x64-release.msi) |
| Windows Server 2008 R2 SP1 x64 | **EOL** Jan 2020 | **9.3.12** | Supported ~Oct 2026 | [UNTESTED] — not in official 9.3.12 label | [splunkforwarder-9.3.12-x64-release.msi](https://download.splunk.com/products/universalforwarder/releases/9.3.12/windows/splunkforwarder-9.3.12-c3c164f2e6c4-x64-release.msi) |
| Windows Server 2012 x64 | **EOL** Oct 2023 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — not in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |
| Windows Server 2012 R2 x64 | **EOL** Oct 2023 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — not in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |
| Windows Server 2016 x64 | Supported Jan 2027 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — not in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |
| Windows Server 2019 x64 | Supported Jan 2029 | **9.4.11** | Supported ~Sep 2027 | Confirmed in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |
| Windows Server 2022 x64 | Supported Oct 2031 | **9.4.11** | Supported ~Sep 2027 | Confirmed in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |
| Windows Server 2025 x64 | Supported Oct 2034 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — not in official 9.4.11 label | [splunkforwarder-9.4.11-windows-x64.msi](https://download.splunk.com/products/universalforwarder/releases/9.4.11/windows/splunkforwarder-9.4.11-bbcbf19b5450-windows-x64.msi) |

### Windows EOL Warnings

> **Windows Server 2003 (x86 and x64)**
> Both Microsoft support (ended July 2015) and Splunk support (ended October 2019) have expired. These versions will not receive any further security patches from either vendor. These hosts should be decommissioned. Deploy at your own risk.

> **Windows Server 2008 (non-R2)**
> Microsoft support ended January 2020. Splunk 8.2.9 reached EOL October 2023. No security patches will be issued by either vendor. These hosts should be decommissioned.

> **Windows Server 2008 R2 SP1**
> Microsoft support ended January 2020 (ESU also expired). The OS will not receive further Microsoft security patches. Splunk 9.3.x remains within Splunk's support window (~October 2026), meaning Splunk vulnerabilities will still be patched — however the underlying OS will not be. Plan decommission or upgrade.

> **Windows Server 2012 and 2012 R2**
> Microsoft extended security updates (ESU) expired October 2023. The OS will not receive further Microsoft security patches. Splunk 9.4.x remains within Splunk's support window (~September 2027). Plan upgrade to Server 2019 or later.

> **Windows Server 2016**
> Microsoft support runs until January 2027. Windows Server 2016 does not appear in the official Splunk download page label for any version from 9.3.x onwards. The recommended version (9.4.11) should be tested before broad deployment.

---

## Red Hat Enterprise Linux (RHEL) Universal Forwarder Recommendations

**Note:** RHEL-compatible distributions — Oracle Linux (including UEK kernels), CentOS Stream, Rocky Linux, and AlmaLinux — share the same RPM package and compatibility as RHEL of the same major version.

| OS Version | Red Hat Status | Recommended UF Version | Splunk Status | Notes | Download |
|---|---|---|---|---|---|
| RHEL 5 (el5) | **EOL** Nov 2020 | **8.2.1** | **EOL** Oct 2023 | Below scope of this table (RHEL 6+) — included for completeness | [splunkforwarder-8.2.1-linux-x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/8.2.1/linux/splunkforwarder-8.2.1-ddff1c41e5cf-linux-2.6-x86_64.rpm) |
| RHEL 6 (el6) | **EOL** Nov 2024 | **9.0.3** | **EOL** Oct 2024 | | [splunkforwarder-9.0.3-linux-x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/9.0.3/linux/splunkforwarder-9.0.3-dd0128b1f8cd-linux-2.6-x86_64.rpm) |
| RHEL 7 (el7) | **ELS** until Jun 2026 | **9.3.12** | Supported ~Oct 2026 | Splunk 9.4.x does not support RHEL 7 — see warning below | [splunkforwarder-9.3.12.x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/9.3.12/linux/splunkforwarder-9.3.12-c3c164f2e6c4.x86_64.rpm) |
| RHEL 8 (el8) | Supported until May 2029 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — 9.4.11 compatibility with RHEL 8 not independently verified | [splunkforwarder-9.4.11.x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/9.4.11/linux/splunkforwarder-9.4.11-bbcbf19b5450.x86_64.rpm) |
| RHEL 9 (el9) | Supported until May 2032 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — 9.4.11 compatibility with RHEL 9 not independently verified | [splunkforwarder-9.4.11.x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/9.4.11/linux/splunkforwarder-9.4.11-bbcbf19b5450.x86_64.rpm) |
| RHEL 10 (el10) | Supported until May 2035 | **9.4.11** | Supported ~Sep 2027 | [UNTESTED] — 9.4.11 compatibility with RHEL 10 not independently verified | [splunkforwarder-9.4.11.x86_64.rpm](https://download.splunk.com/products/universalforwarder/releases/9.4.11/linux/splunkforwarder-9.4.11-bbcbf19b5450.x86_64.rpm) |

### RHEL EOL Warnings

> **RHEL 5 (el5)**
> Red Hat support ended November 2020. Splunk 8.2.x reached EOL October 2023. Neither vendor will issue further security patches. These hosts should be decommissioned urgently.

> **RHEL 6 (el6)**
> Red Hat ELS ended November 2024. Splunk 9.0.x reached EOL October 2024. Both vendor supports have now expired simultaneously. These hosts represent an elevated security risk and should be treated as urgent upgrade candidates.

> **RHEL 7 (el7)**
> Standard Red Hat support ended June 2024. Extended Life Support (ELS) is available as a paid Red Hat subscription until June 2026. Splunk 9.3.x remains within Splunk's support window (~October 2026) and will continue to receive security patches. Splunk 9.4.x does not support RHEL 7 (requires glibc 2.28 minimum; RHEL 7 ships glibc 2.17). Plan upgrade to RHEL 8+ before June 2026.

---

## Splunk Version End-of-Life Reference

| Splunk Version | Release Date | EOL Date | Notes |
|---|---|---|---|
| 6.x | Oct 2013 – Apr 2016 | Oct 2019 | All 6.x branches EOL simultaneously |
| 7.x | Sep 2017 – Sep 2019 | Oct 2021 | All 7.x branches EOL simultaneously |
| 8.0 / 8.1 | Oct 2019 / Oct 2020 | Apr 2022 / Apr 2023 | |
| 8.2 | Apr 2021 | Oct 2023 | |
| 9.0 | Sep 2022 | Oct 2024 | |
| 9.1 | Jul 2023 | Oct 2024 | |
| 9.2 | Jan 2024 | ~Oct 2025 | Approaching EOL — plan upgrades |
| 9.3 | Sep 2024 | ~Oct 2026 | Actively supported |
| 9.4 | Sep 2025 | ~Sep 2027 | Actively supported |
| 10.0 | Mar 2025 | ~Mar 2027 | Actively supported |
| 10.2 | Jan 2026 | ~Jan 2028 | Actively supported — latest release |

Splunk follows a standard 24-month support lifecycle per major.minor release. EOL dates marked with ~ are calculated from release date and should be verified against the [Splunk Support Policy](https://www.splunk.com/en_us/support-and-services/support-programs.html).

---

## Additional Platform Notes

### Other Linux distributions

The following Linux distributions use the same UF binary but are not covered in the RHEL table above. Use the `.tar.gz` package for SLES, `.deb` or `.tar.gz` for Ubuntu, and `.rpm` or `.tar.gz` for Amazon Linux.

| Distribution | Recommended UF | Vendor Status | Notes |
|---|---|---|---|
| SUSE Linux Enterprise Server (SLES) 9/10 | 8.2.1 | **EOL** SUSE | Splunk EOL. |
| SUSE Linux Enterprise Server (SLES) 11 | 9.0.3 | **EOL** SUSE | Splunk EOL. |
| SUSE Linux Enterprise Server (SLES) 12 | 9.3.12 | **EOL** SUSE (Jun 2024) | Splunk supported. |
| SUSE Linux Enterprise Server (SLES) 15 | 9.4.11 | Supported | |
| Ubuntu 12.04 / 12.10 / 14.04 | 8.2.1 | **EOL** Ubuntu | Splunk EOL. |
| Ubuntu 16.04 | 9.0.3 | **EOL** Ubuntu | Splunk EOL. |
| Ubuntu 18.04 | 9.3.12 | **EOL** Ubuntu (Apr 2023) | Splunk supported. |
| Ubuntu 20.04 | 9.4.11 | Supported | |
| Ubuntu 22.04 | 9.4.11 | Supported | |
| Ubuntu 24.04 | 9.4.11 | Supported | |
| Amazon Linux 2023 | 9.4.11 | Supported | |

---

*This document should be reviewed and updated when new Splunk releases are published or when OS vendor support dates change.*
