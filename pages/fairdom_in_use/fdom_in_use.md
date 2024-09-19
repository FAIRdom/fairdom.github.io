---
title: FAIRDOM-SEEK In Use
toc: false
redirect_from: 
 - /instance
 - /fairdom_in_use
---

The [FAIRDOM-SEEK](/fairdom-seek) platform enables the building of Project Hubs where investigators can store, share, access, connect and interact with digital objects generated from their research, and use them in their own analyses.

Each Hub draws on the common features of the FAIRDOM-SEEK platform in different ways, configuring and customising its look, organisation and content. The FAIRDOM-SEEK has an organisational structure based on the [ISA](https://isa-tools.org/format/specification.html) model. Hubs commonly customise this. For example:

- [FAIRDOMHub](/fairdomhub) projects are based on the ISA. 
- [WorkflowHub](/fairdom-in-use/workflowhub) “teams” replace projects and the ISA is not used at all.

Each Hub positions itself in a different place in the project asset management pipeline, depending on their different characters. For example:

- [IBISBAKHub](/fairdom-in-use/ibisbakhub) is chiefly used for private collaborations between project partners and for handing over data and models between facilities during the execution of a project.
- [FAIRDOMHub](/fairdomhub) is a Hub used for collaborations and public publishing of results, as well as long term retention of outputs after projects have been completed, relying on the FAIRDOM Alliance to look after them. 
- [MIT  BioMicroCentre](https://openwetware.org/wiki/BioMicroCenter) uses a private hub within the MIT facility to coordinate project management during the running of a project and then pushes the outputs to the FAIRDOMHub in a final publishing step.

**Take a look at the Hubs and Projects below** and see the different ways that FAIRDOM-SEEK is configured to suit different needs.

<div class="row navigation-tiles">
    <div class="col" >
        <div class="card card-tall">
                <a class="stretched-link" aria-label="Go to the FAIRDOM-SEEK Hubs page" href="/fairdom-in-use/fairdom_hubs_search">
                    <h3 class="card-title m-0"><i class="fa-solid fa-folder-tree"></i> FAIRDOM-SEEK Hubs</h3>
                </a>
        </div>
    </div>
    <div class="col" >
        <div class="card card-tall">
                <a class="stretched-link" aria-label="Go to the FAIRDOM-SEEK Projects page" href="/fairdom-in-use/fairdom_projects_search">
                    <h3 class="card-title m-0"><i class="fa-solid fa-folder-tree"></i> FAIRDOM-SEEK Projects</h3>
                </a>
        </div>
    </div>
    <div class="col" >
        &nbsp;
    </div>
</div>


{% comment %} 
include section-navigation-tiles.html type="fairdom_in_use_search"

* [FAIRDOM Hubs in use]({{'/fairdom-in-use/fairdom_hubs_search' | relative_url}})
* [FAIRDOM Projects in use]({{'/fairdom-in-use/fairdom_projects_search' | relative_url}})
Include relative_url filter above so that internal URLs still work
in dev site GitHub Pages, where the whole site is hosted within a folder,
not the root URL.
{% endcomment %}