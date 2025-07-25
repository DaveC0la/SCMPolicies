# SCMPolicies
This repository gathers translation examples from the Security Capability Manager (SCM), an automated security policy enforcement framework. The primary purpose of this project is to translate abstract security intents from different domains into configurations specific to various security tools (known as Network Security Functions (NSFs)). The approach's success lies in its vendor-agnostic approach to securing information systems. It provides an intermediate layer in which security techniques can be described without accounting for the underlying protocols and devices. The framework autonomously enforces these abstract policies according to a formal model of security intents that we are constantly updating. This project is currently under development in the TORSEC research group at Politecnico di Torino.

The structure of the repository contains:
* a folder (**NSF_examples**) with a set of sub-directories consisting of policy examples translated by the SCM
    * Each of these sub-directories contains two files: an _Abstract\_Policy_ XML file, containing the abstract policy provided to the SCM for translation, and a _Low\_Level\_Policy_ text file, containing the policy translated for the target NSF
* a folder (**SCM_validation**) containing the strongSwan policies used to assess the versatility of the model in its channel protection subcomponents
* a folder (**CM-CP_Validation**) containing all the material used for validation purposes in writing the paper "A formal model of security capabilities for automated enforcement of channel protection", specifically:
    * *Abstract_Rules* is a file containing the two abstract rules for the gateways described in the validation infrastructure; these rules were provided to the SCM for translation and the outputs consist of the StrongSwan rules mentioned in the _Guide\_CM-CP\_Validation_ file;
    * *CM-CP* represents a screenshot of the portion of the _Capability Model_ that embodies the security capabilities for channel protection;
    * *Guide\_CM-CP\_Validation* is a file describing how to replicate the infrastructure for validating the secure channel configurations provided by the SCM

Future updates and additions will be documented in this README file.
