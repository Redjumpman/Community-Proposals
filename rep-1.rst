===============================
REP -- 1 Purpose and Guidelines
===============================

+---------+----------------------------+
| REP     | 1                          |
+---------+----------------------------+
| Status  | Draft                      |
+---------+----------------------------+
| Title   | REP Purpose and Guidelines |
+---------+----------------------------+
| Author  | Redjumpman                 |
+---------+----------------------------+
| Type    | Process                    |
+---------+----------------------------+
| Created | 06-Jun-2018                |
+---------+----------------------------+

.. contents:: Table of Contents

**************
What is a REP?
**************

REP stands for Red Enhancement Proposal. A REP is blueprint for the Red Community that details an organization process, informative guidelines, or a technical standard. The REP should be a concise technical specification that includes a breakdown of the justification for the proposal. The REP author is responsible for building consensus within the community and documenting dissenting opinions.

The REP process is intended to be the primary method for proposing new standards, features, and disciplines for the community. All finalized REPs will be archived and maintained on the Cog-Creators `Community-Proposals <https://github.com/Cog-Creators/Community-Proposals>`_ Github repository. Initial draft proposals will begin their journey on the `Cog Board <https://cogboard.red>`_ Community-Proposals discussion board. 

*********
REP Types
*********

There are two types of REPs:

- **Process**  
   A process REP is an organization proposal that changes or implements specific operating procedures for Red. They should require a community consensus, and upon implementation, require compliance from the user base. In addition, REPs of this type require a majority vote from Red's core developers, staff, and administrators.

- **Standards**  
   An informative REP provides guidelines or information on important components of the Red organization. An example of this kind of REP may be implementing a coding style (like black) or creating official information on roles and responsibilities.  A standards REP may also be included in conjunction with a process REP to provide additional supplemental information.

***********
REP Process
***********

The REP system is a 5 step process: Design, Submission, Review, Revise, and Resolve. Each step is a critical part of the process, and successful proposals follow this workflow. A draft REP has a life cycle no greater than 90 days. While a decision may be made before that time, a decision for rejection or acceptance will be made within 90 days of it's initial submission to Cog Board. 

.. image:: https://i.imgur.com/Cqfosf3.png
   :height: 950 px
   :width: 900 px
   :scale: 50 %
   :alt: REP Workflow
   :align: center

Design
^^^^^^

The REP process begins with an idea for Red. Each REP should attempt to encapsulate a single proposal or idea. The more limited the scope, the more successful it will be. REP reviewers have the right to reject proposals if they appear too unfocused or broad. Try limiting the scope or break your idea into several REPs.

Each REP must have an author, but can contain several co-authors. The author(s) role is to not only design and submit the REP, but to shepherd the community discussion and attempt to build a consensus around the idea.

An idea should be addressed and vetted publicly before submitting a REP. This is meant to save the author time, before trying to rally a community consensus around the idea. Asking the community about their thoughts before submitting a REP can save a lot of time or strengthen your proposal. Consider discussing your ideas on the official discord or Cog Board. 

Submission
^^^^^^^^^^^^^^^^^^^^^

* Fork the Cog-Creators `Community-Proposals <https://github.com/Cog-Creators/Community-Proposals>`_ repository.    

* Create a new file named `rep-9999.rst`      

* Design your rep and submit a post titled `REP TITLE` (where title is the name of your REP) to Community Proposals on Cog Board https://cogboard.red   

* The community, developers, and the community will weigh in on your proposal. Be sure to include any other supporting documents that may otherwise give more insight to your REP.   

* If your proposal is accepted, you will be asked to PR it to the Community-Proposals repository where it will be reviewed for any mistakes. This is also the stage where a number will be assigned to your REP.   

Review
^^^^^^^^^^

During the review process, you may be asked to change or update information to fit with the community or organization needs. Authors are responsible for collecting feedback from the community to strengthen their proposal. Dissenting ideas and counter-points are collected during this time. Having a list of counter-proposals and why they are not sufficient prevents have to defend the same question multiple times.

Resolution
^^^^^^^^^^^^^^

A REP cycle is every 90 days. At the end of it's cycle, if no comment for acceptance has been made, it will be officially closed and rejected. However, a REP may be rejected or accepted before this date. 

The final authority for REP approval is a majority vote from the core developers, staff, and administrators. For matters that do not affect the organization as a whole, such as a technical project specification, only a majority vote from the core developers is required. 

Once a REP has been officially accepted, you will be required to PR your proposal to the `Community-Proposals <https://github.com/Cog-Creators/Community-Proposals>`_ repository. It will then receive a final revision before being assigned a number and merged.


Maintenance
^^^^^^^^^^^^^^^
In general, Process type REPs are no longer modified after they have reached the Final state. Once a REP has been completed, the organization adopts this as the formal standard.

Standard type REPs may be updated over time to reflect changes to development practices and other organization details. The precise process followed in these cases will depend on the nature and purpose of the REP being updated.


******************************************
What Are The Elements of a Successful REP?
******************************************


* **Preamble** 
    Table containing meta-data about the REP, including the REP number, a short descriptive title (limited to a maximum of 44 characters), the type of REP, and the names of each author. The creation date will be the implementation date and changed at the time of final submission. 

* **Abstract**
    a short (~200 word) description of the issue being addressed.

* **Motivation** 
    The motivation is critical for REPs that want to change the Red organization. It should clearly explain why the existing mechanisms (or lack thereof) is inadequate to address the problem that the REP solves. REP submissions without sufficient motivation may be rejected outright.

* **Rationale** 
    The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other communities. The rationale should provide evidence of consensus within the community and discuss important objections or concerns raised during discussion.

* **Reference Documentation**
    The reference implementation must be completed before any REP is given status "Final", but it need not be completed before the REP is accepted.


**********
REP Header
**********
This must go at the top of your REP. Items marked with a * are optional.

+----------------+----------------------------------------+
| REP            | rep number                             |
+----------------+----------------------------------------+
| Title          | rep title                              |
+----------------+----------------------------------------+
| Author         | list of authors' discord names         |
+----------------+----------------------------------------+
| \*Sponsor      | REP endorsement discord names          |
+----------------+----------------------------------------+
| Status         | Draft Accepted \| Final  Superseded    |
+----------------+----------------------------------------+
| Type           | Standards  Process track               |
+----------------+----------------------------------------+
| \*Requires     | rep numbers                            |
+----------------+----------------------------------------+
| Created        | date created on, in dd-mmm-yyyy format |
+----------------+----------------------------------------+
| \*Replaces     | rep number                             |
+----------------+----------------------------------------+
| \*Superseded-By| rep number                             |
+----------------+----------------------------------------+

Sponsors are for core developers/staff/administrators who have helped to write or expressed their explicit endorsement. 

*************************
REP Formats and Templates
*************************

REPs are UTF-8 encoded text files using the reStructuredText format. REPs **MUST** be submitted in this format! No other format will be accepted. For more information on using reStructuredText please view the `Sphinx Documentation <http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_.

A blank template for writing your own REP can be found on the `Community-Proposals <https://github.com/Cog-Creators/Community-Proposals>`_ repository, labled template.rst
