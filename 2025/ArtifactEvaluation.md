---
layout: default2025
title: Artifact Evaluation
published: true
---

SLE’25 implements a two-rounds review process that also evaluates the quality of the artifacts supporting accepted research papers. This is the Artifact Evaluation track.

Authors of research and tools paper accepted for SLE 2025 will be invited to submit artifacts.  
In the context of the SLE community, an artifact refers to any digital object that supports, complements, or is a result of research in the field of software language engineering.  
This includes, but it is not limited to, tools, language grammars, metamodels, codebases, transformation scripts, formal proofs, benchmarks, datasets, statistical analyses, and surveys.  

The submitted artifacts will be reviewed by a dedicated Artifact Evaluation Committee. The approved artifacts will then be made first-class bibliographic objects, easy to find and cite.  
Depending on the quality of the artifact, the artifact might be awarded with different kinds of “badges” that are visible on the final paper.

The submission is optional and it is additional to your already accepted paper at SLE’25. It will not have a negative impact.

Artifacts provide tangible evidence of results, enable reproducibility, and encourage reuse and extension by the community.

---

## Artifact Review Process:

Submitted artifacts will go through a two-phase evaluation.

1. **Kick-the-tires**:  
   Reviewers check the artifact integrity and look for any possible setup problems that may prevent it from being properly evaluated  
   (e.g., corrupted or missing files, VM won’t start, immediate crashes on the simplest example, etc.).  
   Authors are informed of the outcome and will be given a 5-day period to read and respond to the kick-the-tires reports of their artifacts.  
   During the author response period, interactive discussions between reviewers and authors will be possible through HotCRP.

2. **Artifact assessment**:  
   Reviewers evaluate the artifacts, checking if they live up to the claims the authors make in the accompanying documentation.

---

## Artifact Preparation Guidelines

At a high level, we are interested in artifacts that:

- Have no dependencies. Use of docker images is strongly recommended. Virtual machine images in OVF/OVA format containing the artifact can also be provided.
- Have a minimal number of setup steps. Ideally, it should just be importing the docker/VM image.
- Have a short run, so that reviewers can try first before carrying the full review (kick-the-tire).
- Have a push-button evaluation. Ideally, the evaluation can be run through a single script, which performs the computation and generates the relevant figures/experimental data presented in the paper.  
  The evaluation should either display progress messages or expected duration should be provided.  
  This fully automated approach may be a bit more costly to set up, but you won’t have any copy/pasting issues for your paper, and regenerating data is heavily simplified.
- Include some documentation on the code and layout of the artifact.
- Use widely supported open formats for documents, preferably CSV or JSON for data.
- Document which outputs are associated with which parts of your paper, if possible, please specify table, figure, or sub-sections.

