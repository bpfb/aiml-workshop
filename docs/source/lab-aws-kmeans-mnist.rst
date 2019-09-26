.. _AwsConsole: https://console.aws.amazon.com/

===========================
Lab - KMeans on MNIST (AWS)
===========================

Introduction
------------

This lab uses a SageMaker hosted Jupyter notebook example provided by AWS to demonstrate an a very basic application of machine learning using KMeans clustering on the MNIST data set.

Open the SageMaker Console
--------------------------

#. Go to the `AWS Console <AwsConsole_>`_.
#. Find the "Amazon SageMaker" service and click the link.

   .. image:: img/console.sagemaker.png
	 
Start a Notebook Instance
-------------------------
#. Click "Create notebook instance"
   or select an existing notebook instance and start it.

   .. image:: img/console.createinstance.png
	      
#. Once the instance is in service, select "Open Jupyter"
   
Get AWS Example Notebook
------------------------

#. When the Jupyter notebook has opened, select the "SageMaker Examples" tab.

   .. image:: img/sagemaker.examples.png

#. In the section *SageMaker Python SDK* select the notebook "kmeans_mnist.ipynb" and click "Use".  This will create a copy in your notebook instance.
   
   .. image:: img/sagemaker.kmeans_mnist.png
      
Launch the Notebook
-------------------

#. If it doesn't launch automatically, navigate to the notebook in the "Files" tab and and click on the .ipynb file to launch the notebook

   .. image:: img/sagemaker.kmeans_mnist_launch.png

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
