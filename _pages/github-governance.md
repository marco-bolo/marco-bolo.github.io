---
title: Github Governance
author: Marc Portier
date: 2023-08-07
layout: home
---

## Intro and Motivation

The various partners of the [Marco-Bolo project]({{ site.data.links.www }}) are independently using the [shared github space at marco-bolo]({{ site.data.links.gitorg }}). This page wants to arrange some clear and simple ways to:
* organize who does what over there.
* agree on some naming to keep surprise low
* provide essential documentation / overview
* help each other by avoiding needless inspiration into creative names and locations reducing overall findability


Also, through the usage of the [gh-pages feature](https://pages.github.com/), the repos could be easily building up a consistent behind-the-scenes collaborations oriented web-presence (targeting on data management, not competing with the current [project website]({{ site.data.links.www }}) at some selected hostname `https://{hostname}.marcobolo-project.eu/`

The starting point repository for that is already setup at [{{ site.data.links.gitrepo }}]({{ site.data.links.gitrepo }}) , but any extra repo can easily add on to the web-presence if deemed useful. This observation adds some extra useful elements to consider:
* for now we opted to use the [gitbook-theme](http://jekyllthemes.org/themes/gitbook/) to get some consistency
* we will need to do some management of the URI space

## User / Team Management

### Sign Up & Join

New people requesting to take up a role in the github space of marco-bolo should:
* make sure they [have a github-account](https://github.com/join)
* then pass the created github-account-name to this [request to join the team]({{ site.data.links.gitrepo }}/issues/1) 

### Teams

Teams allow for a manageable way to hand out permissins accross the repositories.
Currently [no teams]({{ site.data.links.gitorg }}/teams) have been set-up

## Naming Convention

### Top level rules

To achieve some consistency in appearance, and make sure people easily find what they look for:

* we only use lower case for repo names
* we use dashes `-` as demarcation between words (aka [Kebab case](https://www.theserverside.com/definition/Kebab-case))
  * exceptions:
    * dots are allowed in domain-name-like constructs (e.g. `marco-bolo.github.io`)
* avoid plural (so no trailing s) in folders and repo-names

### Suffixes in use to indicate type (or purpose) of the repository

By introducing these suffixes we know what to expect inside the repos

<div class="table-wrapper" markdown="block">

|repo suffix       | type / purpose of repo | expected content / workflow | comments | 
|-----------------:|:-----------------------|:----------------------------|:---------|
| `*-ontology`     | vocab terms and relations | - maintained ttl or jsonld <br>- to produce some published variant  | publication system to be decided  | 
| `*-data`         | | | publication system (like linkML) to be decided) | 
| `*-*-sandbox`    | playground try-out | in combination with one of the other suffixes | sounds logic to have some of those to start with provenance, linkml stuff, …. ?
| `*-catalogue`    | reference catalolgue of linkable stuff | | | 

</div>


## New github repositories

* Should be requested for by https://github.com/marco-bolo/marco-bolo.github.io/issues/
  * please introduce purpose
  * please indicate if the repo will be adding to the URI namespace through github-pages
* Should follow naming-convention
* Should provide a well managed top-level READMe.md

## Documentation 

Documentation on how to further organise this space will be managed through markdown `_pages` in [this very repo]({{ site.data.links.gitrepo }}) and made findable from here.


## Central Repo Listing

The full list of [available repositories]({{ site.data.links.gitorg }}/repositories) is produced by github automatically. 

If needed to further clarify a managed table-listing will be provided explaining further what the role and purpose of each repo in the organization is about.


## Agreement on remote large file storage

The size and amount of data to be stored in github is limited (and also somewhat defying use and purpose of the implicit version management).

No overall decision has been made on how to deal with these as of yet.


## Maintenance

### Proactive maintenance

Further maintenance of these guidelines and the actual gitub space will be taken up as part of the regular WP1 meetings.

At least every 6 months these should
* round up an overview of the space and suggest clean-up actions (to be tracked via github issues) 
  * to specific repository-owners 
  * to clean up, fix, comply to best practices and uniformity;
* update the policy if needed

Minutes of this should be part of the running document of WP1 meeting-minutes.

### Reactive maintenance

New complaints or suggestions about any of this or the practical repos in use should be addressed via [new github issues]({{ site.data.links.gitrepo }}/issues/new)
