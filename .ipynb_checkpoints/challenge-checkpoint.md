## **Stage 1 – Data Analysis Challenge for Solving Business Problems at CafeBazaar (October 2019)**

The attached file contains information about users of the Android app *Divar*:
🔗 [Download the dataset](https://drive.google.com/open?id=1rbXEGszvK1NpdPM0ULfI1Q4yN8Q6dKtN)

### **Dataset Columns:**

1. **adid**
   A unique identifier for each user.

2. **network\_name**
   The ad network through which the user installed the Divar app. Possible values:

   * `Organic`: Users who installed the app without seeing an ad.
   * `Tapsell`
   * `Adword UAC Installs`
   * `Cafebazaar searchad`

3. **installed\_at**
   The exact timestamp (to the second) when the app was installed.

4. **activity\_kind**
   The type of activity performed by the user. Possible values:

   * `install`
   * `event` – Refers to actions taken within the app.

5. **event\_name**
   Name of the event, if applicable. Only populated when `activity_kind = event`. Possible values:

   * `get_contact`: Clicking the “Contact Info” button on a listing page.
   * `new_post_submit`: Clicking the “Submit” button on the final screen of the posting process, marking the completion of creating a new post.

6. **created\_at**
   The exact timestamp (to the second) when the activity occurred.

---

### **Task Instructions:**

Start by verifying the cleanliness and accuracy of the data.

Then, address the following questions:

#### **1. User Quality Metrics by Network**

Define metrics to compare user quality across different ad networks. Two key metrics are:

* **Engagement Rate:**
  The percentage of users who performed *at least one important event* (`get_contact` or `new_post_submit`) **within 3 days of installing** the app.

* **Retention Rate:**
  Among users who performed an important event within 3 days, calculate the percentage who performed **any further event** within **30 days after their first event**.

🧮 Compute these two metrics for each ad network.
📊 Present the results using appropriate charts.

#### **2. Suspicious Behavior Detection**

If you observe any suspicious or anomalous patterns in the data, describe and visualize them using suitable charts.

