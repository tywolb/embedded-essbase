# Launch Embedded Essbase

## Introduction

In this lab, you will open embedded Essbase from Database Actions and sign-in with the Essbase user created in Lab 1. You will confirm that the Essbase home page is available before importing the PeakGear Sporting Goods application in the next lab.

Estimated Lab Time: 10 minutes

### About Essbase

Essbase provides multidimensional cubes for analyzing business data. In this workshop, Essbase is available from the Data Studio area of Database Actions in your existing Autonomous AI Lakehouse.

### Objectives

In this lab, you will:

- Launch Essbase from Data Studio.
- Sign in to Essbase and verify that it provisioned properly.
- Confirm the Import action is available for the Essbase user.

### Prerequisites

This lab assumes you have:

- Access to the existing Autonomous AI Lakehouse with embedded Essbase enabled.
- The workshop user's Database Actions URL, username, and password from Lab 1.

## Task 1: Launch Essbase from Data Studio

1. Return to your AI Lakehouse details page.
![Essbase Login](images/ailh_2a.png)

2. Click on **Tool Configuration** from the ribbon options.
![Essbase Login](images/t1.png)

3. Scroll down to **Essbase** then click **Edit**.
![Essbase Login](images/t2.png)

4. Toggle **Enable Essbase** on and click apply. You can configure the OCPU count and idle time here as well.
![Essbase Login](images/t3.png)

5. After AI Lakehouse finishes updating, copy the URL under Essbase and paste it in a new browser window. Once the Essbase login page appears, proceed to Task 2.

    > **Note:** Alternatively, launch Essbase by copying the Database actions URL from the search bar and replace `/ords/...` with `/essbase/jet`
![Essbase Login](images/t4.png)

## Task 2: Verify the Essbase Home Page and Signed-In User

1. On the Essbase sign-in page, enter the username and password for the workshop user created in Lab 1.
![Essbase Login](images/essbase1.png)

2. Select **Sign In**. Essbase will take a few minutes to provision when the first user logs in.

3. Confirm that the Essbase home page opens and that you are signed in as the workshop user.
![Essbase Login](images/temp4.png)

4. Locate the **Applications** area and the **Import** action. You will import and verify the prepared PeakGear application in the next lab.
![Essbase Login](images/ess2.png)

    > **Note:** If the Essbase user cannot sign-in to Essbase, return to Data Actions as the ADMIN user and refer to Lab 1 Task 3.

You have launched embedded Essbase and verified the workshop user's sign-in.

## Learn More

- [Connect with Built-In Oracle Database Actions](https://docs.oracle.com/en/cloud/paas/autonomous-database/serverless/adbsb/connect-database-actions.html)
- [Using the Oracle Essbase Web Interface](https://docs.oracle.com/en/database/other-databases/essbase/26/ugess/index.html)

## Acknowledgements

* **Author** - Ty Wolber, Cloud Engineer
* **Last Updated By/Date** - Ty Wolber, October 2026