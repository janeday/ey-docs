# How to monitor your Engine Yard applications with New Relic

#### Introduction

New Relic is a tool for monitoring web application performance — from the end-user experience down to a line of application code. 

You get real data about your users. For example, you can see what countries your users are in, what browsers they use, how long they wait for pages to download. You get trending data; is your application is faster or slower this week than last week? When problems occur, you can get a transaction response performance breakdown and view a detailed timeline of an individual request.    

**Note:** New Relic Standard is free for AppCloud customers.

#### Process for setting up and using New Relic to monitor your application

1. [Choose a New Relic plan] [1]
2. [Configure your application for monitoring] [2]
3. [View New Relic performance data for your application] [3]

---

<h2><a id="topic1"> Choose a New Relic plan</a></h2>

#### Introduction

The first task in setting up New Relic is to choose the plan you want. The Standard plan is free with your Engine Yard account. But, you might decide that the Professional plan better suits you needs. 

#### To choose a New Relic plan

1. In AppCloud, click Account > Account Settings.
    
2. Click your account name.

3. Under the Services section at the bottom of the Account page, click Manage your New Relic plan.

    ![New Relic logo under Services](images/new_relic_logo.png)

3. Read and agree to the New Relic Terms of Service and select the check box. 
  
    ![Figure 2](images/choose_a_plan.jpg)

	<!-- this figure needs to be updated when the UI is updated -->
	
	Choose Bronze for the Standard plan or Gold for the Professional plan. (Our website will be updated soon to reflect the new plan names.)
	
    
5. Activate a plan.

Your New Relic account is created automatically using your Engine Yard account and password. 

If you selected the Professional plan, the New Relic charge appears on your AppCloud account bill; you won't get a separate bill from New Relic.

---

<h2><a id="topic2"> Configure your application for monitoring</a></h2>

#### Introduction

There are three parts to configuring your application:  

  * [Install the newrelic gem.] [A]  
  * [Edit your environment.rb file or your Gemfile.] [B]  
  * [Enable New Relic monitoring in AppCloud.] [C]

<h4><a id="topicA"> To install the newrelic_rpm gem</h4> </a>

1. In AppCloud, click Dashboard.
2. Click the Applications *tab*.
3. Click the Add Rubygems icon. 

    ![add rubygems icon](images/add_ruby_gem.png)

4. Search for the newrelic_rpm gem and add it to your selected gem list.

    ![newrelic rpm 3.0.1 gem selected](images/newrelic_rpm_gem_selected.png)

<!-- 2011.06.03 JD says: at some later date replace the above with a cross-reference to the generic process of adding a gem -->

<h4><a id="topicA"> To edit environment.rb or Gemfile</h4> </a>

1. Do one of the following to add the newrelic_rpm gem:

    * For Rails 3 and installations using Bundler, add the gem to your Gemfile.

    * For Rails 2.0 and Rails 2.1 to 2.3 without Bundler, edit your environment.rb file.

    For details, see the [[New Relic Knowledge Base about installing the gem.|  http://support.newrelic.com/kb/ruby/ruby-agent-installation-gem]]

<h4><a id="topicC"> To enable your application for New Relic monitoring</h4> </a>

1. In AppCloud, click Dashboard.
2. Click the Applications *link*.
3. Click the pencil icon.

    ![pencil icon](images/pencil_icon.png)

3. At the bottom of this page, select the check box to Enable New Relic Monitoring.

    ![Enable New Relic Monitoring check box](images/enable_new_relic_monitoring.png)

4. Deploy your application.

---

<h2><a id="topic3"> View New Relic performance data for your application</a></h2>

#### Introduction

The goal is to monitor your application through the New Relic dashboard. When you are signed on to AppCloud, SSO lets you click through to view your New Relic data.

#### To view New Relic data for your application

1. In AppCloud, click Account > Account Settings.
  
    ![Account Settings page](images/services-1.png)
  
2. Click the account name.

3. Under the Services section, click the New Relic logo.

    ![New Relic logo under Services now activated](images/new_relic_logo_activated.png)

4. Click the link to login and view your performance data.

    This links to New Relic website where you can review your data.

---


  [1]: #topic1        "topic1"
  [2]: #topic2        "topic2"
  [3]: #topic3        "topic3"
  [A]: #topicA        "topicA"	
  [B]: #topicB        "topicB"
  [C]: #topicC        "topicC"