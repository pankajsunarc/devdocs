<div markdown="1">
 
## Install the Magento software
You can get Magento Community Edition 2.1 from Github, Composer, or using a compressed archive. 

See one of the following sections for more information:

*	[Get the Magento CE software using Composer](#install-rc-composer)
*	[Get a compressed archive](#install-archive)
*	[Get the Magento CE software from GitHub](#install-rc-gh)
*	[Complete the installation](#install-finish)

### Get the Magento CE software using Composer {#install-rc-composer}
{:.no_toc}

The CE software is available from `repo.magento.com`. Before getting the CE software, familiarize yourself with the Composer metapackage  <a href="{{page.baseurl}}install-gde/prereq/integrator_install.html" target="_blank">prerequisites</a>, then run 

	composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition=<version> <installation directory name>

where `<version>` is `2.1.0`, `2.1.1`, and so on

For example, to install Magento CE 2.1.1 in the `magento2` directory:

	composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition=2.1.1 magento2

### Get a compressed archive {#install-archive}
{:.no_toc}

{% include install/releasenotes/get-ce-software_zip.md %}

### Get the Magento CE software from GitHub {#install-rc-gh}
{:.no_toc}

<div class="bs-callout bs-callout-warning">
    <p>If you clone the Magento 2 GitHub repository, you <em>cannot</em> use the Magento software in a production environment. You cannot have a live store that accepts orders and so on.</p>
</div>

Before proceeding, please familiarize yourself with these prerequisites, then run

	git clone git@github.com:magento/magento2.git
	cd magento2
	git checkout tags/<version> [-b <version>]

where 

`<version>` is `2.1.0`, `2.1.1`, and so on

`[-b <version>]` optionally checks out a new branch.


### Complete the installation {#install-finish}
{:.no_toc}

After you get the CE software:

1.	[Set file system ownership and permissions]({{ page.baseurl }}install-gde/prereq/file-system-perms.html).
2.	Install the software:

	*	[Web Setup Wizard]({{ page.baseurl }}install-gde/install/web/install-web.html)
	*	[Command line]({{ page.baseurl }}install-gde/install/cli/install-cli.html)

## Upgrade from an earlier version
See the following sections for more information.

### Upgrade an existing installation from the GitHub repository {#upgrade-github}
{:.no_toc}

Developers who contribute to the CE codebase can <a href="{{page.baseurl}}comp-mgr/bk-compman-upgrade-guide.html" target="_blank">upgrade manually</a> from the Magento CE GitHub repository.

1.	Go to the <a href="{{page.baseurl}}install-gde/install/cli/dev_update-magento.html" target="_blank">Contributing Developers</a> page.

2.	Follow the instructions to pull the updates from the repository and update using Composer.

### Other upgrades {#upgrade-other}
{:.no_toc}

Other types of upgrades are discussed in [Upgrade to Magento version 2.1 (June 22, 2016)]({{page.baseurl}}release-notes/tech_bull_21-upgrade.html).