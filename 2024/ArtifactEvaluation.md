---
layout: default2024
title: Artifact Evaluation
published: true
---
SLE'24 implements a two-rounds review process that also evaluates the quality of the artifacts supporting accepted research papers. This is the Artifact Evaluation track.

Authors of research papers accepted for SLE 2024 will be invited to submit artifacts. Any kind of artifact that is presented in the paper can be submitted (tools, grammars, metamodels, models, programs, algorithms, scripts, proofs, datasets, statistical tests, checklists, surveys, interview protocols, visualizations, annotated bibliographies, and tutorials).

The submitted artifacts will be reviewed by a dedicated Artifact Evaluation Committee (AEC). The approved artifacts will then be made first-class bibliographic objects, easy to find and cite. Depending on the quality of the artifact, the artifact might be awarded with different kinds of “badges” that are visible on the final paper.

The submission is additional to your already accepted paper at SLE24. It will not have a negative impact.

The artifact evaluation process of SLE borrows heavily from processes described at [www.artifact-eval.org](https://www.artifact-eval.org).

##  Submission and Reviewing Process

* You need an accepted paper at SLE24.
* Use this submission page: https://sle24ae.hotcrp.com/paper/new
* You need to submit a PDF version of your paper for evaluating the artifact-paper consistency.
* The artifact can be associated with a different set of authors (different from the paper). 
* You require a copy of the abstract of the paper.
* We require a single artifact for each paper (1-to-1 mapping paper-and-artifact).
* Artifacts can be provided as zip or DOI.
* The artifact provided and evaluated must be precisely the artifact linked in the paper. We assure that the DOI points to the specific version, or that the SHA of the linked content is the same.
* The PDF and artifact should NOT be anonymized anymore.
* The process includes a Kicking-the-tires stages (close to a rebuttal): Reviewers report possible problems that may prevent artifacts from being properly evaluated. Authors will be given three days to read and respond to the kick-the-tires reports of their artifacts and solve any issues preventing the artifact evaluation (potentially resubmitting artifacts). Thereafter, the actually reviewing takes place.

##  Quality Criteria
Submitted artifacts will be evaluated by the AEC concerning the following criteria. Depending on the criteria, different Badges are assigned (we limit us the 'evaluated' and 'available' badge).

### Artifacts 'Evaluated' (Badge)

* **Documented**: At minimum, an inventory of artifacts is included, and sufficient description provided to enable the artifacts to be exercised.

* **Consistent**: The artifacts are relevant to the associated paper, and contribute in some inherent way to the generation of its main results.

* **Complete**: To the extent possible, all components relevant to the paper in question are included. (Proprietary artifacts need not be included. If they are required to exercise the package, then this should be documented, along with instructions on how to obtain them. Proxies for proprietary data should be included to demonstrate the analysis.)

* **Exercisable**: Included scripts and/or software used to generate the results in the associated paper can be successfully executed, and included data can be accessed and appropriately manipulated.

### Artifacts 'Available' (Badge)

* **Identification**: Using DOIs to identify published objects is standard. It is important to use a DOI that points to the specific version with which the results of the paper can be reproduced (for Zenodo: do not use the "always latest" DOI; for FigShare: use a DOI with a version suffix, e.g., ".v1").

* **Long-Term Availability**: It is necessary that the artifacts are archived in an archive that hosts the artifacts on a long-term basis, such as in digital libraries of the ACM, Zenodo, etc. (version repositories do not fulfill this requirement, as the hosting company could decide at any time to discontinue the service, as done by Google, for example: Google Code).

* **Immutability**: It is necessary that the artifact cannot be changed after publication because the reader needs to use the material exactly as the authors did to obtain their result.

Detailed definitions of these badges and the respective evaluation criteria may be found at the [ACM Artifact Review Badging site](https://www.acm.org/publications/policies/artifact-review-and-badging-current).

##   Important Dates (Authors and PC)

* Artifact Submission Deadline: 06.09.2024 
* Kick-the-tires author response period: 19.09.2024
* Deadline Author Response: 23.09.2024
* Author Notification: 11.10.2024

All dates are AOE.

##   Important Dates (PC)

* Deadline bidding on artifacts: 10.09.2024
* Assignment of artifacts to PC: 11.09.2024 
* Kick-the-tires evaluation: 18.09.2024 
* Artifact Assessment: 07.10.2024
* Artifact Discussion and Decision: 08-10.10.2024

All dates are AOE.

##   Further Information
For further information on the artifact evaluation of SLE 2024, feel free to contact the artifact evaluation chairs.

Best regards,
Sérgio Medeiros and Johannes Härtel
SLE24 Artifact Evaluation Co-Chairs

* sqmedeiros@gmail.com
* johanneshrtel@googlemail.com

##   Additional Hints

* An archive file (gz, xz, or zip) containing everything needed for supporting a full evaluation of the artifact. The archive file has to include at least the artifact itself and a text file named README.txt that contains the following information:
** An overview of the archive file, documenting the content of the archive.
** A setup/installation guide giving detailed instructions on how to setup or install the submitted artifact.
** Detailed step-by-step instructions on how to reproduce any experiments or other activities that support the conclusions given in the paper.
** When preparing your artifact, consider that your artifact should be as accessible to the AEC as possible. In particular, it should be possible for the AEC to quickly make progress in the investigation of your artifact. Please provide some simple scenarios describing concretely how the artifact is intended to be used. For a tool, this would include specific inputs to provide or actions to take, and expected output or behavior in response to this input.
* For artifacts that are tools, it is recommended to provide the tool installed and ready to use on a virtual machine for VirtualBox, VMware, SHARE, a Docker image, or a similar widely available platform.
* Please use widely supported open formats for documents (e.g., PDF, HTML) and data (e.g., CSV, JSON).