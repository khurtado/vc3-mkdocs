# VC3 User Guide

### Building Your First Virtual Cluster
**Prerequisites**

In order to use VC3, you’ll need an allocation or account in a target resource that is supported by VC3. These include, but are not limited to:

  - University of Chicago - Research Computing Center
  - University of Notre Dame - Center for Research Computing
  - Brookhaven National Laboratory - Scientific Data & Computing Center
  - Syracuse University - Research Computing
  - Texas Advanced Computing Center
  - NERSC
  - Amazon Web Services
  - Open Science Grid
  - and more!

Institutions and resources are added frequently - be sure to subscribe to our
newsletter and visit [Virtual Clusters](https://www.virtualclusters.org/community)!

### Login or Create Account

When you first visit [Virtual Clusters](https://www.virtualclusters.org), you’ll
be presented with a Login link in the top right of the screen. Click “Login” -
this will take you to a [Globus](https://globus.org) sign-in site.

![step1](../img/screenshot_272.png)

### Sign in to Globus

You will then be asked to sign in with your institutional identity, or your
Globus ID. If you are using the former, simply type in the name of your
institution and click “Continue”. Proceed to Step 3a.

Otherwise, click “Sign in with Globus ID” and proceed to the alternate Step 3b.

![step2](../img/screenshot_273.png)

## Login with your institutional ID

You should be presented with a login page for your institutional ID, with your
institution’s branding. Go ahead and sign-in now. 
**Note that your password is not sent to the VC3 or Globus web portals**. 
Continue to step 4.

![step3a](../img/screenshot_275.png)

## Login with your Globus ID

(_Alternative step - if you do not have an institutional ID supported by Globus_)

<– Globus ID page –>

## Complete or update your VC3 profile

Once you have signed in, you’ll be asked to update or complete your VC3 profile
with information such as your Institution and any other data we cannot
directly extract from your Globus account. Click “Update Profile” once done.

Note that other actions are not allowed until the profile is complete. 

The "SSH KEY" box can be used to upload your public ssh key. 
This will allow you to access your future clusters in the VC3 infrastructure.
Remeber: it is the **public** key what needs to be uploaded. 

If you do not have a public ssh key, 
instructions to create it can be found in the link at the top-right corner. 


![step4](../img/screenshot_276.png)

## Connect an Allocation

After updating your profile, you can connect an allocation to the VC3 service.
An allocation, in VC3, is defined as combination of a username and resource
target that consumes some type of compute unit - regardless of whether it is
billed as Service Units (many HPC centers), dollars (AWS, GCE), or priority
(HTCondor and other opportunistic systems).

Clicking My Allocations on the left shows all allocations currently associated
with your account. You may select a new one by clicking the "New Allocation" button.

![step5](../img/screenshot_277.png)

You will be able to select a resource target from the drop down menu, and enter
an account name for the resource. This is the same account name that you use to
SSH to the remote system.

![step5a](../img/screenshot_278.png)

In order to create a virtual cluster, the VC3 needs to be able to SSH
to the remote resource. 
Once you’ve connected your allocation, the system starts a process to validate it.

![step5b](../img/screenshot_279.png)

Follow the instructions.
You will be asked to login to the resource. 
Once there, just copy and paste the command that is displayed in the box "step 3".

![step5c](../img/screenshot_281.png)


![step5d](../img/screenshot_282.png)

This token allows the VC3 system to SSH into a cluster as yourself and submit
jobs on your, or your project’s, behalf.

## Defining a Project

VC3, as a platform for cooperative scientific computing, allows you create
projects to share your allocations and virtual clusters with trusted members of
your group, laboratory, or collaboration. To start a new project, click
“Projects” on the sidebar, then click “+ New Project”.

![step6](../img/screenshot_283.png)

You may give your project an arbitrary name and choose initial project members.
Once finished, click “Create Project”.

![step6a](../img/screenshot_284.png)

You should be returned to the Projects page, where you will be able to see all
of your projects and memberships.

![step6b](../img/screenshot_285.png)

## Creating a Cluster Template

VC3 allows users to create “Cluster Templates” that describe the components of
their virtual cluster, including the type of cluster, 
number of head nodes, worker nodes, etc. 
VC3 currently supports HTCondor and WorkQueue clusters with dynamic worker nodes,
and fixed head nodes.

To define a new template, click the “Cluster Templates” link on the left panel.
You’ll be able to give your cluster a name, select framework, and number of
workers. Click “Define Cluster Template” to finish creating the template.

![step7](../img/screenshot_286.png)

## Resources

The VC3 team curates an ever-expanding list of resources for end-users, with a
focus on Campus Clusters, HPC centers, and Cloud resources. You can find these
resources by clicking the “Resources” link on the left panel.

You can also click an individual resource and see expanded information, such as
batch system type, links to documentation, etc.

## Launching a Virtual Cluster

Now that you have created a Project and associated at least one allocation to it,
you are ready to create and launch your clusters.
