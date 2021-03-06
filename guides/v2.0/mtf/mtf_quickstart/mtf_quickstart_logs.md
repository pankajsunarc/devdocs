---
layout: default
group: mtf-guide
subgroup: 30_Quickstart
title: Quick start with the Functional Testing Framework
menu_title: See logs for failed tests
menu_order: 4
version: 2.0
github_link: mtf/mtf_quickstart/mtf_quickstart_logs.md
redirect_from: /guides/v1.0/mtf/mtf_quickstart/mtf_quickstart_logs.html
---

All failed tests are logged in `<magento2_root_dir>/dev/tests/functional/var/log`.

<div class="bs-callout bs-callout-tip">
  <p>This path is set in <code>&lt;magento2&gt;/dev/tests/functional/phpunit.xml</code>, element <code>&lt;env name="basedir" value="&lt;path_to_directory&gt;" /&gt;</code>.</p>
</div>

All Magento errors are logged in `<magento2_root_dir>/var/log`.