The artifact evaluated by the AEC and linked in the paper must be precisely the same.  
AEC Chairs will assure that DOIs point to the specific version evaluated. To create a DOI, you can use platforms like [Zenodo](https://zenodo.org/), [FigShare](https://figshare.com/) or [OSF](https://osf.io/), which offer free DOI creation.

**PDF and artifact should NOT be anonymized anymore.**

### Authors are strongly discouraged from:
- Downloading content over the internet during experiments or tests;
- Using closed-source software libraries, frameworks, operating systems, and container formats; and
- Providing experiments or tests that run for multiple days. If the artifact takes several days to run, we ask that you provide us with the full artifact and a reduced input set  
  (in addition to the full set) to only partially reproduce your results in a shorter time.  
  If the artifact requires special hardware, please get in touch with the AEC chairs, let us know of the issue, and provide us with (preferably SSH) access to a self-hosted platform for accessing the artifact.

---

## Artifact Submission Guidelines:

Every submission must include the following.  
Authors must submit a single artifact for a paper (1-to-1 mapping, paper-to-artifact).

- A **DOI** for downloading the artifact.
- A **PDF version** of the accepted paper for evaluating the artifact-paper consistency.
- A **Markdown-formatted file** providing an overview of the artifact. **PLEASE USE THE AUTHORS TEMPLATE:**  
  [https://doi.org/10.5281/zenodo.14975264](https://doi.org/10.5281/zenodo.14975264)

Artifact submissions will be handled through the HotCRP submission system at the following link:  
[https://sle25ae.hotcrp.com/](https://sle25ae.hotcrp.com/)

**NOTE:** The artifact can be associated with a different set of authors (different from the accepted paper).

---

## Quality Criteria

Submitted artifacts will be evaluated by the AEC concerning the following criteria.  
Depending on the criteria, different Badges are assigned (we limit ourselves to the ‘Evaluated’ and ‘Available’ badges).

---

### Artifact Evaluated (Badges)

There are two quality levels of the ‘Evaluated’ badge:

#### **Artifact Evaluated - Functional (Badge)**  
<img src="https://www.acm.org/binaries/content/gallery/acm/publications/artifact-review-v1_1-badges/artifacts_evaluated_functional_v1_1.png" width="100" height="100">

> “The artifacts associated with the research are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation."

- **Documented**: At minimum, an inventory of artifacts is included, and sufficient description provided to enable the artifacts to be exercised.
- **Consistent**: The artifacts are relevant to the associated paper and contribute in some inherent way to the generation of its main results.
- **Complete**: To the extent possible, all components relevant to the paper in question are included.
- **Exercisable**: Included scripts and/or software used to generate the results in the associated paper can be successfully executed.

---

#### **Artifact Evaluated - Reusable (Badge)**  

<img src="https://www.acm.org/binaries/content/gallery/acm/publications/artifact-review-v1_1-badges/artifacts_evaluated_reusable_v1_1.png" width="100" height="100">

> “The artifacts associated with the paper are of a quality that significantly exceeds minimal functionality.  
> That is, they have all the qualities of the Artifacts Evaluated – Functional level, but, in addition, they are very carefully documented and well-structured to the extent that reuse and repurposing is facilitated."

---

#### **Artifact Available (Badge)**  

<img src="https://www.acm.org/binaries/content/gallery/acm/publications/artifact-review-v1_1-badges/artifacts_available_v1_1.png" width="100" height="100">

> “Author-created artifacts relevant to this paper have been placed on a publicly accessible archival repository.  
> A DOI or link to this repository along with a unique identifier for the object is provided.”

---

## Important Dates (Authors):

- **Artifact submission Deadline**: 23.04.2025 (AoE)
- **Start Kick-the-Tires author response period**: 29.04.2025 (AoE)
- **End Kick-the-Tires author response period**: 02.05.2025 (AoE)
- **Author artifact Notification**: 01.06.2025 (AoE)


## Important Dates (PC Members):

- **Artifact submission deadline**: 23.04.2025 (AoE)  
- **Artifact bidding**: 24-26.04.2025  
- **Camera-ready deadline for SLE papers**: 01.05.2025 (AoE)  
- **Kick-the-Tires review deadline**: 29.04.2025 (AoE)
- **Kick-the-Tires response deadline**: 02.05.2025 (AoE)  
- **Final review deadline**: 24.05.2025 (AoE)  
- **Artifact discussion**: 25-31.05.2025  
- **Artifact notification**: 01.06.2025 (AoE)  


---

## Awards

The **Distinguished Artifact** award will be presented to the artifact that most significantly exceeds expectations.  
This recognition is determined by the AEC chairs based on the recommendations of the artifact evaluation committee.

---

## Any Questions?

For further information on the artifact evaluation of SLE 2025, feel free to contact the artifact evaluation chairs.

**Best regards,**  
**Idriss Riouak and Jeff Smits**  

- **Idriss Riouak**: [idriss.riouak@cs.lth.se](mailto:idriss.riouak@cs.lth.se)  
- **Jeff Smits**: [j.smits-1@tudelft.nl](mailto:j.smits-1@tudelft.nl)
