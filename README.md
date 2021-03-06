# Model-based Fairness Analysis: A Sub-Framework of the MoPrivFair Methodology

This file presents the artifacts that are used in Chapter 4 of my PhD thesis, which provides a Framework for Analysing Individual Fairness based on Software Models. This framework is a sub-framework of the proposed MoPrivFair methodology in my thesis. The artifacts include:
* the *UMLfair profile*.

* The inputs and the outputs of applying our proposed framework on three case studies namely, the School Management System based on an artificail case study, the Delivery Management System based on the incedent describtion of [Amazon's delivery-free service](https://www.bloomberg.com/graphics/2016-amazon-same-day/), and the Loan Management System based on [business process model](https://link.springer.com/chapter/10.1007/978-3-319-92901-9_19) from an [event log](https://www.win.tue.nl/bpi/doku.php?id=2012:challenge) recording the loan management process of a Dutch financial institute. 

# Recources

* **Profile: The UMLfair Profile:** https://github.com/QRamadan/MoPrivFair-FairnessAnalysis/blob/master/profile.zip
* **Lunch configuration: The lucn configuration to the transformation tool hugo/RT:** https://github.com/QRamadan/MoPrivFair-FairnessAnalysis/blob/master/hugort.launch

* **Artifacts: The school management system case study:** https://github.com/QRamadan/MoPrivFair-FairnessAnalysis/blob/master/SchoolManagementSystem.zip
* **Artifacts: The delivery management system case study:** https://github.com/QRamadan/MoPrivFair-FairnessAnalysis/blob/master/DeliveryManagementSystem.zip
* **Artifacts: The loan management system case study:** https://github.com/QRamadan/MoPrivFair-FairnessAnalysis/blob/master/LoanManagementSystem.zip

The artifacts of each each case study contains: 
* A (*.uml*) file: the UML model of the system annotated with the UMLfair profile.
* A (*.xlsx*) file: the dataset of the system which used to uncover proxies for protected data. 
* a (.pml) file: the result of transforming the UML into PROMELA by using the [Hugo/RT](https://www.informatik.uni-augsburg.de/en/chairs/swt/sse/hugort/) tool. 
* a (*.pdf*) file: provides the generated batches of claims together with their verifications results. The verifiaction results are the output of  the [SPIN](http://spinroot.com/spin/whatispin.html) model checker. 
* a (*.trail*) files: counterexamples generated by the [SPIN](http://spinroot.com/spin/whatispin.html) model checker that explain the violated claims in the (*.pdf*) file.
