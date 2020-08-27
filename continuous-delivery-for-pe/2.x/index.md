# Continuous Delivery

-   [Welcome to Continuous Delivery for Puppet Enterprise](cd_user_guide.md)
-   [Release notes](release_notes_cdpe_index.md)
    -   [Continuous Delivery for PE release notes](cd_release_notes.md)
    -   [Continuous Delivery for PE known issues](known_issues_cdpe.md)
    -   [Release notes archive](release_notes_cdpe_archive.md)
-   [Getting started with Continuous Delivery for PE](getting_started.md#concept-9811)
    -   [Step 1: Install Continuous Delivery for PE](getting_started.md#getting_started_install)
    -   [Step 2: Create your user account and set up a workspace](getting_started.md#getting_started_user_and_workspace)
    -   [Step 3: Set up integrations and configure job hardware](getting_started.md#getting_started_integrations)
    -   [Step 4: Add a control repo](getting_started.md#task-3948)
    -   [Step 5: Set up a pipeline](getting_started.md#getting_started_default_pipeline)
    -   [Step 6: Set up an environment node group](getting_started.md#getting_started_environment_groups)
    -   [Step 7: Deploy changes to your nodes](getting_started.md#getting_started_deploy)
    -   [Step 8: Create an impact analysis report](getting_started.md#getting_started_impact_analysis)
-   [Installing](install_set_up.md)
    -   [System requirements](cd_system_requirements.md#concept-3479)
        -   [Continuous Delivery for PE architecture](cd_system_requirements.md#cd_architecture)
        -   [Hardware requirements](cd_system_requirements.md#hardware_requirements)
        -   [Supported external databases](cd_system_requirements.md#supported_external_databases)
        -   [Job hardware requirements](cd_system_requirements.md#job_hardware_requirements)
        -   [Supported Puppet Enterprise versions](cd_system_requirements.md#reference-8404)
        -   [Supported browsers](cd_system_requirements.md#reference-3315)
    -   [Install Continuous Delivery for PE from the PE console](install_pe_console.md#install_pe_console)
        -   [Install Continuous Delivery for PE from the PE 2019.2.x or 2019.1.x console](install_pe_console.md#install_pe_2019-1-x_console)
        -   [Install Continuous Delivery for PE from the PE 2018.1.8+ console](install_pe_console.md#install_pe_2019-0-3_or_2018-1-8_console)
        -   [Advanced configuration options](install_pe_console.md#advanced_configuration_options)
        -   [Automate upgrades of your Continuous Delivery for PE console installation](install_pe_console.md#cd_upgrade)
    -   [Install Continuous Delivery for PE using the cd4pe module](install_module.md#install_module)
        -   [Install Continuous Delivery for PE with the cd4pe module](install_module.md#install_with_module)
        -   [Configure Continuous Delivery for PE with a task](install_module.md#configure_task)
        -   [Advanced configuration options](install_module.md#advanced_configuration_options)
    -   [Generate a trial license](generating_a_license.md)
    -   [Alternative installation methods](alternative_installation_methods.md)
        -   [Install Continuous Delivery for PE using Docker](installing_continuous_delivery.md)
        -   [Configure a Continuous Delivery for PE module installation using classification](configure_classification.md#configure_classification)
            -   [Setting sensitive parameters in Hiera](configure_classification.md#sensitive_paramemters_hiera)
-   [Configuring and adding integrations](configuring.md)
    -   [Integrate with source control](integrations.md#integrations)
        -   [Integrate with Azure DevOps](integrations.md#integrate_azure_devops)
        -   [Integrate with Bitbucket Cloud](integrations.md#integrate_bitbucket_cloud)
        -   [Integrate with Bitbucket Server](integrations.md#integrate_bitbucket_server)
        -   [Integrate with GitHub](integrations.md#integrate_github)
        -   [Integrate with GitHub Enterprise](integrations.md#integrate_github_enterprise)
        -   [Integrate with GitLab](integrations.md#integrate_gitlab)
    -   [Integrate with Puppet Enterprise](integrate_with_puppet_enterprise.md#task-4324)
        -   [Create a Continuous Delivery user and user role in PE](integrate_with_puppet_enterprise.md#task-1594)
        -   [Add your Puppet Enterprise credentials](integrate_with_puppet_enterprise.md#task-7458)
    -   [Configure impact analysis](configure_impact_analysis.md#concept-4400)
        -   [Generate a dedicated Puppet Enterprise certificate](configure_impact_analysis.md#task-8916)
        -   [Install modules](configure_impact_analysis.md#task-3091)
        -   [Update classification](configure_impact_analysis.md#task-4402)
        -   [Add credentials to Continuous Delivery for PE](configure_impact_analysis.md#task-6154)
    -   [Configure job hardware](configure_job_hardware.md#concept-7483)
        -   [Configure job hardware with the web UI](configure_job_hardware.md#task-1714)
        -   [Configure job hardware with distelli.yml](configure_job_hardware.md#task-9198)
        -   [Configure global shared job hardware](configure_job_hardware.md#configure_global_shared_hardware)
        -   [Upgrade the Continuous Delivery agent](configure_job_hardware.md#task-369)
    -   [Analytics data collection](cd_analytics.md#concept-2956)
        -   [What data does Continuous Delivery for PE collect?](cd_analytics.md#concept-473)
        -   [Opt out of analytics data collection when installing with the cd4pe module](cd_analytics.md#task-4591)
        -   [Opt out of analytics data collection when installing with Docker](cd_analytics.md#task-2159)
    -   [Configure LDAP](configure_ldap.md#concept-9646)
        -   [Create a new LDAP configuration](configure_ldap.md#task-6946)
        -   [Create an LDAP group map](configure_ldap.md#task-4052)
    -   [Configure SMTP](configure_smtp.md)
    -   [Configure SSL](configure_ssl.md#concept-6026)
        -   [Setting up a new SSL configuration](configure_ssl.md#adding_ssl_configuration)
-   [Managing workspaces](managing_workspaces.md#managing_workspaces)
    -   [Best practices when creating workspaces](managing_workspaces.md#best_practices_creating_workspaces)
    -   [Set up a new workspace for a team](managing_workspaces.md#set_up_new_workspace)
-   [Testing Puppet code with jobs](example_jobs.md#concept-5714)
    -   [What is a job?](example_jobs.md#concept-7782)
    -   [Install job dependencies](example_jobs.md#task-300)
    -   [Pre-built job reference](example_jobs.md#reference-5355)
    -   [Sample non-Docker-based module jobs](example_jobs.md#reference-6550)
    -   [Sample non-Docker-based control repo jobs](example_jobs.md#concept-1237)
-   [Constructing pipelines](start_building_your_modules_pipeline.md#concept-9279)
    -   [Stages and tasks in pipelines](start_building_your_modules_pipeline.md#concept-9220)
    -   [Set up a pipeline](start_building_your_modules_pipeline.md#task-767)
    -   [Test code automatically with a pipeline](start_building_your_modules_pipeline.md#task-3463)
    -   [Test pull requests automatically](start_building_your_modules_pipeline.md#task-3835)
    -   [Deploy code automatically with a pipeline](start_building_your_modules_pipeline.md#task-8025)
-   [Previewing the impact of code changes](impact_analysis.md#concept-5425)
    -   [Add impact analysis to a control repo pipeline](impact_analysis.md#task-6946)
    -   [Add impact analysis to a module pipeline](impact_analysis.md#add_ia_module_pipeline)
-   [Deploying Puppet code](deploying_puppet_code.md)
    -   [Introducing deployments](introducing_deployments.md#concept-9880)
        -   [Git branches and Continuous Delivery for PE](introducing_deployments.md#concept-1698)
    -   [Create environment node groups](cd_environment_node_groups.md)
    -   [Deployment policies](deployment_policies.md#concept-8247)
        -   [Which deployment policy should I use?](deployment_policies.md#reference-7857)
        -   [Direct deployment policy](deployment_policies.md#concept-1274)
        -   [Temporary branch policy](deployment_policies.md#concept-5197)
        -   [Eventual consistency policy](deployment_policies.md#concept-2949)
        -   [Incremental branch policy](deployment_policies.md#concept-9080)
        -   [Blue-green branch policy](deployment_policies.md#concept-3340)
    -   [Deploy code manually](deploy_code_manually.md)
    -   [Deploy module code](deploy_module.md)
    -   [Require approval for deployments to protected Puppet environments](approval.md)
-   [Managing access](cd_managing_access.md)
    -   [Create a user account](create_a_user_account.md)
    -   [Adding users and creating groups](users_and_groups.md#concept-2720)
        -   [Add a user](users_and_groups.md#task-1680)
        -   [Create a new group](users_and_groups.md#task-3379)
        -   [Add or remove group members](users_and_groups.md#task-8482)
        -   [Assign permissions to a group](users_and_groups.md#task-9591)
        -   [Remove a user from a workspace](users_and_groups.md#task-7240)
    -   [Permissions reference](permissions_reference.md)
    -   [Using the root console](the_root_console.md#concept-8907)
        -   [Designate super users](the_root_console.md#task-6082)
        -   [Change a user's password](the_root_console.md#task-8056)
        -   [Reset a user's email address](the_root_console.md#task-9698)
-   [Upgrading to 3.x](upgrading_to_3_x.md)
