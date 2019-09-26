.. _AwsConsole: https://console.aws.amazon.com/

=======================
Lab - City Checkbook
=======================

Introduction
------------

This lab uses a SageMaker hosted Jupyter notebook to demonstrate an exploration of City of Los Angeles purchase order data for supplies and services, as well as using an XGBoost machine learning algorithm to predict if a given invoice to the city will be paid in a timely manner.


Open the SageMaker Console
--------------------------

#. Go to the `AWS Console <AwsConsole_>`_.
#. Find the "Amazon SageMaker" service and click the link.

   .. image:: img/console.sagemaker.png
	      
Start a Notebook Instance
--------------------------
#. Click "Create notebook instance"
   or select an existing notebook instance and start it.

   .. image:: img/console.createinstance.png
	      
#. Once the instance is in service, select "Open Jupyter"
   
Clone git repository
--------------------

#. When the Jupyter notebook has opened, start a Terminal by selecting "New"->"Terminal"

   .. image:: img/sagemaker.start_terminal.png
      
#. In the terminal, type:

   #. ``cd SageMaker``
   #. ``git clone https://github.com/bpfb/aiml-workshop.git``
   #. ``exit``

#. Close the terminal tab

Launch the Notebook
-------------------

#. Navigate to "aiml-workshop/lab_city_checkbook/"
#. Select the notebook "City_Checkbook_aws.ipynb" to launch it

  .. image:: img/sagemaker.city_checkbook.png
	      
#. Follow the steps described in the notebook

Halting the Notebook
--------------------

#. When done with the notebook, select "File"->"Close and Halt"

  .. image:: img/sagemaker.close_and_halt.png
	      
#. With all notebooks halted, and terminals exited, you may quit Jupyter

  .. image:: img/sagemaker.quit.png
   
Stopping the Instance
---------------------

#. From the SageMaker dashboard, select the instance and choose "Stop" from the actions menu.  **The notebook instance will incur charges until stopped**.

   #. Stopping the instance leaves files and notebooks in place.  You can restart it at anytime, right where you left off.
   #. Make sure you **stop any endpoints** created by the notebook if you don't need them.  They accrue (significant) charges until stopped.

   .. image:: img/sagemaker.stop_instance.png


