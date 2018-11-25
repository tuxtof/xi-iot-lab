.. _functions_main:

*********
Functions
*********

The FaceFeed application utilises functions within Data Pipelines to transform the incoming data (video feed) and draw inference (Face IDs).

The functions described in this step are a critical part of the way FaceFeed works and specify the "order" in which the various processing steps happen.

1. Login to the Nutanix Xi IoT Dashboard_ using the credentials that have been provided for you.
2. Using the "hamburger" button, expand the **Apps and Data** section and select **Functions**.  Note that we are now using the **Apps and Data** section instead of the **Infrastructure** section used up to this point.

.. figure:: ../images/hamburger.png

The functions we'll use have been created prior to this lab and have been made available on Github.

For **each** of the Python functions contained in the Github repository, please follow the steps below.

3. Browse to the Functions_ repository.
4. For each file there, e.g. **aggregatefeed.py**, click the filename then click **Raw**.
5. Copy the Python code to your clipboard or to your text editor.
6. In the Xi IoT console, while on the **Functions** page, click **Create**
7. Set the name of the function to the same name as the Python file without the **.py** extension, *maintaining case-sensititivity*.  For example, for the Python file **aggregatefeed.py**, set the function name to **aggregatefeed**.
8. Set the description to something meaningful.  Since these scripts are new to us, the description entered here doesn't really matter ...
9. Set the **Project** to the **FaceFeed** project we created earlier.
10. Set the **Language** to **Python**.
11. Set the **Runtime Environment** to **Tensorflow Python**.

.. figure:: ../images/create_function_general.png

12. Click **Next**.
13. Paste the code from step 5 into the text field provided.
14. Click **Create**.
15. Repeat steps 3-14 for each of the other 4 Python functions.

When you have completed the steps above, you will have 5 functions created.

.. figure:: ../images/create_function_final.png

Adding the Nutanix Xi IoT Functions is now complete.

.. _Dashboard: https://iot.nutanix.com/
.. _Functions: https://github.com/nutanix/xi-iot/tree/master/projects/facefeed/functions